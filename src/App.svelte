<script lang="ts">
  import { Router, Link, Route } from "svelte-routing";
  import Navbar from './components/Navbar.svelte';
  import Home from './routes/Home.svelte';
  import Blog from './routes/Blog.svelte';
  import About from './routes/About.svelte';
  import Contact from './routes/Contact.svelte';
</script>

<Router>
  <main class="min-h-screen bg-gray-50">
    <Navbar />
    <div class="container mx-auto px-4 py-8">
      <Route path="/" component={Home} />
      <Route path="/blog" component={Blog} />
      <Route path="/about" component={About} />
      <Route path="/contact" component={Contact} />
    </div>
  </main>
</Router>