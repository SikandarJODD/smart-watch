<script>
  let prdoucttitle = "Product  Collections";
  let pgtext =
    "This is a section of some simple filler text, also known as placeholder text. It shares some characteristics of a real written text but is random or otherwise generated.";

  let pgdata = [
    {
      id: 1,
      title: "ColorFit Caliber Buzz",
      brand: "Fancy Brand",
      price: "Rs.1,999",
      oldprice: "Rs.2,500",
      img: "https://cdn.shopify.com/s/files/1/0997/6284/products/Artboard3_1d215692-f72e-445b-aca5-fd5107f47d2d.png?v=1673941537",
      imgalt: "Photo by Austin Wade",
    },
    {
      id: 2,
      title: "ColorFit Caliber 2 Buzz",
      brand: "Cool Brand",
      price: "Rs.1,999",
      oldprice: "",
      img: "https://cdn.shopify.com/s/files/1/0997/6284/products/1_49b76d4f-6c8b-4fce-9061-89e05f1eb7f1.png?v=1669294148",
    },
    {
      id: 3,
      title: "ColorFit Pro 3",
      brand: "Funky Brand",
      price: "Rs.3,500",
      oldprice: "",
      img: "https://cdn.shopify.com/s/files/1/0997/6284/products/NoiseColoFitPro3Smartwatch-1stImage_1.png?v=1627585572",
    },
    {
      id: 4,
      title: "Noise ColorFit Pulse",
      brand: "Tunky Brand",
      price: "Rs.2,500",
      oldprice: "",
      img: "https://cdn.shopify.com/s/files/1/0997/6284/products/NoisePulse1stImageNew_1.png?v=1655378598",
    },
    {
      id: 5,
      title: "ColorFit Pulse 2",
      brand: "Funky Brand",
      price: "Rs.1,500",
      oldprice: "",
      img: "https://cdn.shopify.com/s/files/1/0997/6284/products/image_2022_07_13T14_17_32_557Z.png?v=1657764046",
    },
    {
      id: 6,
      title: "ColorFit Vision 2",
      brand: "Tunky Brand",
      price: "Rs.1,300",
      oldprice: "",
      img: "https://cdn.shopify.com/s/files/1/0997/6284/products/center.png?v=1656047411",
    },
    {
      id: 7,
      title: "Evolve 2 Play",
      brand: "Funky Brand",
      price: "₹1,499",
      oldprice: "",
      img: "https://cdn.shopify.com/s/files/1/0997/6284/products/Black1_3806338e-c756-4c25-bc61-b955a4a5df11.png?v=1674061195",
    },
    {
      id: 8,
      title: "ColorFit Icon 2",
      brand: "Tunky Brand",
      price: "₹1,300",
      oldprice: "",
      img: "https://cdn.shopify.com/s/files/1/0997/6284/products/Artboard11_10f875bf-f9aa-48d9-ac83-b97abe2b5c25.png?v=1672654462",
    },
  ];
</script>

<div class="bg-gray-900 py-6 sm:py-8 lg:py-20">
  <div class="max-w-screen-2xl px-4 md:px-8 mx-auto">
    <!-- text - start -->
    <div class="mb-10 md:mb-16">
      <h2
        class="text-sky-400 main_hero text-2xl lg:text-5xl font-bold text-center mb-4 md:mb-6"
      >
        {prdoucttitle}
      </h2>

      <p class="max-w-screen-md text-slate-500 md:text-lg text-center mx-auto">
        {pgtext}
      </p>
    </div>
    <!-- text - end -->

    <div
      class="grid sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-x-4 md:gap-x-6 gap-y-8"
    >
      <!-- product - start -->
      {#each pgdata as product}
        <div>
          <a
            href="/products"
            class="group h-96 block bg-gray-100 rounded-lg overflow-hidden shadow-lg relative mb-2 lg:mb-3"
          >
            <!-- svelte-ignore a11y-img-redundant-alt -->
            <img
              src={product.img}
              loading="lazy"
              alt="Photo by Nick Karvounis"
              class="w-full h-full object-fill object-center group-hover:scale-110 transition duration-200"
            />
          </a>

          <div class="flex justify-between items-start gap-2 px-2">
            <div class="flex flex-col">
              <a
                href="/products"
                class="text-slate-300 hover:text-sky-400 text-lg lg:text-xl font-bold transition duration-100"
                >{product.title}</a
              >
              <span class="text-slate-500">by {product.brand}</span>
            </div>

            <div class="flex flex-col items-end">
              <span class="text-cyan-400 lg:text-lg font-bold"
                >{product.price}</span
              >
            </div>
          </div>
        </div>
      {/each}
    </div>
  </div>
</div>
