<script>
  import FeaturesPage from "$lib/components/FeaturesPage.svelte";
  import ImgGallery from "$lib/components/ImgGallery.svelte";
  import PageHero from "$lib/components/PageHero.svelte";
  import PageProd from "$lib/components/PageProd.svelte";
  import PageStats from "$lib/components/PageStats.svelte";
</script>

<svelte:head>
  <title>Funky Tunky | Home Page</title>
</svelte:head>
<main>
  <PageHero />
  <PageProd />
  <ImgGallery />
  <FeaturesPage />
  <PageStats />
</main>
