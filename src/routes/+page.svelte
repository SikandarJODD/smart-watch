<script>
  import FeaturesPage from "$lib/components/FeaturesPage.svelte";
  import ImgGallery from "$lib/components/ImgGallery.svelte";
  import PageHero from "$lib/components/PageHero.svelte";
  import PageProd from "$lib/components/PageProd.svelte";
  import PageStats from "$lib/components/PageStats.svelte";
  import Logo from "$lib/wristwatch.png";
</script>

<svelte:head>
  <title>Matrix | Home Page</title>
  <link rel="shortcut icon" href={Logo} type="image/x-icon" />
  <meta name="description" content="Building Character Takes Time - Matrix" />
  <meta
    name="og:image"
    content="https://cdn-icons-png.flaticon.com/512/9335/9335046.png"
  />
  <meta name="keywords" content="Watch,Matrix,Smart Watch" />
</svelte:head>
<main>
  <PageHero />
  <PageProd />
  <ImgGallery />
  <FeaturesPage />
  <PageStats />
</main>
