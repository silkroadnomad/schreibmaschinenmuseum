<script lang="ts">
  import TypewriterCard from '../components/TypewriterCard.svelte';

  const typewriters = [
    {
      title: "Remington No. 1",
      image: "remington1",
      year: "1874",
      country: "USA",
      price: "2.5",
      tokenId: "1"
    },
    {
      title: "Continental Standard",
      image: "continental",
      year: "1892",
      country: "Germany",
      price: "3.0",
      tokenId: "2"
    },
    {
      title: "Hermes 3000",
      image: "hermes",
      year: "1958",
      country: "Switzerland",
      price: "1.8",
      tokenId: "3"
    },
    {
      title: "Olivetti Lettera 22",
      image: "olivetti",
      year: "1950",
      country: "Italy",
      price: "2.2",
      tokenId: "4"
    },
    {
      title: "Underwood No. 5",
      image: "underwood",
      year: "1901",
      country: "USA",
      price: "4.0",
      tokenId: "5"
    },
    {
      title: "Royal Quiet De Luxe",
      image: "royal",
      year: "1939",
      country: "USA",
      price: "2.8",
      tokenId: "6"
    }
  ];
</script>

<div class="text-center mb-12">
  <h1 class="text-4xl font-bold mb-4">Welcome to the Austrian Typewriter Museum</h1>
  <p class="text-xl text-gray-600">Discover our collection of historic typewriters available as NFTs</p>
</div>

<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
  {#each typewriters as typewriter}
    <TypewriterCard {...typewriter} />
  {/each}
</div>