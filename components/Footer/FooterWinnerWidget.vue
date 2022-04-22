<template>
    <div class=" mr-8">
        <FooterWidgetTitle :title="title"/>

        <div class="grid grid-cols-3 sm:grid-cols-3 gap-3">
            <n-link v-for="(match, index) in matches" :key="index" to="/">
                <img :src="`${match.gamingBg}`" :alt="match.gamingAlt">
            </n-link>
        </div>
    </div>
</template>
<script>
export default {
    components:{
        FooterWidgetTitle: () => import('@/components/Footer/FooterWidgetTitle'),
    },
    data () {
        return {
            title: "Sponsors",
            matches: [
                {
                    gamingBg: "/images/others/makemeglobal.png",
                    gamingAlt: "Makemeglobal"
                },
                // {
                //    gamingBg: "/images/others/makemeglobal-logo.png",
                //     gamingAlt: "Makemeglobal"
                // },
                // {
                //    gamingBg: "/images/others/makemeglobal-logo.png",
                //     gamingAlt: "Makemeglobal"
                // },
                // {
                //    gamingBg: "/images/others/makemeglobal-logo.png",
                //     gamingAlt: "Makemeglobal"
                // },
                // {
                //     gamingBg: "/images/others/makemeglobal-logo.png",
                //     gamingAlt: "Makemeglobal"
                // },
                // {
                //     gamingBg: "/images/others/makemeglobal-logo.png",
                //     gamingAlt: "Makemeglobal"
                // }
            ]
        }
    },
}
</script>