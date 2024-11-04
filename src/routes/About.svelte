<script lang="ts">
  import { Link } from "svelte-routing";
</script>

<div class="max-w-4xl mx-auto">
  <h1 class="text-4xl font-bold mb-8">About Our Museum</h1>
  
  <section class="bg-white rounded-lg shadow-md p-8 mb-8">
    <h2 class="text-2xl font-semibold mb-4">Our History</h2>
    <p class="text-gray-600 mb-4">
      Founded in 1985, the Austrian Typewriter Museum has been preserving and showcasing the rich history of typewriters 
      for over three decades. Located in the heart of Vienna, our museum houses one of Europe's most extensive collections 
      of vintage typewriters, spanning from the earliest models to late 20th-century innovations.
    </p>
  </section>

  <section class="bg-white rounded-lg shadow-md p-8 mb-8">
    <h2 class="text-2xl font-semibold mb-4">NFT Initiative</h2>
    <p class="text-gray-600 mb-4">
      In 2024, we launched our groundbreaking NFT program, revolutionizing how historical artifacts can be owned and 
      preserved. Each typewriter in our collection is digitally tokenized, allowing enthusiasts worldwide to own a piece 
      of typing history while supporting the museum's conservation efforts.
    </p>
    <div class="bg-blue-50 border-l-4 border-blue-500 p-4">
      <h3 class="text-lg font-semibold text-blue-700 mb-2">How It Works</h3>
      <ul class="list-disc list-inside text-gray-600 space-y-2">
        <li>Each NFT represents ownership of a physical typewriter in our collection</li>
        <li>NFT holders receive exclusive access to detailed documentation and history</li>
        <li>Owners can visit their typewriter in person at any time</li>
        <li>All proceeds support museum preservation and expansion</li>
      </ul>
    </div>
  </section>

  <section class="bg-white rounded-lg shadow-md p-8">
    <h2 class="text-2xl font-semibold mb-4">Visit Us</h2>
    <div class="grid md:grid-cols-2 gap-8">
      <div>
        <h3 class="text-lg font-semibold mb-2">Opening Hours</h3>
        <ul class="text-gray-600 space-y-1">
          <li>Tuesday - Friday: 10:00 - 18:00</li>
          <li>Saturday - Sunday: 11:00 - 16:00</li>
          <li>Monday: Closed</li>
        </ul>
      </div>
      <div>
        <h3 class="text-lg font-semibold mb-2">Location</h3>
        <p class="text-gray-600">
          Schreibmaschinenmuseum<br>
          Herrengasse 23<br>
          1010 Vienna, Austria
        </p>
      </div>
    </div>
    <Link 
      to="/contact" 
      class="inline-block mt-6 bg-blue-600 text-white py-2 px-4 rounded hover:bg-blue-700 transition-colors"
    >
      Contact Us
    </Link>
  </section>
</div>