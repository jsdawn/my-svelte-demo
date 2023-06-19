<script>
  import { link } from 'svelte-spa-router';

  let title = 'Blog!';
</script>

<h1>{title}</h1>
<a href="/blog/233" use:link>BlogPost</a>
