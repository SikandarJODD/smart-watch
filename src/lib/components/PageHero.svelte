<script>
  let mainTitle = "Matrix Build Character in Time";
  let subTitle = "#ChangeYourTime";
  let PageText =
    "Matrix  is a company that provides a wide range of services to help you build your character in <i>time</i>.";
  let btn1 = "Products";
  let btn2 = "Learn More";
</script>

<section class="bg-gray-900 text-white">
  <div
    class="mx-auto max-w-screen-xl px-4 py-32 lg:flex lg:h-screen lg:items-center"
  >
    <div class="mx-auto max-w-6xl text-center  ">
      <h1
        class="bg-gradient-to-r from-green-300 via-blue-400 to-purple-700 bg-clip-text text-3xl font-extrabold text-transparent sm:text-6xl pb-3"
      >
        {mainTitle}

        <span class="sm:block "> {subTitle} </span>
      </h1>

      <p class="mx-auto mt-4 max-w-xl sm:text-xl sm:leading-relaxed">
        {@html PageText}
      </p>

      <div class="mt-8 flex flex-wrap justify-center gap-4">
        <a
          class="block w-full rounded border border-blue-600 bg-blue-600 px-12 py-3 text-sm font-medium text-white hover:bg-transparent hover:text-white focus:outline-none focus:ring active:text-opacity-75 sm:w-auto"
          href="/products"
        >
          {btn1}
        </a>

        <a
          class="block w-full rounded border border-blue-600 px-12 py-3 text-sm font-medium text-white hover:bg-blue-600 focus:outline-none focus:ring active:bg-blue-500 sm:w-auto"
          href="/about"
        >
          {btn2}
        </a>
      </div>
    </div>
  </div>
</section>
