<script>
  import UpperPage from "./components/UpperPage.svelte";
  import TiktokLinksPage from "./components/TiktokLinksPage.svelte";
  import LowerPage from "./components/LowerPage.svelte";

  let data = [
    {
      id: "0",
      title: "TikTok Account",
      link: "https://www.tiktok.com/@galaxytheprogrammer",
    },
    {
      id: "1",
      title: "Svelte Framework",
      link: "https://svelte.dev/",
    },
    {
      id: "2",
      title: "MIT License",
      link: "https://choosealicense.com/licenses/mit/",
    },
  ];

  let pageData = {
    page_title: "TikTok Link Menu",
    page_desc: "Made by 'GalaxyTheProgrammer' using the Svelte Framework!",
    footnote: [
      {
        id: "0",
        data: "PS: Svelte is amazing and you should use it in my opinion",
      },
      {
        id: "1",
        data: "Svelte have not paid me to say this!",
      },
      {
        id: "2",
        data: "© 2021 GalaxyGamingBoy",
      },
      {
        id: "3",
        data: " ( MIT LICENSE )",
      },
    ],
  };
</script>

<main>
  <UpperPage {pageData} />
  <TiktokLinksPage {data} />
  <LowerPage footnoteData={pageData.footnote} />
</main>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
