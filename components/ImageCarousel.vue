<!-- <template>
    <div class="relative overflow-hidden w-full h-[500px]">
        <div class="flex animate-scroll">
          <div class="flex-none w-full" v-for="(image, index) in allImages" :key="index">
            <img :src="image" alt="Carousel image" class="w-full h-[500px] object-cover">
          </div>
        </div>
      </div>
</template>

<script setup lang="ts">
import carousel1 from '@/assets/img/hero1.jpg'
import carousel2 from '@/assets/img/hero2.jpg'
import carousel3 from '@/assets/img/hero3.jpg'
import carousel4 from '@/assets/img/hero4.jpg'
import carousel5 from '@/assets/img/hero5.jpg'
const images = ref([
  carousel1, carousel2, carousel3, carousel4, carousel5
]);

const allImages = computed(() => [...images.value, ...images.value]);
</script>

<style scoped>
@keyframes scroll {
  0% {
    transform: translateX(0);
  }

  100% {
    transform: translateX(-50%);
  }
}

.animate-scroll {
  width: calc(200% - 0.5rem);
  /* Adjust based on your actual needs */
  display: flex;
  animation: scroll 10s linear infinite;
}
</style> -->

<!-- <template>
    <main>
        <h1></h1>
        <div class="carousel-container relative overflow-hidden w-full h-64" ref="carousel">
            <div class="carousel-track flex" :style="{ 'animation-duration': scrollSpeed + 's' }">
                <div class="flex-none border-2 border-red-500 h-[500px] w-full" v-for="(image, index) in allImages"
                    :key="index">
                    <img :src="image" alt="Carousel image" class="w-full h-[500px] object-cover">
                </div>
            </div>
        </div>
    </main>
</template>

<script lang="ts" setup>
import carousel1 from '@/assets/img/business1.jpeg'
import carousel2 from '@/assets/img/business2.jpeg'
import carousel3 from '@/assets/img/business3.jpeg'
import carousel4 from '@/assets/img/business4.jpeg'
import carousel5 from '@/assets/img/business5.jpeg'
const images = ref([
    carousel1, carousel2, carousel3, carousel4, carousel5
]);


const allImages = computed(() => [...images.value, ...images.value]);

const scrollSpeed = 10;
const carousel = ref<HTMLElement | null>(null);

const startScroll = (element: HTMLElement, speed: number) => {
    const totalWidth = element.clientWidth / 2;
    let currentPosition = 0;

    const step = () => {
        currentPosition += 1;
        if (currentPosition >= totalWidth) {
            currentPosition = 0;
        }
        element.scrollTo(currentPosition, 0);
    };

    const intervalId = setInterval(step, speed * 10);

    return () => clearInterval(intervalId);
};

let stopScroll: (() => void) | undefined;

onMounted(() => {
    if (carousel.value) {
        stopScroll = startScroll(carousel.value, scrollSpeed);
    }
});

onUnmounted(() => {
    if (stopScroll) {
        stopScroll();
    }
});
</script>

<style scoped>
.carousel-container {
    width: 100%;
    overflow: hidden;
}

.carousel-track {
    will-change: transform;
    display: flex;
    animation: scroll linear infinite;
}

@keyframes scroll {
    0% {
        transform: translateX(0);
    }

    100% {
        transform: translateX(-50%);
    }
}
</style> -->

<template>
    <main class="bg-white dark:bg-gray-900">
        <section class="container px-6 py-10 mx-auto space-y-10">
            <div class="text-center">
                <h1 class="text-2xl font-semibold text-gray-800 capitalize lg:text-3xl dark:text-white"
                    data-aos="flip-left">Innovation in Action</h1>

                <p class="max-w-lg mx-auto mt-4 text-gray-500" data-aos="flip-left">
                    Browse our portfolio to see how we've transformed challenges into technological triumphs. Each
                    project is a testament to our innovative solutions and strategic foresight, driving real results
                    across industries.
                </p>
            </div>

            <div class="carousel-container overflow-hidden relative">
                <div class="carousel-track flex gap-x-5" :style="{ transform: `translateX(-${offset}px)` }">
                    <div class="image-item flex-none w-full" v-for="(image, index) in allImages" :key="index">
                        <img :src="image" class="h-full w-full object-cover object-center" alt="">
                    </div>
                </div>
            </div>
        </section>
    </main>
</template>

<script lang="ts">
import carousel1 from '@/assets/img/business1.png'
import carousel2 from '@/assets/img/business2.png'
import carousel3 from '@/assets/img/business3.png'
import carousel4 from '@/assets/img/business4.png'
import carousel5 from '@/assets/img/business5.png'
export default defineComponent({
    name: 'ContinuousCarousel',
    setup() {
        const images = ref([
            carousel1, carousel2, carousel3, carousel4, carousel5
        ]);

        // Duplicate the images to simulate infinite loop
        const allImages = ref([...images.value, ...images.value]);

        const offset = ref(0);
        const itemWidth = 300; // width of each image
        const scrollSpeed = 2; // speed in pixels

        let interval: number | undefined;

        function startScrolling() {
            interval = window.setInterval(() => {
                if (offset.value >= itemWidth * images.value.length) {
                    offset.value = 0; // Reset to start when end is reached
                } else {
                    offset.value += scrollSpeed;
                }
            }, 20);
        }

        onMounted(() => {
            startScrolling();
        });

        onUnmounted(() => {
            if (interval) {
                clearInterval(interval);
            }
        });

        return { allImages, offset };
    }
});
</script>

<style scoped>
.carousel-container {
    width: 100%;
    height: 500px;
    /* Adjust as needed */
}

.carousel-track {
    will-change: transform;
    min-width: max-content;
}

.image-item {
    width: 300px;
    /* Ensure this matches `itemWidth` in script */
    flex-shrink: 0;
}
</style>