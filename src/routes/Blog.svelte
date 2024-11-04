<script lang="ts">
  const posts = [
    {
      title: "The History of QWERTY Layout",
      date: "2024-03-15",
      excerpt: "Discover how the QWERTY keyboard layout became the global standard...",
      image: "/images/qwerty.jpg"
    },
    {
      title: "Collecting Vintage Typewriters",
      date: "2024-03-10",
      excerpt: "Tips and tricks for starting your own typewriter collection...",
      image: "/images/collecting.jpg"
    }
  ];
</script>

<div class="max-w-4xl mx-auto">
  <h1 class="text-3xl font-bold mb-8">Latest News</h1>
  
  <div class="space-y-8">
    {#each posts as post}
      <article class="bg-white rounded-lg shadow-md overflow-hidden">
        <img src={post.image} alt={post.title} class="w-full h-48 object-cover"/>
        <div class="p-6">
          <h2 class="text-2xl font-bold mb-2">{post.title}</h2>
          <p class="text-gray-500 text-sm mb-4">{post.date}</p>
          <p class="text-gray-600">{post.excerpt}</p>
          <button class="mt-4 text-blue-600 hover:text-blue-800">Read more →</button>
        </div>
      </article>
    {/each}
  </div>
</div>