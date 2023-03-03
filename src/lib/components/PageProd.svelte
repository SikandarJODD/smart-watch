<script>
  let title = "Vintage Cars";
  let img1 =
    "https://i.pinimg.com/564x/d1/44/bc/d144bca97b033bdb904bf7c313cf2c93.jpg";
  let img2 =
    "https://i.pinimg.com/564x/0a/8a/c0/0a8ac0cbaa1e69e295fb9ceb98deed99.jpg";
  let btn = "View All";
  let text =
    "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quas rerum quam amet provident nulla error!";
</script>

<section class="bg-gray-900">
  <div class="max-w-screen-xl px-4 py-8 mx-auto sm:py-12 sm:px-6 lg:px-8">
    <div class="grid grid-cols-1 gap-4 lg:grid-cols-3 lg:items-stretch">
      <div
        class="grid p-6 bg-gradient-to-b from-slate-600 to-gray-900 rounded place-content-center sm:p-8 shadow-2xl"
      >
        <div class="max-w-md mx-auto text-center lg:text-left">
          <header>
            <h2 class="text-xl font-bold text-sky-500 sm:text-5xl">
              {title}
            </h2>

            <p class="mt-4 text-slate-400">
              {text}
            </p>
          </header>

          <a
            href="/products"
            class="inline-block px-12 py-3 mt-8 text-sm font-medium text-white transition bg-blue-600 border border-blue-600 hover:bg-transparent rounded hover:shadow focus:outline-none focus:ring"
          >
            {btn}
          </a>
        </div>
      </div>

      <div class="lg:col-span-2 lg:py-8">
        <ul class="grid grid-cols-2 gap-4">
          <li>
            <a
              href="/products"
              class="block group shadow-2xl hover:shadow-cyan-500 transition duration-200"
            >
              <img
                src={img1}
                alt=""
                class="object-cover w-full rounded aspect-square"
              />
            </a>
          </li>

          <li>
            <a
              href="/products"
              class="block group shadow-2xl hover:shadow-cyan-500 transition duration-200"
            >
              <img
                src={img2}
                alt=""
                class="object-cover w-full rounded aspect-square"
              />
            </a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</section>
