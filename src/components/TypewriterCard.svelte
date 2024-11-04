<script lang="ts">
  import TypewriterImage from './TypewriterImage.svelte';
  
  export let title: string;
  export let image: string;
  export let year: string;
  export let country: string;
  export let price: string;
  export let tokenId: string;

  async function buyNFT() {
    // NFT purchase logic would go here
    alert('NFT purchase functionality will be implemented with Web3 integration');
  }
</script>

<div class="bg-white rounded-lg shadow-md overflow-hidden">
  <TypewriterImage {title} />
  <div class="p-4">
    <h3 class="text-xl font-semibold mb-2">{title}</h3>
    <p class="text-gray-600">Year: {year}</p>
    <p class="text-gray-600">Country: {country}</p>
    <p class="text-lg font-bold mt-2">{price} ETH</p>
    <button 
      on:click={buyNFT}
      class="mt-4 w-full bg-blue-600 text-white py-2 px-4 rounded hover:bg-blue-700 transition-colors"
    >
      Buy NFT
    </button>
  </div>
</div>