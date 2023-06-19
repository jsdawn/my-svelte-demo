<script>
  // import '@colorfuldots/svelteit/dist/css/svelteit.min.css';

  import Router from 'svelte-spa-router';
  import Home from './pages/Home.svelte';
  import About from './pages/About.svelte';
  import Blog from './pages/Blog.svelte';
  import BlogPost from './pages/BlogPost.svelte';

  const routes = {
    // Exact path
    '/': Home,

    // Using named parameters, with last being optional
    '/blog': Blog,

    // Wildcard parameter
    '/about': About,

    // Catch-all
    // This is optional, but if present it must be the last
    '*': BlogPost,
  };
</script>

<nav>
  <a href="/">Home</a>
  <a href="#/blog">blog</a>
  <a href="#/about">about</a>
</nav>

<Router {routes} />
