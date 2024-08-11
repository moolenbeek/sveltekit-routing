<script lang="ts">
  import { page } from "$app/stores";
  import { TabGroup, Tab, TabAnchor } from "@skeletonlabs/skeleton";
</script>

<TabGroup>
  <TabAnchor href="/" selected={$page.url.pathname === "/"}>Home</TabAnchor>
  <TabAnchor href="/about" selected={$page.url.pathname === "/about"}>About</TabAnchor>
  <TabAnchor href="/contact" selected={$page.url.pathname === "/contact"}>Contact</TabAnchor>
</TabGroup>

<div class="container h-full mx-auto flex justify-center items-center">
  <div class="space-y-5">
    <h1>this is the contact page.</h1>
  </div>
</div>
