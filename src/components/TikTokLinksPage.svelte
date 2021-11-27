<script>
  import TikTokLinkElement from "./TiktokLinksComponents/TiktokLinkElement.svelte";

  export let data = [];
</script>

<div class="div-size">
  {#each data as element (element.id)}<TikTokLinkElement
      title={element.title}
      link={element.link}
    />{/each}
</div>

<style>
</style>
