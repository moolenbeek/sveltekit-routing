<script lang="ts">
  import { page } from "$app/stores";
  export let data;
</script>

<div class="container p-4">
  <a href="/blog">blog</a> / {$page.params.slug}
  <div class="justify-center p-4">
    <h1>{data.post.title}</h1>
    <div>{@html data.post.content}</div>
  </div>
</div>
