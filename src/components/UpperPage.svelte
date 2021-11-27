<script>
  import SHSS from "./Snippets/SSHS.svelte";
  import UpperPageTitle from "./UpperPageComponents/UpperPageTitle.svelte";
  import UpperPageDesc from "./UpperPageComponents/UpperPageDesc.svelte";

  export let pageData = {};
</script>

<UpperPageTitle title={pageData.page_title} />
<UpperPageDesc desc={pageData.page_desc} />
<SHSS />
