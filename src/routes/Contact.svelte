<script lang="ts">
  let formData = {
    name: '',
    email: '',
    subject: '',
    message: ''
  };

  function handleSubmit() {
    // Form submission logic would go here
    alert('Thank you for your message. We will get back to you soon!');
    formData = {
      name: '',
      email: '',
      subject: '',
      message: ''
    };
  }
</script>

<div class="max-w-2xl mx-auto">
  <h1 class="text-4xl font-bold mb-8">Contact Us</h1>

  <div class="bg-white rounded-lg shadow-md p-8">
    <form on:submit|preventDefault={handleSubmit} class="space-y-6">
      <div>
        <label for="name" class="block text-sm font-medium text-gray-700 mb-1">Name</label>
        <input
          type="text"
          id="name"
          bind:value={formData.name}
          required
          class="w-full px-4 py-2 border border-gray-300 rounded-md focus:ring-blue-500 focus:border-blue-500"
        />
      </div>

      <div>
        <label for="email" class="block text-sm font-medium text-gray-700 mb-1">Email</label>
        <input
          type="email"
          id="email"
          bind:value={formData.email}
          required
          class="w-full px-4 py-2 border border-gray-300 rounded-md focus:ring-blue-500 focus:border-blue-500"
        />
      </div>

      <div>
        <label for="subject" class="block text-sm font-medium text-gray-700 mb-1">Subject</label>
        <input
          type="text"
          id="subject"
          bind:value={formData.subject}
          required
          class="w-full px-4 py-2 border border-gray-300 rounded-md focus:ring-blue-500 focus:border-blue-500"
        />
      </div>

      <div>
        <label for="message" class="block text-sm font-medium text-gray-700 mb-1">Message</label>
        <textarea
          id="message"
          bind:value={formData.message}
          required
          rows="4"
          class="w-full px-4 py-2 border border-gray-300 rounded-md focus:ring-blue-500 focus:border-blue-500"
        ></textarea>
      </div>

      <button
        type="submit"
        class="w-full bg-blue-600 text-white py-2 px-4 rounded-md hover:bg-blue-700 transition-colors"
      >
        Send Message
      </button>
    </form>

    <div class="mt-8 pt-8 border-t border-gray-200">
      <h2 class="text-xl font-semibold mb-4">Other Ways to Reach Us</h2>
      <div class="space-y-4 text-gray-600">
        <p>
          <strong>Email:</strong> info@typewritermuseum.at
        </p>
        <p>
          <strong>Phone:</strong> +43 1 234 5678
        </p>
        <p>
          <strong>Address:</strong><br>
          Schreibmaschinenmuseum<br>
          Herrengasse 23<br>
          1010 Vienna, Austria
        </p>
      </div>
    </div>
  </div>
</div>