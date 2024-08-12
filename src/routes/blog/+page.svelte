<script lang="ts">
  export let data;
</script>

<div class="container h-full mx-auto flex justify-center items-center">
  <div class="space-y-5">
    <h1>this is the blog page.</h1>

    <ul class="list">
      {#each data.summaries as { slug, title }}
        <li>
          <span class="flex-auto"><a href="/blog/{slug}">{title}</a></span>
        </li>
      {/each}
    </ul>
  </div>
</div>
