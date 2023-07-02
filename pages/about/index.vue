<template>
<div class="bg-gray-900">
  <!-- Header -->
  <header class="absolute inset-x-0 top-0 z-50">
    <nav class="mx-auto flex max-w-7xl items-center justify-between p-6 lg:px-8" aria-label="Global">
      <div class="flex lg:flex-1">
        <a href="#" class="-m-1.5 p-1.5">
          <span class="sr-only">Your Company</span>
          <img class="h-8 w-auto" src= "/.../static/resus.png" alt="">
        </a>
      </div>
      <div class="flex lg:hidden">
        <button type="button" class="-m-2.5 inline-flex items-center justify-center rounded-md p-2.5 text-gray-400">
          <span class="sr-only">Open main menu</span>
          <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true">
            <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
          </svg>
        </button>
      </div>
      <div class="hidden lg:flex lg:gap-x-12">
        <a href="/" class="text-sm font-semibold leading-6 text-white">Home</a>
      </div>
     
    </nav>
    <!-- Mobile menu, show/hide based on menu open state. -->
    <div class="lg:hidden" role="dialog" aria-modal="true">
      <!-- Background backdrop, show/hide based on slide-over state. -->
      <div class="fixed inset-0 z-50"></div>
      <div class="fixed inset-y-0 right-0 z-50 w-full overflow-y-auto bg-gray-900 px-6 py-6 sm:max-w-sm sm:ring-1 sm:ring-white/10">
        <div class="flex items-center justify-between">
          <a href="#" class="-m-1.5 p-1.5">
            <span class="sr-only">Your Company</span>
            <img class="h-8 w-auto" src="https://tailwindui.com/img/logos/mark.svg?color=indigo&shade=500" alt="">
          </a>
          <button type="button" class="-m-2.5 rounded-md p-2.5 text-gray-400">
            <span class="sr-only">Close menu</span>
            <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true">
              <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
            </svg>
          </button>
        </div>
        <div class="mt-6 flow-root">
          <div class="-my-6 divide-y divide-gray-500/25">
            <div class="space-y-2 py-6">
              <a href="/" class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-white hover:bg-gray-800">Product</a>
             
            </div>
            <div class="py-6">
              <a href="#" class="-mx-3 block rounded-lg px-3 py-2.5 text-base font-semibold leading-7 text-white hover:bg-gray-800">Log in</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </header>

  <main class="relative isolate">
    <!-- Background -->
    <div class="absolute inset-x-0 top-4 -z-10 flex transform-gpu justify-center overflow-hidden blur-3xl" aria-hidden="true">
      <div class="aspect-[1108/632] w-[69.25rem] flex-none bg-gradient-to-r from-[#80caff] to-[#4f46e5] opacity-25" style="clip-path: polygon(73.6% 51.7%, 91.7% 11.8%, 100% 46.4%, 97.4% 82.2%, 92.5% 84.9%, 75.7% 64%, 55.3% 47.5%, 46.5% 49.4%, 45% 62.9%, 50.3% 87.2%, 21.3% 64.1%, 0.1% 100%, 5.4% 51.1%, 21.4% 63.9%, 58.9% 0.2%, 73.6% 51.7%)"></div>
    </div>

    <!-- Header section -->
    <div class="px-6 pt-14 lg:px-8">
      <div class="mx-auto max-w-2xl pt-24 text-center sm:pt-40">
        <h2 class="text-4xl font-bold tracking-tight text-white sm:text-6xl">We love Coffee</h2>
        <p class="mt-6 text-lg leading-8 text-gray-300">Resus Cafe: A cup of coffee, a slice of heaven.</p>
      </div>
    </div>
    <div class="mx-auto mt-20 max-w-7xl px-6 lg:px-8">
      <div class="mx-auto max-w-2xl lg:mx-0 lg:max-w-none">
        <div class="grid max-w-xl grid-cols-1 gap-8 text-base leading-7 text-gray-300 lg:max-w-none lg:grid-cols-2">
          <div>
            <p>Resus Cafe is a coffee shop located in Riyadh, Saudi Arabia. We are committed to providing our customers with the best possible coffee experience. We offer a wide variety of coffee drinks, pastries, and sandwiches, all made with fresh, high-quality ingredients. Our staff is friendly and knowledgeable, and we are always happy to help you find the perfect drink or food item.</p>
          </div>
          <div>
            <p>Our mission is to provide our customers with a comfortable and welcoming space to enjoy a cup of coffee and relax. We believe that coffee is more than just a drink; it is a way to connect with others and enjoy the moment. We hope that our customers will leave our cafe feeling refreshed and happy.</p>
            <p class="mt-8">Resus Cafe was founded in 2012 by two friends who were passionate about coffee. They started out with a small coffee shop in Riyadh, but they quickly grew in popularity. Today, Resus Cafe has several locations throughout Riyadh and is one of the most popular coffee shops in the city.</p>
          </div>
        </div>
        <dl class="mt-16 grid grid-cols-1 gap-x-8 gap-y-12 sm:mt-20 sm:grid-cols-2 sm:gap-y-16 lg:mt-28 lg:grid-cols-4">
          <div class="flex flex-col-reverse gap-y-3 border-l border-white/20 pl-6">
            <dt class="text-base leading-7 text-gray-300">Business was founded</dt>
            <dd class="text-3xl font-semibold tracking-tight text-white">2012</dd>
          </div>
          <div class="flex flex-col-reverse gap-y-3 border-l border-white/20 pl-6">
            <dt class="text-base leading-7 text-gray-300">People on the team</dt>
            <dd class="text-3xl font-semibold tracking-tight text-white">120+</dd>
          </div>
          <div class="flex flex-col-reverse gap-y-3 border-l border-white/20 pl-6">
            <dt class="text-base leading-7 text-gray-300">Kilion of beans sold</dt>
            <dd class="text-3xl font-semibold tracking-tight text-white">250k</dd>
          </div>
          <div class="flex flex-col-reverse gap-y-3 border-l border-white/20 pl-6">
            <dt class="text-base leading-7 text-gray-300">Valuation</dt>
            <dd class="text-3xl font-semibold tracking-tight text-white">$70M</dd>
          </div>
        </dl>
      </div>
    </div>
    <footer aria-labelledby="footer-heading" class="bg-white">
        <h2 id="footer-heading" class="sr-only">Footer</h2>
        <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
          <div class="py-10 md:flex md:items-center md:justify-between">
            <div class="text-center md:text-left">
              <p class="text-md text-black">مؤسسة أغذيتي لتقديم الوجبات</p>

              <p class="text-md text-black">5044، عيسى الملاجي، الصفا، 5043</p>

              <p class="text-md text-black">0500028516</p>
            </div>

            <div class="mt-4 flex items-center justify-center md:mt-0">
              <div class="flex space-x-8">
                <a
                  href="https://instagram.com/resuscafe.sa?igshid=ZWQyN2ExYTkwZQ==
"
                  class="text-sm text-gray-500 hover:text-gray-600"
                  >instagram</a
                >

                <a
                  href="https://maps.app.goo.gl/7PzMp5afBX7rHxVG9?g_st=ic"
                  class="text-sm text-gray-500 hover:text-gray-600"
                  >Location</a
                >
                <a
                  href="/about"
                  class="text-sm text-gray-500 hover:text-gray-600"
                  >About</a
                >
              </div>

              <div class="ml-6 border-l border-gray-200 pl-6">
                <a
                  href="#"
                  class="flex items-center text-gray-500 hover:text-gray-600"
                >
                  <img
                    src="https://icons.iconarchive.com/icons/wikipedia/flags/72/SA-Saudi-Arabia-Flag-icon.png"
                    alt=""
                    class="h-auto w-5 flex-shrink-0"
                  />
                </a>
              </div>
            </div>
          </div>
        </div>
      </footer>


    
  </main>


  
</div>

</template>

<script>
export default {

}
</script>

<style>

</style>