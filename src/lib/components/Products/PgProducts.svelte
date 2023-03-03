<script>
  let prdoucttitle = "Product Collections";
  let pgtext =
    "This is a section of some simple filler text, also known as placeholder text. It shares some characteristics of a real written text but is random or otherwise generated.";

  let pgdata = [
    {
      id: 1,
      title: "Fancy Outfit",
      brand: "Fancy Brand",
      price: "$19.99",
      oldprice: "$39.99",
      img: "https://i.pinimg.com/564x/f7/d1/3a/f7d13acad6cb754438fd5a9da3d78818.jpg",
      imgalt: "Photo by Austin Wade",
    },
    {
      id: 2,
      title: "Cool Outfit",
      brand: "Cool Brand",
      price: "$29.99",
      oldprice: "",
      img: "https://i.pinimg.com/564x/20/83/06/208306ef7f5659a46c2b1c592e7851d2.jpg",
    },
    {
      id: 3,
      title: "Funky Outfit",
      brand: "Funky Brand",
      price: "$39.99",
      oldprice: "",
      img: "https://i.pinimg.com/564x/f5/b3/b7/f5b3b7a64c253f882bfdd4337c7721ac.jpg",
    },
    {
      id: 4,
      title: "Tunky Outfit",
      brand: "Tunky Brand",
      price: "$49.99",
      oldprice: "",
      img: "https://images.pexels.com/photos/1183266/pexels-photo-1183266.jpeg?auto=compress&cs=tinysrgb&w=600",
    },
    {
      id: 5,
      title: "Funky Outfit",
      brand: "Funky Brand",
      price: "$39.99",
      oldprice: "",
      img: "https://i.pinimg.com/564x/a2/ea/98/a2ea989a1bc308ca8dfe9b2b30e93918.jpg",
    },
    {
      id: 6,
      title: "Tunky Outfit",
      brand: "Tunky Brand",
      price: "$49.99",
      oldprice: "",
      img: "https://i.pinimg.com/564x/4d/d3/de/4dd3debfeaf25d0e935505eb81eb288f.jpg",
    },
    {
      id: 7,
      title: "Funky Outfit",
      brand: "Funky Brand",
      price: "$39.99",
      oldprice: "",
      img: "https://i.pinimg.com/750x/da/1f/c9/da1fc9118f89831b25a0e5303350edc7.jpg",
    },
    {
      id: 8,
      title: "Tunky Outfit",
      brand: "Tunky Brand",
      price: "$49.99",
      oldprice: "",
      img: "https://i.pinimg.com/564x/05/fb/84/05fb8402f6b786dde6c69d09e545c8b0.jpg",
    },
  ];
</script>

<div class="bg-gray-900 py-6 sm:py-8 lg:py-12">
  <div class="max-w-screen-2xl px-4 md:px-8 mx-auto">
    <!-- text - start -->
    <div class="mb-10 md:mb-16">
      <h2
        class="text-sky-300 text-2xl lg:text-4xl font-bold text-center mb-4 md:mb-6"
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
              class="w-full h-full object-cover object-center group-hover:scale-110 transition duration-200"
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
