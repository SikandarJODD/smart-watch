<script>
  import Img3 from "$lib/img3.jpg";
  import Img4 from "$lib/img4.png";
  import Img6 from "$lib/img6.jpg";
  import Img7 from "$lib/img7.jpg";
  let img1 = Img3;
  // Short img2
  let img2 = Img6;
  let img3 = Img7;
  // Short img4
  let img4 = Img4;
</script>

<div class="bg-gray-900 py-6 sm:py-8 lg:py-12 md:px-24">
  <div class="max-w-screen-2xl px-4 md:px-8 mx-auto">
    <div class="grid grid-cols-2 sm:grid-cols-3 gap-4 md:gap-6 xl:gap-8">
      <!-- image - start -->
      <a
        href="/"
        class="group h-48 md:h-80 flex items-end  overflow-hidden rounded-lg shadow-lg relative"
      >
        <!-- svelte-ignore a11y-img-redundant-alt -->
        <img
          src={img1}
          loading="lazy"
          alt="Photo by Minh Pham"
          class="w-full h-full object-cover object-center absolute inset-0 group-hover:scale-110 transition duration-200"
        />

        <div
          class="bg-gradient-to-t from-gray-800 via-transparent to-transparent opacity-50 absolute inset-0 pointer-events-none"
        />

        <!-- <span
          class="inline-block text-white text-sm md:text-lg relative ml-4 md:ml-5 mb-3"
          >VR</span
        > -->
      </a>
      <!-- image - end -->

      <!-- image - start -->
      <a
        href="/"
        class="group h-48 md:h-80 md:col-span-2 flex items-end  overflow-hidden rounded-lg shadow-lg relative"
      >
        <!-- svelte-ignore a11y-img-redundant-alt -->
        <img
          src={img2}
          loading="lazy"
          alt="Photo by Magicle"
          class="w-full h-full object-full  absolute inset-0 group-hover:scale-110 transition duration-200"
        />

        <div
          class="bg-gradient-to-t from-gray-800 via-transparent to-transparent opacity-50 absolute inset-0 pointer-events-none"
        />

        <!-- <span
          class="inline-block text-white text-sm md:text-lg relative ml-4 md:ml-5 mb-3"
          >Tech</span
        > -->
      </a>
      <!-- image - end -->

      <!-- image - start -->
      <a
        href="/"
        class="group h-48 md:h-80 md:col-span-2 flex items-end  overflow-hidden rounded-lg shadow-lg relative"
      >
        <!-- svelte-ignore a11y-img-redundant-alt -->
        <img
          src={img3}
          loading="lazy"
          alt="Photo by Martin Sanchez"
          class="w-full h-full object-cover object-center absolute inset-0 group-hover:scale-110 transition duration-200"
        />

        <div
          class="bg-gradient-to-t from-gray-800 via-transparent to-transparent opacity-50 absolute inset-0 pointer-events-none"
        />

        <!-- <span
          class="inline-block text-white text-sm md:text-lg relative ml-4 md:ml-5 mb-3"
          >Dev</span
        > -->
      </a>
      <!-- image - end -->

      <!-- image - start -->
      <a
        href="/"
        class="group h-48 md:h-80 flex items-end  overflow-hidden rounded-lg shadow-lg relative "
      >
        <!-- svelte-ignore a11y-img-redundant-alt -->
        <img
          src={img4}
          loading="lazy"
          alt="Photo by Lorenzo Herrera"
          class="w-full h-full object-cover object-center absolute inset-0 group-hover:scale-110   transition duration-200"
        />

        <div
          class="bg-gradient-to-t from-gray-800 via-transparent to-transparent opacity-50 absolute inset-0 pointer-events-none"
        />

        <!-- <span
          class="inline-block text-white text-sm md:text-lg relative ml-4 md:ml-5 mb-3"
          >Retro</span
        > -->
      </a>
      <!-- image - end -->
    </div>
  </div>
</div>
