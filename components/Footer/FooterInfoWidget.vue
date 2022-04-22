<template>
    <div class="flex flex-col mr-12 xl:mr-100">
        <!-- Footer Logo Start -->
        <NuxtLink to="/" class="mb-10">
            <img src="/images/technobites.png" alt="Footer Logo">
        </NuxtLink>
        <!-- Footer Logo End -->

        <!-- Text Start -->
        <p> The official site of TECHNOB!TES. Witness the best of folks fighting their way to ace to the pinnacle in various inter college events.</p>
        <!-- Text End -->

        <!-- Social Icon List Start -->
        <ul class="flex mt-4">
            <li v-for="(link, index) in links" :key="index" class="mr-4 last:mr-0">
                <a :href="`${link.href}`" :style="{backgroundImage: `url(${ link.BgShape })`}" class="w-10 h-10 leading-10 text-center inline-block"><i :class="link.className"></i></a>
            </li>
        </ul>
        <!-- Social Icon List End -->
    </div>
</template>

<script>
    export default {
        data() {
            return {
                links: [
                    {
                        href: "https://www.instagram.com/technobites2k22",
                        BgShape: "/images/icon/dribble.webp",
                        className: "icofont-instagram text-white"
                    },
                    {
                        href: "https://www.youtube.com/channel/UCN5RqZWauumdzzytfZZiKeg",
                        BgShape: "/images/icon/youtobe-bg.webp",
                        className: "icofont-youtube-play text-white"
                    }
                    
                ]
            }
        }
    }
</script>