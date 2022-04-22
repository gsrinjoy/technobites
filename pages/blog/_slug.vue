<template>
  <div class="bg-cover bg-gray-800" style="background-image:url(/images/bg/body-bg2.webp);">
    
    <HeaderSection/>

    <OffCanvasMobileMenu :class="{'show-mobile-menu' : navOpen}" @togglenav="navOpen = !navOpen" />
    
    <Breadcrumb :BreadcrumbTitle="BreadcrumbTitle" :BreadcrumbSubTitle="BreadcrumbSubTitle"/>

    <div class="details">
        <div class="container">
            <div class="grid mb-20">
                <div class="single-grid">
                    <div class="post-top-area max-w-4xl m-auto text-center mb-16">
                        <ul class="flex mb-8 justify-center text-white">
                            <li class="relative pr-8 content-after after:bg-primary after:absolute after:top-3 after:right-4 after:w-1 after:h-1 after:rounded-full">
                                By <span>Laxi Mehta</span>
                            </li>
                            <li class="relative pr-8 content-after after:bg-primary after:absolute after:top-3 after:right-4 after:w-1 after:h-1 after:rounded-full">
                                <span>{{blogData.date}}</span>
                            </li>
                            <li class="">
                                <span>5 min read</span>
                            </li>
                        </ul>
                        <h2 class="text-white font-bold uppercase xl:text-title lg:text-5xl md:text-4xl sm:text-3xl text-2xl xl:leading-70 lg:leading-12 leading-10">{{blogData.title}}</h2>
                    </div>
                    <div class="post-tags my-8 space-x-3 text-white text-center">
                        <n-link to="/" class="px-4 py-2 border-secondary-80 bg-secondary-100 hover:bg-primary hover:border-primary transition-all border-2 border-solid inline-block rounded-md"> Tech Event</n-link>
                        <n-link to="/" class="px-4 py-2 border-secondary-80 bg-secondary-100 hover:bg-primary hover:border-primary transition-all border-2 border-solid inline-block rounded-md"> Technobites</n-link>
                    </div>
                    <div class="text-center">
                        <!-- <img :src="blogData.imgLarge" alt=""> -->
                    </div>
                    <div class="content max-w-4xl m-auto mt-20">                    
                        <div class="description">“Tell me, and I forget, teach me, and I may remember, involve me, and learn.” 
-Benjamin Franklin

                            <h4 class="text-white xl:text-2xl lg:text-xl md:text-2xl sm:text-lg font-bold uppercase transition-all mb-2 sm:mb-5 leading-9"></h4>
                            <p class="leading-8">These words of wisdom are tailored to the student's college experience. The vibrant college life would not be complete without fests, an important part of a student’s life. It leaves an indelible mark on the academic calendar and students look forward to the date.</p> 
                            <p class="leading-8">It's no secret that employers love to hire candidates who have knowledge and expertise in their field and know how to communicate and interact with clients. Your CV speaks volumes about your talents if you've actively participated in college parties, cultural activities, sports tournaments or anything outside of the classroom. If you participate in certain activities, it reflects your talent and potential. Employers are looking for candidates who can think clearly and have effective communication skills. People who can multi-task, take initiative, and are enterprising have a higher chance of being employed. Students develop in many ways if they actively participate in university parties.</p>
                            <p class="leading-8">College fest should be an essential part of the course curriculum as it provides a platform for young brains to showcase their innovative ideas and compete with their peers. These fests are a combination of fun and learning, where spectacular ideas are presented, and students learn and feel inspired. These events inspire students to aim higher and achieve their goals.</p>
                            <p class="leading-8">Fests provide students with a platform to showcase their unique talents and are crucial in the holistic development of their personalities, helping to break free from the monotonous academic and evaluation routines. There are internal and external parties that engage students, and their learning varies from their advanced networking skills to understanding the nuances of managing finances and maintaining a good reputation. language of the university at each stage. It is the most effective way to bring young people together on one platform, stimulating social interaction and exchanging a variety of ideas and concepts.</p>
                            <p class="leading-8">The role of college fests is of primary importance and, according to a growing consensus among universities, they have become a tool for learning alongside recreation. The dedication practitioners show during the fest days can drain their energy, but it gives them a sense of satisfaction and replenishes them with enthusiasm and of course important learning. that they will cherish for the rest of their lives.</p>
                            <p class="leading-8">Fests provide students with a platform to showcase their unique talents and are important in the development of an all-around personality that breaks free from monotonous academic and assessment routines. There are internal and external parties that engage students, and their learning varies from their advanced networking skills to understanding the nuances of how to manage finances and how to maintain a reputation language of the university at each stage. It is the most effective way to bring young people together on one platform, stimulating social interaction and exchanging a variety of ideas and concepts.</p>
                            <!-- <img class="rounded-3xl" src="/images/blog/blog_details_layer.webp" alt="">
                            <blockquote class="py-5 mb-5"><p class="font-bold text-yellow italic lg:text-3xl text-xl">Lorem Ipsum is simply dummy text of the printing and typesetting industry has been the industry's standard dummy text ever since the 1500 printer took galley of type scrambled it to make a type specimen book.</p></blockquote>
                            <h4 class="text-white xl:text-2xl lg:text-xl md:text-2xl sm:text-lg font-bold uppercase transition-all mb-2 sm:mb-5 leading-9 mt-10">Our company fails the real world test in all kinds of ways.</h4>
                            <p class="leading-8">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500 when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap electro typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p> -->

                            <div class="social-share-wrap items-center mt-14 py-6 border-b-2 border-t-2 border-secondary-80 flex flex-col sm:flex-row justify-between">
                                <h3 class="share font-bold text-2xl uppercase">Share This Article:</h3>
                                <ul class="post-social-list space-x-2 mt-5 sm:mt-0">
                                    <li class="inline-block">
                                        <a class="px-3 py-2 border-secondary-80 bg-secondary-100 hover:bg-primary hover:border-primary transition-all border-2 border-solid rounded-md" href="https://www.facebook.com"><i class="icofont-facebook"></i></a>
                                    </li>
                                    <li class="inline-block">
                                        <a class="px-3 py-2 border-secondary-80 bg-secondary-100 hover:bg-primary hover:border-primary transition-all border-2 border-solid rounded-md" href="https://www.twitter.com"><i class="icofont-twitter"></i></a>
                                    </li>
                                    <li class="inline-block">
                                        <a class="px-3 py-2 border-secondary-80 bg-secondary-100 hover:bg-primary hover:border-primary transition-all border-2 border-solid rounded-md" href="https://www.instagram.com"><i class="icofont-instagram"></i></a>
                                    </li>
                                </ul>
                            </div>

                        </div>
                    </div>
                </div>
            </div>

            <BlogListinDetails />

            <Disqus class="mt-20" shortname='Admin' />

        </div>
    </div>

    <ContactBanner :paddingTop="paddingTop"/>

    <Footer/>

  </div>
</template>

<script>
import blogData from '@/data/blog.json'
import { Disqus } from 'vue-disqus'
export default {
    props: ["match"],
    components: {
        HeaderSection: () => import('@/components/HeaderSection'),
        OffCanvasMobileMenu: () => import('@/components/Header/OffCanvasMobileMenu'),
        Breadcrumb: () => import('@/components/Breadcrumb'),
        BlogListinDetails: () => import('@/components/Blog/BlogListinDetails'),
        ContactBanner: () => import('@/components/ContactBanner'),
        Footer: () => import('@/components/Footer'),
        Disqus
    },
    data() {
        return {
                blogData,
                slug: this.$route.params.slug,
                navOpen: false,
                BreadcrumbTitle: "BLOG",
                BreadcrumbSubTitle: "BLOG",
                paddingTop: "pt-32"
        }
    },
    mounted () {
        this.blogData = blogData.find(blog => blog.slug == this.$route.params.slug);
    }
}
</script>