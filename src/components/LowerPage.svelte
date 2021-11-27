<script>
  import LowerPageLine from "./LowerPageComponents/LowerPageLine.svelte";

  export let footnoteData = [];
</script>

{#each footnoteData as ftC (ftC.id)}
  <LowerPageLine data={ftC.data} />
{/each}
