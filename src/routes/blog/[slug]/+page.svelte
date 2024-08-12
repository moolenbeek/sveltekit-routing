<script lang="ts">
  import { page } from '$app/stores';
  export let data;
</script>

<div class="container h-full mx-auto flex justify-center items-center">
  <div class="space-y-5">
    <br>
    <a href="/blog">blog</a> / {$page.params.slug}
    <h1>{data.post.title}</h1>
    <div>{@html data.post.content}</div>
  </div>
</div>
