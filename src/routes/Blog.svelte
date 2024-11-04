<script lang="ts">
  const posts = [
    {
      title: "The History of QWERTY Layout",
      date: "2024-03-15",
      excerpt: "Discover how the QWERTY keyboard layout became the global standard...",
      image: "https://images.unsplash.com/photo-1703248184547-13cee07c05b2?q=80&w=3174&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
    },
    {
      title: "Collecting Vintage Typewriters",
      date: "2024-03-10",
      excerpt: "Tips and tricks for starting your own typewriter collection...",
      image: "https://images.unsplash.com/photo-1703925154762-c3d2086c3535?q=80&w=3174&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
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