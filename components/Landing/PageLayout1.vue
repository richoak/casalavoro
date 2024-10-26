<template>
    <div class="min-h-screen bg-gray-100">
      <section class="flex flex-wrap">
        <!-- Left section with large image and overlay text -->
        <div class="w-full md:w-1/2 relative bg-cover bg-center" style="background-image: url('/path-to-image.jpg')">
          <div class="absolute bottom-0 bg-black text-white p-6 w-full text-center">
            <h2 class="text-xl font-bold">A TRACK RECORD OF OUR REAL ESTATE PROJECTS</h2>
          </div>
        </div>
  
        <!-- Right section with project images and descriptions -->
        <div class="w-full md:w-1/2 p-6 bg-white">
          <h2 class="text-lg font-bold mb-4">CASALAVORO HOMES</h2>
  
          <!-- Project 1 -->
          <div class="mb-8">
            <img src="/path-to-project-image1.jpg" alt="Oak Grandeur I" class="w-full h-auto mb-4" />
            <h3 class="font-bold">OAK GRANDEUR I <span class="text-red-500">(SOLD OUT)</span></h3>
            <p>
              Oak-Grandeur I is a residential, luxurious, modern, state-of-the-art, tastefully finished six units of three-bedroom edifice, located in the heart of Abuja.
            </p>
          </div>
  
          <!-- Project 2 -->
          <div>
            <img src="/path-to-project-image2.jpg" alt="Oak Grandeur II" class="w-full h-auto mb-4" />
            <h3 class="font-bold">OAK GRANDEUR II <span class="text-red-500">(SOLD OUT)</span></h3>
            <p>
              Oak-Grandeur II is an exclusive, beautiful apartment built on 650sqm of land in the secure area of Jahi-Abuja.
            </p>
          </div>
        </div>
      </section>
    </div>
  </template>
  
  <script setup lang="ts">
  // Import any necessary functions, if needed
  </script>
  
  <style scoped>
  /* Any specific styles for layout refinements */
  </style>
  