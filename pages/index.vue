<template>
  <!-- component -->
  <div>
    <!--
  This example requires some changes to your config:
  
  ```
  // tailwind.config.js
  module.exports = {
    // ...
    plugins: [
      // ...
      require('@tailwindcss/forms'),
      require('@tailwindcss/aspect-ratio'),
    ],
  }
  ```
-->
    <div class="bg-white">
      <!--
    Mobile menu

    Off-canvas menu for mobile, show/hide based on off-canvas menu state.
  -->
      <div class="relative z-40 lg:hidden" role="dialog" aria-modal="false">
        <!--
      Off-canvas menu backdrop, show/hide based on off-canvas menu state.

      Entering: "transition-opacity ease-linear duration-300"
        From: "opacity-0"
        To: "opacity-100"
      Leaving: "transition-opacity ease-linear duration-300"
        From: "opacity-100"
        To: "opacity-0"
    -->
        <div class="fixed inset-0 bg-black bg-opacity-25"></div>

        <div class="fixed inset-0 z-40 flex">
          <!--
        Off-canvas menu, show/hide based on off-canvas menu state.

        Entering: "transition ease-in-out duration-300 transform"
          From: "-translate-x-full"
          To: "translate-x-0"
        Leaving: "transition ease-in-out duration-300 transform"
          From: "translate-x-0"
          To: "-translate-x-full"
      -->
        </div>
      </div>

      <header class="relative z-10">
        <nav aria-label="Top">
          <!-- Top navigation -->
          

          <!-- Secondary navigation -->
          <div class="bg-white">
            <div class="border-b border-gray-200">
              <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
                <div class="flex h-16 items-center justify-between">

                  <div class="hidden h-full lg:flex">
                    <p class="text-4xl py-4">
                    مؤسسة أغذيتي لتقديم الوجبات

                    </p>
                  </div>

                  <!-- Mobile menu and search (lg-) -->
                  <div class="flex flex-1 items-center lg:hidden">
                    <!-- Mobile menu toggle, controls the 'mobileMenuOpen' state. -->
                    <button
                      type="button"
                      class="-ml-2 rounded-md bg-white p-2 text-gray-400"
                    >
                      <span class="sr-only">Open menu</span>
                      <!-- Heroicon name: outline/bars-3 -->
                      <svg
                        class="h-6 w-6"
                        xmlns="http://www.w3.org/2000/svg"
                        fill="none"
                        viewBox="0 0 24 24"
                        stroke-width="1.5"
                        stroke="currentColor"
                        aria-hidden="true"
                      >
                        <path
                          stroke-linecap="round"
                          stroke-linejoin="round"
                          d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
                        />
                      </svg>
                    </button>

                    <!-- Search -->
                    
                  </div>

                  <!-- Logo (lg-) -->

                  
                </div>
              </div>
            </div>
          </div>
        </nav>
      </header>

      <main>
        <!-- Hero -->
        <div class="flex flex-col border-b border-gray-200 lg:border-0">
          

          <div class="relative">
            <div
              aria-hidden="true"
              class="absolute hidden h-full w-1/2 bg-gray-100 lg:block"
            ></div>
            <div class="relative bg-gray-100 lg:bg-transparent">
              <div
                class="mx-auto max-w-7xl px-4 sm:px-6 lg:grid lg:grid-cols-2 lg:px-8"
              >
                <div class="mx-auto max-w-2xl py-24 lg:max-w-none lg:py-64">
                  <div class="lg:pr-16">
                    <h1
                      class="text-4xl font-bold tracking-tight text-gray-900 sm:text-5xl xl:text-6xl"
                    >
                      مؤسسة أغذيتي لتقديم الوجبات
                    </h1>
                    <p class="mt-4 text-xl text-gray-600">
                      Better Beans, Better Coffee
                    </p>
                    
                  </div>
                </div>
              </div>
            </div>
            <div
              class="h-48 w-full sm:h-64 lg:absolute lg:top-0 lg:right-0 lg:h-full lg:w-1/2"
            >
              <img
                src="../static/resus.png"
                alt=""
                class="h-full w-full object-cover object-center"
              />
            </div>
          </div>
        </div>

       
        <!-- Collections -->
        

        <!-- Sale and testimonials -->
        <div class="relative overflow-hidden">
          <!-- Decorative background image and gradient -->
          <div aria-hidden="true" class="absolute inset-0">
            <div
              class="absolute inset-0 mx-auto max-w-7xl overflow-hidden xl:px-8"
            >
              <img
                src="https://tailwindui.com/img/ecommerce-images/home-page-02-sale-full-width.jpg"
                alt=""
                class="h-full w-full object-cover object-center"
              />
            </div>
            <div class="absolute inset-0 bg-white bg-opacity-75"></div>
            <div
              class="absolute inset-0 bg-gradient-to-t from-white via-white"
            ></div>
          </div>

          <!-- Sale -->

          <!-- Testimonials -->
        </div>
      </main>

      <footer aria-labelledby="footer-heading" class="bg-white">
        <h2 id="footer-heading" class="sr-only">Footer</h2>
        <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">

          <div class="py-10 md:flex md:items-center md:justify-between">
            <div class="text-center md:text-left">
              <p class="text-2xl text-black">  مؤسسة أغذيتي لتقديم الوجبات </p>
               
            
<p class="text-2xl text-black">
  5044، عيسى الملاجي، الصفا، 5043
</p>

<p class="text-2xl text-black">
  0500028516
</p>
            
            </div>

            <div class="mt-4 flex items-center justify-center md:mt-0">
              <div class="flex space-x-8">
                <a href="#" class="text-sm text-gray-500 hover:text-gray-600"
                  >Accessibility</a
                >

                <a href="#" class="text-sm text-gray-500 hover:text-gray-600"
                  >Privacy</a
                >

                <a href="#" class="text-sm text-gray-500 hover:text-gray-600"
                  >Terms</a
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
                  <span class="ml-3 text-sm">Change</span>
                  <span class="sr-only">location and currency</span>
                </a>
              </div>
            </div>
          </div>
        </div>
      </footer>
    </div>
  </div>
</template>
