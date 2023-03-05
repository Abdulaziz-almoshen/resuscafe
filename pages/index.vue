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
          <div class="bg-gray-900">
            <div
              class="mx-auto flex h-10 max-w-7xl items-center justify-between px-4 sm:px-6 lg:px-8"
            >
              <!-- Currency selector -->
              <form class="hidden lg:block lg:flex-1">
                <div class="flex">
                  <label for="desktop-currency" class="sr-only">Currency</label>
                  <div
                    class="group relative -ml-2 rounded-md border-transparent bg-gray-900 focus-within:ring-2 focus-within:ring-white"
                  >
                    <select
                      id="desktop-currency"
                      name="currency"
                      class="flex items-center rounded-md border-transparent bg-gray-900 bg-none py-0.5 pl-2 pr-5 text-sm font-medium text-white focus:border-transparent focus:outline-none focus:ring-0 group-hover:text-gray-100"
                    >
                      <option>CAD</option>

                      <option>USD</option>

                      <option>AUD</option>

                      <option>EUR</option>

                      <option>GBP</option>
                    </select>
                    <div
                      class="pointer-events-none absolute inset-y-0 right-0 flex items-center"
                    >
                      <!-- Heroicon name: mini/chevron-down -->
                      <svg
                        class="h-5 w-5 text-gray-300"
                        xmlns="http://www.w3.org/2000/svg"
                        viewBox="0 0 20 20"
                        fill="currentColor"
                        aria-hidden="true"
                      >
                        <path
                          fill-rule="evenodd"
                          d="M5.23 7.21a.75.75 0 011.06.02L10 11.168l3.71-3.938a.75.75 0 111.08 1.04l-4.25 4.5a.75.75 0 01-1.08 0l-4.25-4.5a.75.75 0 01.02-1.06z"
                          clip-rule="evenodd"
                        />
                      </svg>
                    </div>
                  </div>
                </div>
              </form>

              <p
                class="flex-1 text-center text-sm font-medium text-white lg:flex-none"
              >
                Get free delivery on orders over $100
              </p>

              <div
                class="hidden lg:flex lg:flex-1 lg:items-center lg:justify-end lg:space-x-6"
              >
                <a
                  href="#"
                  class="text-sm font-medium text-white hover:text-gray-100"
                  >Create an account</a
                >
                <span class="h-6 w-px bg-gray-600" aria-hidden="true"></span>
                <a
                  href="#"
                  class="text-sm font-medium text-white hover:text-gray-100"
                  >Sign in</a
                >
              </div>
            </div>
          </div>

          <!-- Secondary navigation -->
          <div class="bg-white">
            <div class="border-b border-gray-200">
              <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
                <div class="flex h-16 items-center justify-between">
                  <!-- Logo (lg+) -->
                  <div class="hidden lg:flex lg:items-center">
                    <a href="#">
                      <span class="sr-only">Your Company</span>
                      <img
                        class="h-8 w-auto"
                        src="https://scontent.fruh4-6.fna.fbcdn.net/v/t39.30808-6/243547962_1063021347901551_6553224124569965068_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=TREgUPftLoIAX-_hQ5x&_nc_ht=scontent.fruh4-6.fna&oh=00_AfCzNvdtlqvQAXqyQz8kmTexs9zi312js1_zK3MN3oM7ow&oe=63C091C2"
                        alt=""
                      />
                    </a>
                  </div>

                  <div class="hidden h-full lg:flex">
                    <!-- Mega menus -->
                    <div class="ml-8">
                      <div class="flex h-full justify-center space-x-8">
                        <div class="flex">
                          <div class="relative flex">
                            <!-- Item active: "border-indigo-600 text-indigo-600", Item inactive: "border-transparent text-gray-700 hover:text-gray-800" -->
                            <button
                              type="button"
                              class="border-transparent text-gray-700 hover:text-gray-800 relative z-10 -mb-px flex items-center border-b-2 pt-px text-sm font-medium transition-colors duration-200 ease-out"
                              aria-expanded="false"
                            >
                              Beans
                            </button>
                          </div>

                          <!--
                        'Women' mega menu, show/hide based on flyout menu state.

                        Entering: "transition ease-out duration-200"
                          From: "opacity-0"
                          To: "opacity-100"
                        Leaving: "transition ease-in duration-150"
                          From: "opacity-100"
                          To: "opacity-0"
                      -->
                          
                        </div>

                        <div class="flex">
                          <div class="relative flex">
                            <!-- Item active: "border-indigo-600 text-indigo-600", Item inactive: "border-transparent text-gray-700 hover:text-gray-800" -->
                            <button
                              type="button"
                              class="border-transparent text-gray-700 hover:text-gray-800 relative z-10 -mb-px flex items-center border-b-2 pt-px text-sm font-medium transition-colors duration-200 ease-out"
                              aria-expanded="false"
                            >
                              Cups
                            </button>
                          </div>

                          <!--
                        'Men' mega menu, show/hide based on flyout menu state.

                        Entering: "transition ease-out duration-200"
                          From: "opacity-0"
                          To: "opacity-100"
                        Leaving: "transition ease-in duration-150"
                          From: "opacity-100"
                          To: "opacity-0"
                      -->
                          <div
                            class="absolute inset-x-0 top-full text-gray-500 sm:text-sm"
                          >
                            <!-- Presentational element used to render the bottom shadow, if we put the shadow on the actual panel it pokes out the top, so we use this shorter element to hide the top of the shadow -->
                            <div
                              class="absolute inset-0 top-1/2 bg-white shadow"
                              aria-hidden="true"
                            ></div>

                            
                          </div>
                        </div>

                        <a
                          href="#"
                          class="flex items-center text-sm font-medium text-gray-700 hover:text-gray-800"
                          >Company</a
                        >

                        <a
                          href="#"
                          class="flex items-center text-sm font-medium text-gray-700 hover:text-gray-800"
                          >Stores</a
                        >
                      </div>
                    </div>
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
                    <a
                      href="#"
                      class="ml-2 p-2 text-gray-400 hover:text-gray-500"
                    >
                      <span class="sr-only">Search</span>
                      <!-- Heroicon name: outline/magnifying-glass -->
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
                          d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z"
                        />
                      </svg>
                    </a>
                  </div>

                  <!-- Logo (lg-) -->
                  <a href="#" class="lg:hidden">
                    <span class="sr-only">Your Company</span>
                    <img
                      src="https://scontent.fruh4-6.fna.fbcdn.net/v/t39.30808-6/243547962_1063021347901551_6553224124569965068_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=TREgUPftLoIAX-_hQ5x&_nc_ht=scontent.fruh4-6.fna&oh=00_AfCzNvdtlqvQAXqyQz8kmTexs9zi312js1_zK3MN3oM7ow&oe=63C091C2"
                      alt="https://scontent.fruh4-6.fna.fbcdn.net/v/t39.30808-6/243547962_1063021347901551_6553224124569965068_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=TREgUPftLoIAX-_hQ5x&_nc_ht=scontent.fruh4-6.fna&oh=00_AfCzNvdtlqvQAXqyQz8kmTexs9zi312js1_zK3MN3oM7ow&oe=63C091C2"
                      class="h-8 w-auto"
                    />
                  </a>

                  <div class="flex flex-1 items-center justify-end">
                    <div class="flex items-center lg:ml-8">
                      <div class="flex space-x-8">
                        <div class="hidden lg:flex">
                          <a
                            href="#"
                            class="-m-2 p-2 text-gray-400 hover:text-gray-500"
                          >
                            <span class="sr-only">Search</span>
                            <!-- Heroicon name: outline/magnifying-glass -->
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
                                d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z"
                              />
                            </svg>
                          </a>
                        </div>

                        <div class="flex">
                          <a
                            href="#"
                            class="-m-2 p-2 text-gray-400 hover:text-gray-500"
                          >
                            <span class="sr-only">Account</span>
                            <!-- Heroicon name: outline/user -->
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
                                d="M15.75 6a3.75 3.75 0 11-7.5 0 3.75 3.75 0 017.5 0zM4.501 20.118a7.5 7.5 0 0114.998 0A17.933 17.933 0 0112 21.75c-2.676 0-5.216-.584-7.499-1.632z"
                              />
                            </svg>
                          </a>
                        </div>
                      </div>

                      <span
                        class="mx-4 h-6 w-px bg-gray-200 lg:mx-6"
                        aria-hidden="true"
                      ></span>

                      <div class="flow-root">
                        <a href="#" class="group -m-2 flex items-center p-2">
                          <!-- Heroicon name: outline/shopping-cart -->
                          <svg
                            class="h-6 w-6 flex-shrink-0 text-gray-400 group-hover:text-gray-500"
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
                              d="M2.25 3h1.386c.51 0 .955.343 1.087.835l.383 1.437M7.5 14.25a3 3 0 00-3 3h15.75m-12.75-3h11.218c1.121-2.3 2.1-4.684 2.924-7.138a60.114 60.114 0 00-16.536-1.84M7.5 14.25L5.106 5.272M6 20.25a.75.75 0 11-1.5 0 .75.75 0 011.5 0zm12.75 0a.75.75 0 11-1.5 0 .75.75 0 011.5 0z"
                            />
                          </svg>
                          <span
                            class="ml-2 text-sm font-medium text-gray-700 group-hover:text-gray-800"
                            >0</span
                          >
                          <span class="sr-only">items in cart, view bag</span>
                        </a>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </nav>
      </header>

      <main>
        <!-- Hero -->
        <div class="flex flex-col border-b border-gray-200 lg:border-0">
          <nav aria-label="Offers" class="order-last lg:order-first">
            <div class="mx-auto max-w-7xl lg:px-8">
              <ul
                role="list"
                class="grid grid-cols-1 divide-y divide-gray-200 lg:grid-cols-3 lg:divide-y-0 lg:divide-x"
              >
                <li class="flex flex-col">
                  <a
                    href="#"
                    class="relative flex flex-1 flex-col justify-center bg-white py-6 px-4 text-center focus:z-10"
                  >
                    <p class="text-sm text-gray-500">Download the app</p>
                    <p class="font-semibold text-gray-900">
                      Get an exclusive $5 off code
                    </p>
                  </a>
                </li>

                <li class="flex flex-col">
                  <a
                    href="#"
                    class="relative flex flex-1 flex-col justify-center bg-white py-6 px-4 text-center focus:z-10"
                  >
                    <p class="text-sm text-gray-500">
                      Return when you&#039;re ready
                    </p>
                    <p class="font-semibold text-gray-900">
                      60 days of free returns
                    </p>
                  </a>
                </li>

                <li class="flex flex-col">
                  <a
                    href="#"
                    class="relative flex flex-1 flex-col justify-center bg-white py-6 px-4 text-center focus:z-10"
                  >
                    <p class="text-sm text-gray-500">
                      Sign up for our newsletter
                    </p>
                    <p class="font-semibold text-gray-900">
                      15% off your first order
                    </p>
                  </a>
                </li>
              </ul>
            </div>
          </nav>

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
                      Focus on coffee
                    </h1>
                    <p class="mt-4 text-xl text-gray-600">
                      Better Beans, Better Coffee
                    </p>
                    <div class="mt-6">
                      <a
                        href="#"
                        class="inline-block rounded-md border border-transparent bg-red-300 py-3 px-8 font-medium text-white hover:bg-indigo-700"
                        >Shop Branches</a
                      >
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div
              class="h-48 w-full sm:h-64 lg:absolute lg:top-0 lg:right-0 lg:h-full lg:w-1/2"
            >
              <img
              src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSP_47cBMQhOScClx-AXzWymXR9dSBantm3RtWTEaaSiybTqzq7PczYgz1qT7Ry-NHX3fE&usqp=CAU"
                alt=""
                class="h-full w-full object-cover object-center"
              />
            </div>
          </div>
        </div>

        <!-- Trending products -->
        <section aria-labelledby="trending-heading" class="bg-white">
          <div class="py-16 sm:py-24 lg:mx-auto lg:max-w-7xl lg:py-32 lg:px-8">
            <div class="flex items-center justify-between px-4 sm:px-6 lg:px-0">
              <h2
                id="trending-heading"
                class="text-2xl font-bold tracking-tight text-gray-900"
              >
                Trending products
              </h2>
              <a
                href="#"
                class="hidden text-sm font-semibold text-indigo-600 hover:text-indigo-500 sm:block"
              >
                See everything
                <span aria-hidden="true"> &rarr;</span>
              </a>
            </div>

            <div class="relative mt-8">
              <div class="relative w-full overflow-x-auto">
                <ul
                  role="list"
                  class="mx-4 inline-flex space-x-8 sm:mx-6 lg:mx-0 lg:grid lg:grid-cols-4 lg:gap-x-8 lg:space-x-0"
                >
                  <li class="inline-flex w-64 flex-col text-center lg:w-auto">
                    <div class="group relative">
                      <div
                        class="aspect-w-1 aspect-h-1 w-full overflow-hidden rounded-md bg-gray-200"
                      >
                        <img
                          src="https://i.etsystatic.com/22823368/r/il/8cd262/2396270395/il_fullxfull.2396270395_7ajx.jpg"
                          alt="Black machined steel pen with hexagonal grip and small white logo at top."
                          class="h-full w-full object-cover object-center group-hover:opacity-75"
                        />
                      </div>
                      <div class="mt-6">
                        <p class="text-sm text-gray-500">Spicy</p>
                        <h3 class="mt-1 font-semibold text-gray-900">
                          <a href="#">
                            <span class="absolute inset-0"></span>
                            Spicy Chicken
                          </a>
                        </h3>
                        <p class="mt-1 text-gray-900">$35</p>
                      </div>
                    </div>

                    
                  </li>

                  <!-- More products... -->
                </ul>
              </div>
            </div>

            <div class="mt-12 px-4 sm:hidden">
              <a
                href="#"
                class="text-sm font-semibold text-indigo-600 hover:text-indigo-500"
              >
                See everything
                <span aria-hidden="true"> &rarr;</span>
              </a>
            </div>
          </div>
        </section>

        <!-- Collections -->
        <section aria-labelledby="collections-heading" class="bg-gray-100">
          <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
            <div
              class="mx-auto max-w-2xl py-16 sm:py-24 lg:max-w-none lg:py-32"
            >
              <h2
                id="collections-heading"
                class="text-2xl font-bold text-gray-900"
              >
                Collections
              </h2>

              <div
                class="mt-6 space-y-12 lg:grid lg:grid-cols-3 lg:gap-x-6 lg:space-y-0"
              >
                <div class="group relative">
                  <div
                    class="relative h-80 w-full overflow-hidden rounded-lg bg-white group-hover:opacity-75 sm:aspect-w-2 sm:aspect-h-1 sm:h-64 lg:aspect-w-1 lg:aspect-h-1"
                  >
                    <img
                      src="data:image/jpeg;base64,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"
                      alt="Desk with leather desk pad, walnut desk organizer, wireless keyboard and mouse, and porcelain mug."
                      class="h-full w-full object-cover object-center"
                    />
                  </div>
                  <h3 class="mt-6 text-sm text-gray-500">
                    <a href="#">
                      <span class="absolute inset-0"></span>
                      Egyption
                    </a>
                  </h3>
                  <p class="text-base font-semibold text-gray-900">
                    Beans
                  </p>
                </div>

                <div class="group relative">
                  <div
                    class="relative h-80 w-full overflow-hidden rounded-lg bg-white group-hover:opacity-75 sm:aspect-w-2 sm:aspect-h-1 sm:h-64 lg:aspect-w-1 lg:aspect-h-1"
                  >
                    <img
                      src="https://i.etsystatic.com/22823368/r/il/18898e/2396290687/il_570xN.2396290687_jq56.jpg"
                      alt="Wood table with porcelain mug, leather journal, brass pen, leather key ring, and a houseplant."
                      class="h-full w-full object-cover object-center"
                    />
                  </div>
                  <h3 class="mt-6 text-sm text-gray-500">
                    <a href="#">
                      <span class="absolute inset-0"></span>
                      Saudi
                    </a>
                  </h3>
                  <p class="text-base font-semibold text-gray-900">
                    Beans
                  </p>
                </div>

                <div class="group relative">
                  <div
                    class="relative h-80 w-full overflow-hidden rounded-lg bg-white group-hover:opacity-75 sm:aspect-w-2 sm:aspect-h-1 sm:h-64 lg:aspect-w-1 lg:aspect-h-1"
                  >
                    <img
                      src="https://i.etsystatic.com/21989441/r/il/e6b2f0/2433671047/il_fullxfull.2433671047_4cmx.jpg"
                      alt="Collection of four insulated travel bottles on wooden shelf."
                      class="h-full w-full object-cover object-center"
                    />
                  </div>
                  <h3 class="mt-6 text-sm text-gray-500">
                    <a href="#">
                      <span class="absolute inset-0"></span>
                      Colombian
                    </a>
                  </h3>
                  <p class="text-base font-semibold text-gray-900">
                    Beans
                  </p>
                </div>
              </div>
            </div>
          </div>
        </section>

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
          <div class="border-t border-gray-200">
            <div class="pt-16 pb-20">
              <div class="md:flex md:justify-center">
                <img
                  src="https://scontent.fruh4-6.fna.fbcdn.net/v/t39.30808-6/243547962_1063021347901551_6553224124569965068_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=TREgUPftLoIAX-_hQ5x&_nc_ht=scontent.fruh4-6.fna&oh=00_AfCzNvdtlqvQAXqyQz8kmTexs9zi312js1_zK3MN3oM7ow&oe=63C091C2"
                  alt="https://scontent.fruh4-6.fna.fbcdn.net/v/t39.30808-6/243547962_1063021347901551_6553224124569965068_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=TREgUPftLoIAX-_hQ5x&_nc_ht=scontent.fruh4-6.fna&oh=00_AfCzNvdtlqvQAXqyQz8kmTexs9zi312js1_zK3MN3oM7ow&oe=63C091C2"
                  class="h-8 w-auto"
                />
              </div>
              <div
                class="mx-auto mt-16 max-w-5xl xl:grid xl:grid-cols-2 xl:gap-8"
              >
                <div class="grid grid-cols-2 gap-8 xl:col-span-2">
                  <div
                    class="space-y-12 md:grid md:grid-cols-2 md:gap-8 md:space-y-0"
                  >
                    <div>
                      <h3 class="text-sm font-medium text-gray-900">
                        Products
                      </h3>
                      <ul role="list" class="mt-6 space-y-6">
                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Bags</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Tees</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Objects</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Home Goods</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Accessories</a
                          >
                        </li>
                      </ul>
                    </div>
                    <div>
                      <h3 class="text-sm font-medium text-gray-900">
                        Customer Service
                      </h3>
                      <ul role="list" class="mt-6 space-y-6">
                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Contact</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Shipping</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Returns</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Warranty</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Secure Payments</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >FAQ</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Find a store</a
                          >
                        </li>
                      </ul>
                    </div>
                  </div>
                  <div
                    class="space-y-12 md:grid md:grid-cols-2 md:gap-8 md:space-y-0"
                  >
                    <div>
                      <h3 class="text-sm font-medium text-gray-900">Company</h3>
                      <ul role="list" class="mt-6 space-y-6">
                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Who we are</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Sustainability</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Press</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Careers</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Terms &amp; Conditions</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Privacy</a
                          >
                        </li>
                      </ul>
                    </div>
                    <div>
                      <h3 class="text-sm font-medium text-gray-900">Legal</h3>
                      <ul role="list" class="mt-6 space-y-6">
                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Terms of Service</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Return Policy</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Privacy Policy</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Shipping Policy</a
                          >
                        </li>
                      </ul>
                    </div>
                  </div>
                </div>
              </div>
            </div>

            <div class="lg:grid lg:grid-cols-2 lg:gap-x-6 xl:gap-x-8">
              <div class="flex items-center rounded-lg bg-gray-100 p-6 sm:p-10">
                <div class="mx-auto max-w-sm">
                  <h3 class="font-semibold text-gray-900">
                    Sign up for our newsletter
                  </h3>
                  <p class="mt-2 text-sm text-gray-500">
                    The latest news, articles, and resources, sent to your inbox
                    weekly.
                  </p>
                  <form class="mt-4 sm:mt-6 sm:flex">
                    <label for="email-address" class="sr-only"
                      >Email address</label
                    >
                    <input
                      id="email-address"
                      type="text"
                      autocomplete="email"
                      required
                      class="w-full min-w-0 appearance-none rounded-md border border-gray-300 bg-white py-2 px-4 text-base text-gray-900 placeholder-gray-500 shadow-sm focus:border-indigo-500 focus:outline-none focus:ring-1 focus:ring-indigo-500"
                    />
                    <div class="mt-3 sm:mt-0 sm:ml-4 sm:flex-shrink-0">
                      <button
                        type="submit"
                        class="flex w-full items-center justify-center rounded-md border border-transparent bg-indigo-600 py-2 px-4 text-base font-medium text-white shadow-sm hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-indigo-500 focus:ring-offset-2 focus:ring-offset-white"
                      >
                        Sign up
                      </button>
                    </div>
                  </form>
                </div>
              </div>

              <div
                class="relative mt-6 flex items-center py-12 px-6 sm:py-16 sm:px-10 lg:mt-0"
              >
                <div class="absolute inset-0 overflow-hidden rounded-lg">
                  <img
                    src="https://tailwindui.com/img/ecommerce-images/footer-02-exclusive-sale.jpg"
                    alt=""
                    class="h-full w-full object-cover object-center saturate-0 filter"
                  />
                  <div
                    class="absolute inset-0 bg-indigo-600 bg-opacity-90"
                  ></div>
                </div>
                <div class="relative mx-auto max-w-sm text-center">
                  <h3 class="text-2xl font-bold tracking-tight text-white">
                    Get early access
                  </h3>
                  <p class="mt-2 text-gray-200">
                    Did you sign up to the newsletter? If so, use the keyword we
                    sent you to get access.
                    <a
                      href="#"
                      class="whitespace-nowrap font-bold text-white hover:text-gray-200"
                      >Go now<span aria-hidden="true"> &rarr;</span></a
                    >
                  </p>
                </div>
              </div>
            </div>
          </div>

          <div class="py-10 md:flex md:items-center md:justify-between">
            <div class="text-center md:text-left">
              <p class="text-sm text-gray-500">
                &copy; 2023 All Rights Reserved Dar Kataket Restaurants Company
                - One Individual Company
              </p>
              <p class="text-sm text-gray-500">Commercial Number: 101074712</p>
              <p class="text-sm text-gray-500">Phone Number: +966540680389</p>
              <p class="text-sm text-gray-500">
                Address: :7936 Haroun Al Rashid Al Jazeerah Dist.3906
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

<script>
export default {}
</script>
