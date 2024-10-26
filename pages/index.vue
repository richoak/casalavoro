<template>
<main>
  <div class="relative isolate overflow-hidden pt-14">
    <img src="@/assets/profile/10.jpg" alt="" class="absolute inset-0 -z-10 h-full w-full object-cover">
    
    <!-- Dark Overlay -->
    <div class="absolute inset-0 bg-black opacity-50 -z-10"></div>
  
    <div class="absolute inset-x-0 -top-40 -z-10 transform-gpu overflow-hidden blur-3xl sm:-top-80" aria-hidden="true">
      <div class="relative left-[calc(50%-11rem)] aspect-[1155/678] w-[36.125rem] -translate-x-1/2 rotate-[30deg] bg-gradient-to-tr from-[#ff80b5] to-[#9089fc] opacity-20 sm:left-[calc(50%-30rem)] sm:w-[72.1875rem]" style="clip-path: polygon(74.1% 44.1%, 100% 61.6%, 97.5% 26.9%, 85.5% 0.1%, 80.7% 2%, 72.5% 32.5%, 60.2% 62.4%, 52.4% 68.1%, 47.5% 58.3%, 45.2% 34.5%, 27.5% 76.7%, 0.1% 64.9%, 17.9% 100%, 27.6% 76.8%, 76.1% 97.7%, 74.1% 44.1%)"></div>
    </div>
    
    <div class="mx-auto max-w-7xl px-6 lg:px-8">
      <div class="mx-auto max-w-2xl py-32 sm:py-48 lg:py-56">
        <div class="text-center">
          <h1 class="text-balance text-5xl font-semibold tracking-tight text-white sm:text-7xl">Build wealth with Casalavoro</h1>
          <p class="mt-8 text-pretty text-lg font-medium text-gray-100 sm:text-xl/8">Finding the safest, reliable, and most profitable real estate opportunities for our clients.</p>
        </div>
      </div>
    </div>
  
    <div class="absolute inset-x-0 top-[calc(100%-13rem)] -z-10 transform-gpu overflow-hidden blur-3xl sm:top-[calc(100%-30rem)]" aria-hidden="true">
      <div class="relative left-[calc(50%+3rem)] aspect-[1155/678] w-[36.125rem] -translate-x-1/2 bg-gradient-to-tr from-[#ff80b5] to-[#9089fc] opacity-20 sm:left-[calc(50%+36rem)] sm:w-[72.1875rem]" style="clip-path: polygon(74.1% 44.1%, 100% 61.6%, 97.5% 26.9%, 85.5% 0.1%, 80.7% 2%, 72.5% 32.5%, 60.2% 62.4%, 52.4% 68.1%, 47.5% 58.3%, 45.2% 34.5%, 27.5% 76.7%, 0.1% 64.9%, 17.9% 100%, 27.6% 76.8%, 76.1% 97.7%, 74.1% 44.1%)"></div>
    </div>
  </div>
  <!-- <div class="bg-gray-900">
    <header class="absolute inset-x-0 top-0 z-50">
      <nav class="flex items-center justify-between p-6 lg:px-8" aria-label="Global">
        <div class="flex lg:flex-1">
          <a href="#" class="-m-1.5 p-1.5">
            <span class="sr-only">Your Company</span>
            <img class="h-8 w-auto" src="@/assets/profile/logo-c-removebg-preview.png" alt="">
          </a>
        </div>
        <div class="flex lg:hidden">
          <button type="button" class="-m-2.5 inline-flex items-center justify-center rounded-md p-2.5 text-gray-400">
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
          <a href="#" class="text-sm font-semibold leading-6 text-white">Contact Us <span aria-hidden="true">&rarr;</span></a>
        </div>
      </nav>
      <div class="lg:hidden" role="dialog" aria-modal="true">
        <div class="fixed inset-0 z-50"></div>
        <div class="fixed inset-y-0 right-0 z-50 w-full overflow-y-auto bg-gray-900 px-6 py-6 sm:max-w-sm sm:ring-1 sm:ring-white/10">
          <div class="flex items-center justify-between">
            <a href="#" class="-m-1.5 p-1.5">
              <span class="sr-only">Your Company</span>
              <img class="h-8 w-auto" src="@/assets/profile/logo-c-removebg-preview.png" alt="">
            </a>
            <button type="button" class="-m-2.5 rounded-md p-2.5 text-gray-400">
              <span class="sr-only">Close menu</span>
              <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true" data-slot="icon">
                <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" />
              </svg>
            </button>
          </div>
          <div class="mt-6 flow-root">
            <div class="-my-6 divide-y divide-gray-500/25">
              <div class="space-y-2 py-6">
                <a href="#" class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-white hover:bg-gray-800">Product</a>
                <a href="#" class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-white hover:bg-gray-800">Features</a>
                <a href="#" class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-white hover:bg-gray-800">Marketplace</a>
                <a href="#" class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-white hover:bg-gray-800">Company</a>
              </div>
              <div class="py-6">
                <a href="#" class="-mx-3 block rounded-lg px-3 py-2.5 text-base font-semibold leading-7 text-white hover:bg-gray-800">Log in</a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </header>
  </div> -->


<div class="overflow-hidden bg-white">
  <div class="relative mx-auto max-w-7xl px-6 py-16 lg:px-8">
    <div class="absolute bottom-0 left-3/4 top-0 hidden w-screen bg-gray-50 lg:block"></div>
    <div class="mx-auto max-w-prose text-base lg:grid lg:max-w-none lg:grid-cols-2 lg:gap-8">
      <div>
        <!-- <h2 class="text-lg font-semibold text-indigo-600">Management Team
        </h2> -->
        <h3 class="mt-2 text-3xl font-bold leading-8 tracking-tight text-gray-900 max-w-xs">
          Statement From The Chief Executive Officer
        </h3>
      </div>
    </div>
    <div class="mt-8 lg:grid lg:grid-cols-2 lg:gap-8">
      <div class="relative lg:col-start-2 lg:row-start-1">
        <svg class="absolute right-0 top-0 -mr-20 -mt-20 hidden lg:block" width="404" height="384" fill="none" viewBox="0 0 404 384" aria-hidden="true">
          <defs>
            <pattern id="de316486-4a29-4312-bdfc-fbce2132a2c1" x="0" y="0" width="20" height="20" patternUnits="userSpaceOnUse">
              <rect x="0" y="0" width="4" height="4" class="text-gray-200" fill="currentColor" />
            </pattern>
          </defs>
          <rect width="404" height="384" fill="url(#de316486-4a29-4312-bdfc-fbce2132a2c1)" />
        </svg>
        <div class="relative mx-auto max-w-prose text-base lg:max-w-none">
          <figure>
            <div class="aspect-h-7 aspect-w-12 lg:aspect-none">
              <img class="rounded-lg object-cover object-center shadow-lg" src="@/assets/profile/lead7.jpeg" alt="Whitney leaning against a railing on a downtown street" width="1184" height="1376">
            </div>
          </figure>
        </div>
      </div>
      <div class="mt-8 lg:mt-0">
        <div class="mx-auto max-w-prose space-y-4 text-base space-y-3 lg:max-w-none">
          <p class="text-lg text-gray-500">Our commitment extends far beyond financial success. As the CEO, Iam honored to lead an organization deeply rooted in unwavering integrity, innovation, and responsible investment practices.</p>
            <p class="text-lg text-gray-500">We pride ourselves on a holistic approach to investment, leveraging astute strategies that foster sustainable growth while prioritizing ethical and socially responsible initiatives. Our mission is to not only deliver exceptional returns to our stakeholders but also to contribute positively to the communities we serve and the world at large.</p>
            <p class="text-lg text-gray-500">We thrive on diversity, leveraging the collective expertise of our team to navigate dynamic market landscapes and identify unique opportunities. Our dedication to cultivating a culture of excellence empowers us to drive impactful change, continuously exploring new avenues for growth and innovation.</p>
            <p class="text-lg text-gray-500">Transparency and accountability are the cornerstones of our operations. We meticulously assess each investment opportunity, ensuring alignment with our values and the potential to generate enduring value for our partners and society.</p>
            <p class="text-lg text-gray-500">As we navigate the ever-evolving global market, our focus remains resolutely on adaptability, resilience, and ethical leadership. We are unwavering in our pursuit of excellence, committed to being at the forefront of responsible investment practices, and dedicated to creating a sustainable, prosperous future for all.</p>
            <p class="text-lg text-gray-500">Thank you for joining us on this journey of responsible investment and positive impact.</p>
         <div>
              <p class="text-lg text-gray-500 font-semibold">Warm regards,</p>
              <p class="text-xl text-gray-900 font-semibold">Williams Olatunbosun</p>
              <!-- <div>
                <video width="600" controls>
                  <source src="/1.mp4" type="video/mp4" />
                  Your browser does not support the video tag.
                </video>
              </div> -->
         </div>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="relative isolate bg-gray-900">
  <div class="mx-auto grid max-w-7xl grid-cols-1 lg:grid-cols-2">
    <div class="relative px-6 pb-20 pt-24 sm:pt-32 lg:static lg:px-8 lg:py-48">
      <div class="mx-auto max-w-xl lg:mx-0 lg:max-w-lg">
        <div class="absolute inset-y-0 left-0 -z-10 w-full overflow-hidden ring-1 ring-white/5 lg:w-1/2">
          <svg class="absolute inset-0 h-full w-full stroke-gray-700 [mask-image:radial-gradient(100%_100%_at_top_right,white,transparent)]" aria-hidden="true">
            <defs>
              <pattern id="54f88622-e7f8-4f1d-aaf9-c2f5e46dd1f2" width="200" height="200" x="100%" y="-1" patternUnits="userSpaceOnUse">
                <path d="M130 200V.5M.5 .5H200" fill="none" />
              </pattern>
            </defs>
            <svg x="100%" y="-1" class="overflow-visible fill-gray-800/20">
              <path d="M-470.5 0h201v201h-201Z" stroke-width="0" />
            </svg>
            <rect width="100%" height="100%" stroke-width="0" fill="url(#54f88622-e7f8-4f1d-aaf9-c2f5e46dd1f2)" />
          </svg>
          <div class="absolute -left-56 top-[calc(100%-13rem)] transform-gpu blur-3xl lg:left-[max(-14rem,calc(100%-59rem))] lg:top-[calc(50%-7rem)]" aria-hidden="true">
            <div class="aspect-[1155/678] w-[72.1875rem] bg-gradient-to-br from-[#80caff] to-[#4f46e5] opacity-20" style="clip-path: polygon(74.1% 56.1%, 100% 38.6%, 97.5% 73.3%, 85.5% 100%, 80.7% 98.2%, 72.5% 67.7%, 60.2% 37.8%, 52.4% 32.2%, 47.5% 41.9%, 45.2% 65.8%, 27.5% 23.5%, 0.1% 35.4%, 17.9% 0.1%, 27.6% 23.5%, 76.1% 2.6%, 74.1% 56.1%)"></div>
          </div>
        </div>
        <h2 class="text-pretty text-4xl font-semibold tracking-tight text-white sm:text-5xl">Get in touch</h2>
        <!-- <p class="mt-6 text-lg leading-8 text-gray-300">Proin volutpat consequat porttitor cras nullam gravida at. Orci molestie a eu arcu. Sed ut tincidunt integer elementum id sem. Arcu sed malesuada et magna.</p> -->
        <dl class="mt-10 space-y-4 text-base leading-7 text-gray-300">
          <div class="flex gap-x-4">
            <dt class="flex-none">
              <span class="sr-only">Address</span>
              <svg class="h-7 w-6 text-gray-400" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true" data-slot="icon">
                <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 21h19.5m-18-18v18m10.5-18v18m6-13.5V21M6.75 6.75h.75m-.75 3h.75m-.75 3h.75m3-6h.75m-.75 3h.75m-.75 3h.75M6.75 21v-3.375c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125V21M3 3h12m-.75 4.5H21m-3.75 3.75h.008v.008h-.008v-.008Zm0 3h.008v.008h-.008v-.008Zm0 3h.008v.008h-.008v-.008Z" />
              </svg>
            </dt>
            <dd>NO_29, Kigoma Street, Wuse, Zone 7 Abuja.</dd>
          </div>
          <div class="flex gap-x-4">
            <dt class="flex-none">
              <span class="sr-only">Telephone</span>
              <svg class="h-7 w-6 text-gray-400" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true" data-slot="icon">
                <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 6.75c0 8.284 6.716 15 15 15h2.25a2.25 2.25 0 0 0 2.25-2.25v-1.372c0-.516-.351-.966-.852-1.091l-4.423-1.106c-.44-.11-.902.055-1.173.417l-.97 1.293c-.282.376-.769.542-1.21.38a12.035 12.035 0 0 1-7.143-7.143c-.162-.441.004-.928.38-1.21l1.293-.97c.363-.271.527-.734.417-1.173L6.963 3.102a1.125 1.125 0 0 0-1.091-.852H4.5A2.25 2.25 0 0 0 2.25 4.5v2.25Z" />
              </svg>
            </dt>
            <dd><a class="hover:text-white" href="tel:+234 9016854815">+234 9016854815</a></dd>
          </div>
          <div class="flex gap-x-4">
            <dt class="flex-none">
              <span class="sr-only">Email</span>
              <svg class="h-7 w-6 text-gray-400" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true" data-slot="icon">
                <path stroke-linecap="round" stroke-linejoin="round" d="M21.75 6.75v10.5a2.25 2.25 0 0 1-2.25 2.25h-15a2.25 2.25 0 0 1-2.25-2.25V6.75m19.5 0A2.25 2.25 0 0 0 19.5 4.5h-15a2.25 2.25 0 0 0-2.25 2.25m19.5 0v.243a2.25 2.25 0 0 1-1.07 1.916l-7.5 4.615a2.25 2.25 0 0 1-2.36 0L3.32 8.91a2.25 2.25 0 0 1-1.07-1.916V6.75" />
              </svg>
            </dt>
            <dd><a class="hover:text-white" href="mailto:hello@example.com">casalavorolimited@gmail.com</a></dd>
          </div>
        </dl>
      </div>
    </div>
    <form action="#" method="POST" class="px-6 pb-24 pt-20 sm:pb-32 lg:px-8 lg:py-48">
      <div class="mx-auto max-w-xl lg:mr-0 lg:max-w-lg">
        <div class="grid grid-cols-1 gap-x-8 gap-y-6 sm:grid-cols-2">
          <div>
            <label for="first-name" class="block text-sm font-semibold leading-6 text-white">First name</label>
            <div class="mt-2.5">
              <input type="text" name="first-name" id="first-name" autocomplete="given-name" class="block w-full rounded-md border-0 bg-white/5 px-3.5 py-2 text-white shadow-sm ring-1 ring-inset ring-white/10 focus:ring-2 focus:ring-inset focus:ring-indigo-500 sm:text-sm sm:leading-6">
            </div>
          </div>
          <div>
            <label for="last-name" class="block text-sm font-semibold leading-6 text-white">Last name</label>
            <div class="mt-2.5">
              <input type="text" name="last-name" id="last-name" autocomplete="family-name" class="block w-full rounded-md border-0 bg-white/5 px-3.5 py-2 text-white shadow-sm ring-1 ring-inset ring-white/10 focus:ring-2 focus:ring-inset focus:ring-indigo-500 sm:text-sm sm:leading-6">
            </div>
          </div>
          <div class="sm:col-span-2">
            <label for="email" class="block text-sm font-semibold leading-6 text-white">Email</label>
            <div class="mt-2.5">
              <input type="email" name="email" id="email" autocomplete="email" class="block w-full rounded-md border-0 bg-white/5 px-3.5 py-2 text-white shadow-sm ring-1 ring-inset ring-white/10 focus:ring-2 focus:ring-inset focus:ring-indigo-500 sm:text-sm sm:leading-6">
            </div>
          </div>
          <div class="sm:col-span-2">
            <label for="phone-number" class="block text-sm font-semibold leading-6 text-white">Phone number</label>
            <div class="mt-2.5">
              <input type="tel" name="phone-number" id="phone-number" autocomplete="tel" class="block w-full rounded-md border-0 bg-white/5 px-3.5 py-2 text-white shadow-sm ring-1 ring-inset ring-white/10 focus:ring-2 focus:ring-inset focus:ring-indigo-500 sm:text-sm sm:leading-6">
            </div>
          </div>
          <div class="sm:col-span-2">
            <label for="message" class="block text-sm font-semibold leading-6 text-white">Message</label>
            <div class="mt-2.5">
              <textarea name="message" id="message" rows="4" class="block w-full rounded-md border-0 bg-white/5 px-3.5 py-2 text-white shadow-sm ring-1 ring-inset ring-white/10 focus:ring-2 focus:ring-inset focus:ring-indigo-500 sm:text-sm sm:leading-6"></textarea>
            </div>
          </div>
        </div>
        <div class="mt-8 flex justify-end">
          <button type="submit" class="rounded-md bg-indigo-500 px-3.5 py-2.5 text-center text-sm font-semibold text-white shadow-sm hover:bg-indigo-400 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-500">Send message</button>
        </div>
      </div>
    </form>
  </div>
</div>
</main>
</template>
