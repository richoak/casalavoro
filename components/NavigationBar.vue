<template>
  <main class="bg-black w-full h-20">
      <div class="bg-black">
          <header class="relative z-50">
            <nav class="flex items-center justify-between p-6 lg:px-8" aria-label="Global">
              <div class="flex lg:flex-1">
                <a href="#" class="-m-1.5 p-1.5">
                  <span class="sr-only">Your Company</span>
                  <img class="h-8 w-auto" src="@/assets/profile/logo-c-removebg-preview.png" alt="">
                </a>
              </div>
              <div class="flex lg:hidden z-50">
                <button @click="openSide" type="button" class="-m-2.5 z-50 inline-flex items-center justify-center rounded-md p-2.5 text-gray-400">
                  <span class="sr-only">Open main menu</span>
                  <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true" data-slot="icon">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
                  </svg>
                </button>
              </div>
              <div class="hidden lg:flex lg:gap-x-12">
                <NuxtLink to="/" class="text-sm font-semibold leading-6 text-white">Home</NuxtLink>
                <NuxtLink to="/about" class="text-sm font-semibold leading-6 text-white">About</NuxtLink>
                <NuxtLink to="/projects" class="text-sm font-semibold leading-6 text-white">Projects</NuxtLink>
                <NuxtLink to="/teams" class="text-sm font-semibold leading-6 text-white">Teams</NuxtLink>
              </div>
              <div class="hidden lg:flex lg:flex-1 lg:justify-end">
                <a href="https://casalavororesidence.com/" class="text-sm font-semibold leading-6 text-white">Casalavoro Residence <span aria-hidden="true">&rarr;</span></a>
              </div>
            </nav>
            
            <!-- Sidebar Menu -->
            <div v-if="isOpen" class="fixed inset-0 z-50 bg-gray-900 bg-opacity-75" role="dialog" aria-modal="true">
              <div class="fixed inset-y-0 right-0 z-50 w-full overflow-y-auto bg-gray-900 px-6 py-6 sm:max-w-sm sm:ring-1 sm:ring-white/10">
                <div class="flex items-center justify-between">
                  <a href="#" class="-m-1.5 p-1.5">
                    <span class="sr-only">Your Company</span>
                    <img class="h-8 w-auto" src="@/assets/profile/logo-c-removebg-preview.png" alt="">
                  </a>
                  <button @click="closeSide" type="button" class="-m-2.5 rounded-md p-2.5 text-gray-400 z-50">
                    <span class="sr-only">Close menu</span>
                    <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true" data-slot="icon">
                      <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
                    </svg>
                  </button>
                </div>
                <div class="mt-6 flow-root">
                  <div class="-my-6 divide-y divide-gray-500/25">
                    <div class="space-y-2 py-6">
                      <NuxtLink @click="isOpen = false" to="/" class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-white hover:bg-gray-800">Home</NuxtLink>
                      <NuxtLink @click="isOpen = false" to="/about" class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-white hover:bg-gray-800">About</NuxtLink>
                      <NuxtLink @click="isOpen = false" to="/projects" class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-white hover:bg-gray-800">Projects</NuxtLink>
                      <NuxtLink @click="isOpen = false" to="/teams" class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-white hover:bg-gray-800">Team</NuxtLink>
                    </div>
                    <div class="py-6">
                      <a href="https://casalavororesidence.com/" class="-mx-3 block rounded-lg px-3 py-2.5 text-base font-semibold leading-7 text-white hover:bg-gray-800">Casalavoro Residence <span aria-hidden="true">&rarr;</span></a>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </header>
        </div>
  </main>
</template>

<script setup lang="ts">
const isOpen = ref(false)

const openSide = () => {
isOpen.value = true
}

const closeSide = () => {
isOpen.value = false
}
</script>
