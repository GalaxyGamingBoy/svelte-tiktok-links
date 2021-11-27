<script>
  import TikTokLinkTitle from "./components/TikTokLinkTitle.svelte";
  import SHSS from "../Snippets/SSHS.svelte";

  export let title = "";
  export let link = "";

  function link_clicked() {
    console.log("Clicked: " + title + " - " + link);
    window.open(link);
  }
</script>

<div>
  <button
    type="button"
    class="btn btn-primary btn-size"
    on:click={link_clicked}
  >
    <TikTokLinkTitle>{title}</TikTokLinkTitle></button
  >
</div>

<SHSS />

<style>
  .btn-size {
    width: 100%;
    white-space: normal;
  }
</style>
