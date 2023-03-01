<script>
  import ImgGallery from "../lib/components/ImgGallery.svelte";
  import PageHero from "../lib/components/PageHero.svelte";
  import PageProd from "../lib/components/PageProd.svelte";
</script>

<svelte:head>
  <title>Funky Tunky | Home Page</title>
</svelte:head>
<main>
  <PageHero />
  <PageProd />
  <ImgGallery />
</main>

<style lang="postcss">
  :global(html) {
    background-color: theme(colors.gray.100);
  }
</style>
