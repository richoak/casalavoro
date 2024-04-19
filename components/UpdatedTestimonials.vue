<template>
    <section class="bg-white dark:bg-gray-900">
        <div class="relative flex">
            <div class="min-h-screen lg:w-1/3"></div>
            <div class="hidden w-3/4 min-h-screen bg-gray-100 dark:bg-gray-800 lg:block"></div>

            <div
                class="container flex flex-col justify-center w-full min-h-screen px-6 py-10 mx-auto lg:absolute lg:inset-x-0">
                <h1 class="text-2xl font-semibold text-gray-800 capitalize lg:text-3xl dark:text-white"
                    data-aos="fade-left" data-aos-delay="100">
                    What our <span class="text-blue-500">customers</span> <br> are saying
                </h1>

                <div class="mt-10 lg:mt-20 lg:flex lg:items-center" v-for="(image, index) in images" :key="index"
                    v-show="index === currentIndex">
                    <img class="object-cover object-center w-full lg:w-[32rem] rounded-lg h-96" :src="image.image" alt="">

                    <div class="mt-8 lg:px-10 lg:mt-0">
                        <h1 class="text-2xl font-semibold text-gray-800 dark:text-white lg:w-72" data-aos="fade-left"
                            data-aos-delay="100">
                            {{ image.title }}
                        </h1>

                        <p class="max-w-lg mt-6 text-gray-500 dark:text-gray-400" data-aos="fade-left"
                            data-aos-delay="100">
                            “{{ image.description }} ”
                        </p>

                        <h3 class="mt-6 text-lg font-medium text-blue-500" data-aos="fade-left" data-aos-delay="100">
                            {{image.name}}</h3>
                        <p class="text-gray-600 dark:text-gray-300" data-aos="fade-left" data-aos-delay="100">{{ image.role }}</p>
                    </div>
                </div>

                <div class="flex items-center justify-between mt-12 lg:justify-start">
                    <button title="left arrow" @click="prevImage"
                        class="p-2 text-gray-800 transition-colors duration-300 border rounded-full rtl:-scale-x-100 dark:border-gray-700 dark:text-gray-200 dark:hover:bg-gray-800 hover:bg-gray-100"
                        data-aos="fade-left" data-aos-delay="100">
                        <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6" fill="none" viewBox="0 0 24 24"
                            stroke="currentColor" stroke-width="2">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M15 19l-7-7 7-7" />
                        </svg>
                    </button>

                    <button title="right arrow" @click="nextImage"
                        class="p-2 text-gray-800 transition-colors duration-300 border rounded-full rtl:-scale-x-100 dark:border-gray-700 dark:text-gray-200 dark:hover:bg-gray-800 lg:mx-6 hover:bg-gray-100"
                        data-aos="fade-left" data-aos-delay="100">
                        <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6" fill="none" viewBox="0 0 24 24"
                            stroke="currentColor" stroke-width="2">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M9 5l7 7-7 7" />
                        </svg>
                    </button>
                </div>
            </div>
        </div>
    </section>
</template>


<script setup lang="ts">
const images = [
    {
        name: 'Ronik Ederson ',
        role: 'Marketing Manager at Stech',
        title: 'Help us improve our productivity',
        description: `Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tempore quibusdam ducimus libero ad tempora doloribus expedita laborum saepe voluptas perferendis delectus assumenda rerum, culpa aperiam dolorum, obcaecati corrupti aspernatur a. `,
        image: 'https://images.unsplash.com/photo-1535713875002-d1d0cf377fde?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=880&q=80',
    },
    {
        name: 'Ronik Ederson sss',
        role: 'Marketing Manager at Stech',
        title: 'Help us improve our productivity',
        description: `Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tempore quibusdam ducimus libero ad tempora doloribus expedita laborum saepe voluptas perferendis delectus assumenda rerum, culpa aperiam dolorum, obcaecati corrupti aspernatur a. `,
        image: 'https://images.unsplash.com/photo-1535713875002-d1d0cf377fde?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=880&q=80',
    },
    {
        name: 'Ronik Ederson ',
        role: 'Marketing Manager at Stech',
        title: 'Help us improve our productivity',
        description: `Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tempore quibusdam ducimus libero ad tempora doloribus expedita laborum saepe voluptas perferendis delectus assumenda rerum, culpa aperiam dolorum, obcaecati corrupti aspernatur a. `,
        image: 'https://images.unsplash.com/photo-1535713875002-d1d0cf377fde?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=880&q=80',
    },
    {
        name: 'Ronik Ederson ',
        role: 'Marketing Manager at Stech',
        title: 'Help us improve our productivity',
        description: `Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tempore quibusdam ducimus libero ad tempora doloribus expedita laborum saepe voluptas perferendis delectus assumenda rerum, culpa aperiam dolorum, obcaecati corrupti aspernatur a. `,
        image: 'https://images.unsplash.com/photo-1535713875002-d1d0cf377fde?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=880&q=80',
    },
    {
        name: 'Ronik Ederson ',
        role: 'Marketing Manager at Stech',
        title: 'Help us improve our productivity',
        description: `Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tempore quibusdam ducimus libero ad tempora doloribus expedita laborum saepe voluptas perferendis delectus assumenda rerum, culpa aperiam dolorum, obcaecati corrupti aspernatur a. `,
        image: 'https://images.unsplash.com/photo-1535713875002-d1d0cf377fde?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=880&q=80',
    }
];

const currentIndex = ref(0);

const beforeEnter = (el) => {
  el.style.transform = 'translateX(100%)';
}

const enter = (el, done) => {
  el.getBoundingClientRect(); // Trigger reflow to put DOM in right state
  el.style.transition = 'transform 0.7s ease-in-out';
  el.style.transform = 'translateX(0)';
  done();
}

const leave = (el, done) => {
  el.style.transition = 'transform 0.7s ease-in-out';
  el.style.transform = 'translateX(-100%)';
  done();
}

function nextImage() {
  currentIndex.value = (currentIndex.value + 1) % images.value.length;
}

function prevImage() {
  currentIndex.value = (currentIndex.value - 1 + images.value.length) % images.value.length;
}
</script>

<style>
.slide-enter-active,
.slide-leave-active {
    transition: transform 0.7s ease-in-out;
}

.slide-enter-from,
.slide-leave-to {
    transform: translateX(100%);
}

.slide-leave-from,
.slide-enter-to {
    transform: translateX(0);
}
</style>