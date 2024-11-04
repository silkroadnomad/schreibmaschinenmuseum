<script lang="ts">
  import { Link } from "svelte-routing";
</script>

<nav class="bg-white shadow-lg">
  <div class="container mx-auto px-4">
    <div class="flex justify-between items-center h-16">
      <Link to="/" class="text-xl font-bold text-gray-800">Typewriter Museum</Link>
      <div class="flex space-x-4">
        <Link to="/" class="text-gray-600 hover:text-gray-800">Home</Link>
        <Link to="/blog" class="text-gray-600 hover:text-gray-800">Blog</Link>
        <Link to="/about" class="text-gray-600 hover:text-gray-800">About</Link>
        <Link to="/contact" class="text-gray-600 hover:text-gray-800">Contact</Link>
      </div>
    </div>
  </div>
</nav>