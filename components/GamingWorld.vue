<template>
    <!-- Gaming World Section Start -->
    <div class="lg:mb-32 md:mb-20 mb-15">
        <div class="container">
            <TitleSection :title="title"/>
        </div>
        <div class="container grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-10">
            <div class="text-white text-center align-cener bg-no-repeat bg-scroll bg-center bg-cover md:pt-14 md:pb-12 md:px-12 sm:py-14 sm:px-6 py-14 px-10 h-460" :style="{backgroundImage: `url(${ service.videoBannerBg })`}" v-for="(service, index) in services" :key="index">
                <div class="mb-12 text-center align-center">
                    <img class="h-37 w-36" :src="service.imgSrc" :alt="service.name">
                </div>
                <div class="block">
                    <h3 class="text-white font-exo text-xl md:text-2xl font-bold uppercase mb-4">{{service.live}}</h3>
                    <p class="">{{service.text}}</p>
                </div>
            </div>
        </div>
    </div>
    <!-- Gaming World Section End -->
</template>

<script>
    export default {
        components: {
            TitleSection: () => import('@/components/Title/TitleSection'),
        },
        data() {
            return {
                title:"Witness the best of events",
                services: [
                    {
                        imgSrc: "/images/others/gaming-world1.webp",
                        name: "Service Image",
                        live: "Technob!Tes",
                        text: "When unknown printer took type and scrambled it to make type specimen book centuries,",
                        videoBannerBg: "/images/others/gaming-world-bg1.webp"
                    },
                    {
                        imgSrc: "/images/others/gaming-world2.webp",
                        name: "Service Image",
                        live: "Glitch",
                        text: "Are you a keyboard warrior? Do you have superior tactics? Do you have what it takes to annihilate your enemies? Pause! this is the event for you!",
                        videoBannerBg: "/images/others/gaming-world-bg2.webp"
                    },
                    {
                        imgSrc: "/images/others/gaming-world3.webp",
                        name: "Service Image",
                        live: "Newly Minted",
                        text: "When unknown printer took type and scrambled it to make type specimen book centuries,",
                        videoBannerBg: "/images/others/gaming-world-bg3.webp"
                    },
                     {
                        imgSrc: "/images/others/gaming-world1.webp",
                        name: "Service Image",
                        live: "Steezy groove",
                        text: "We invite vibrant, lively and dynamic youngsters to spread their energy on stage. So, dancers who have the spirit of engaging the audience are welcomed.",
                        videoBannerBg: "/images/others/gaming-world-bg1.webp"
                    },
                    {
                        imgSrc: "/images/others/gaming-world2.webp",
                        name: "Service Image",
                        live: "Sarangi",
                        text: "Get ready to unveil the singer in you as a Music Mystic to showcase your talent and creativity as you immerse yourself into the world of raags and taals.",
                        videoBannerBg: "/images/others/gaming-world-bg2.webp"
                    },
                    {
                        imgSrc: "/images/others/gaming-world3.webp",
                        name: "Service Image",
                        live: "Blinkz",
                        text: "Here we are to rescue your quirky outfits from the shackles of your closet. Gather up your aesthetic sense, creativity, and enthusiasm and instil a euphonious vogue.",
                        videoBannerBg: "/images/others/gaming-world-bg3.webp"
                    },
                ]
            }
        },
    }
</script>