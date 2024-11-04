<script lang="ts">
  export let title: string;
  
  // Generate a unique but consistent seed for each typewriter
  function generateSeed(text: string): number {
    let hash = 0;
    for (let i = 0; i < text.length; i++) {
      const char = text.charCodeAt(i);
      hash = ((hash << 5) - hash) + char;
      hash = hash & hash;
    }
    return Math.abs(hash);
  }

  // Generate a placeholder image URL with consistent colors for each typewriter
  function generateImageUrl(title: string): string {
    const seed = generateSeed(title);
    const hue = seed % 360;
    const saturation = 70;
    const lightness = 60;
    
    return `https://placehold.co/600x400/hsl(${hue},${saturation}%,${lightness}%)/333333?text=${encodeURIComponent(title)}`;
  }

  $: imageUrl = generateImageUrl(title);
</script>

<img 
  src={imageUrl} 
  alt={title}
  class="w-full h-48 object-cover"
  loading="lazy"
/>