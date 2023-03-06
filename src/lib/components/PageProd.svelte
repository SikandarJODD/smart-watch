<script>
  import Img1 from "$lib/img1.webp";
  import Img2 from "$lib/img2.webp";
  let title = "Smart Watch";
  // let img1 ="https://i.pinimg.com/564x/d1/44/bc/d144bca97b033bdb904bf7c313cf2c93.jpg";
  let img1 = Img1;
  // let img2 ="https://i.pinimg.com/564x/0a/8a/c0/0a8ac0cbaa1e69e295fb9ceb98deed99.jpg";
  let img2 = Img2;
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
            <h2 class="text-xl font-bold text-cyan-400 sm:text-5xl">
              {title}
            </h2>

            <p class="mt-4 text-slate-400">
              {text}
            </p>
          </header>

          <a
            href="/products"
            class="inline-block px-12 py-3 mt-8 text-sm font-medium text-white transition bg-blue-600 border border-blue-600 hover:bg-transparent focus:outline-none focus:ring"
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
              class="block group  filter transition duration-200"
            >
              <img
                src={img1}
                alt=""
                class="object-cover w-full rounded aspect-square hover:scale-110 duration-200 transition-all imgShadow "
              />
            </a>
          </li>
          <li>
            <a href="/products" class="block group  transition duration-200">
              <img
                src={img2}
                alt=""
                class="object-cover w-full rounded aspect-square hover:scale-110 duration-200 transition-all imgShadow "
              />
            </a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</section>

<style>
  .imgShadow:hover {
    transition: all 0.3s ease;
    filter: drop-shadow(0 0 0.9rem rgb(33, 150, 246));
  }
</style>
