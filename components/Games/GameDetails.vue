<template>
    <div class="container relative">
        
        <!-- <h2 class="date text-primary font-bold mb-2">Venue: Blob Studio (Blob Turf), Yamuna Tower 8th Floor, Near Sreebhumi, Kolkata - 48</h2> -->
        <h2 class="text-white font-bold uppercase xl:text-title lg:text-5xl md:text-4xl sm:text-3xl text-2xl xl:leading-70 lg:leading-12 leading-10">{{games.title}}</h2>
                    <div class="gameslide my-15">

                <swiper class="swiper" :options="swiperOption">
                    <swiper-slide v-for="(game, imageIndex) in gameslide" :key="imageIndex">
                        <div class="relative">
                            <img class="sm:h-full h-64 w-full object-cover" :src="`${game.gamingBg}`">
                        </div>
                    </swiper-slide>
                </swiper>

                <!-- Testimonial Arrows -->

                <div class="flex mt-10">
                    <div class="gameslide-button-prev swipper-arrow text-white md:w-68 w-55 md:h-55 h-11 bg-cover flex items-center justify-center hover:bg-arrow-hover-shape bg-arrow-shape transition-all z-50 mr-2">
                        <img class="w-4 h-6" src="/images/icon/navigation-arrow2.webp" alt="">
                    </div>
                    <div class="gameslide-button-next swipper-arrow text-white md:w-68 w-55 md:h-55 h-11 flex items-center justify-center hover:bg-arrow-hover-shape bg-arrow-shape bg-cover transition-all z-50 ml-2">
                        <img class="w-4 h-6" src="/images/icon/navigation-arrow1.webp" alt="">
                    </div>
                </div>
            </div>
        <div class="content-details">
            <div class="description mt-6">
                <h2 class="date text-primary font-bold mb-2 ">Esports</h2>
                <h2 class="text-white font-bold uppercase xl:text-title lg:text-5l md:text-4l sm:text-3l text-2l l:leading-70 lg:leading-12 leading-10">FIFA</h2>
                
                <p class="leading-8">Registration will be done online through google forms.
                Registration is First Come First Serve. (No of playersis Limited)
                It is a multiple round knockout event (1 VS 1).
                The firstround will be played by all the registered users.
                The winner of every round progressesto the next knockoutround.
                Opponents will be chosen randomly.
                At any point in the tournament the organizer/coordinator hasthe right to dismissthe match
                and disqualify a playerin case of fraud detected.

                A match will last for 10 minutes(5 min half) for all the knockoutrounds, except the SEMI-
                FINALS and FINALS where the match length will be 12 minutes(6 min half).

                A coin toss will take place priorto every match. On the basis of the coin toss, the LOSER getsto
                choose whetherthe match will be an International clash or a Club fixture. The WINNER selects
                the team he/she will play with first.
                The GAME DIFFICULTY and the GOALKEEPER level will be set to 'World Class' forthe whole of
                the tournament.
                If the winneris not decided in normal time (10 min and 12 min in case ofsemi's and finals), then
                only the first half of 4 min a half match will be played if the winneris not decided by that, the
                second half will be played of that 4 min half match with the golden goalrule if the winneris not
                decided afterthat a coin toss will take place.
                Ifrequired players can bring their own headsets.
                Participants will be given 2 mins before every match to configure their controls according to
                their needs.
                Participants who do not arrive in time will be disqualified forthe nextround.
                ONLY the participants will be allowed inside the competition area. NO other person will be
                allowed to enterthe area.
                1.</p>
                <br/>
                <h2 class='date text-primary font-bold mb-2'>Registration Process</h2>
                <p class="leading-8">
                    ○ Participants must fill the form providing all necessary details.<br/>
                    ○ Deadline forregistration is 10th May, 10pm.<br/>
                    ○ Registration charges are Rs. <b>100 persquad</b>.<br/>
                    ○ For Registration <a href="https://technobites.bio.link/" target="blank"><b><i>Click here</i></b></a><br/>
                </p>
            </div>

            <div class="description mt-6">
                <h2 class="text-white font-bold uppercase xl:text-title lg:text-5l md:text-4l sm:text-3l text-2l l:leading-70 lg:leading-12 leading-10">BGMI</h2>
                
                <p class="leading-8">Only 1 map (Erangle) will be there. It will be the final and decider map.
                    There should be Max 4 and Min.3 Man Squads.
                    During registration, there will be space for 5 people, 1 extra for backup player.
                    The playerid mustremain same during registration and gameplay, otherwise he/she will not
                    be allowed.
                    Each team mustselect their captain (IGL) who shall be responsible for communications with
                    the officials of the tournament. A team cannot change the team captain during the tournament
                    without prior approval of the tournament officials.
                    Players must not use an emulatorto play on a PC or other device that is not a handheld device.
                    It is a 16 Squad Event. If there are more than 25 teams, there will be anotherroom.
                    There is 1 point Granted Per 1 Kill.
                    Winner will be decided upon who has most point including position point and kill points.
                    There is no limitation on Team Registration.
                    There will be Cash Prize and Certificates.
                1.</p>
                <br/>
                <h2 class='date text-primary font-bold mb-2'>Registration Process</h2>
                <p class="leading-8">
                    ○ Participants must fill the form providing all necessary details.<br/>
                    ○ Deadline for registration is 10th May, 10pm.<br/>
                    ○ Entry Fees for Squad is <b>INR 200.(Per Head 50)</b>.<br/>
                    ○ For Registration <a href="https://technobites.bio.link/" target="blank"><b><i>Click here</i></b></a><br/>
                </p>
            </div>


             <div class="description mt-6">
                <h2 class="text-white font-bold uppercase xl:text-title lg:text-5l md:text-4l sm:text-3l text-2l l:leading-70 lg:leading-12 leading-10">VALORANT</h2>
                
                <p class="leading-8">It will be a knockout tournament. (Up to Semi Finale)
                Each team will be scheduled with their versusteam by the moderators.
                The map will be decided by doing the toss between two teams.
                Registration will be done online through google forms.
                Registration is First Come First Serve. (Team No is Limited)
                It is a 5 Players Team Tournament, with no substitutes.
                All games will take place on Mumbaiservers only.
                Each team must present 1 representative as a captain. He/she isresponsible for
                his/herteam and will be responsible for choosing maps and all communication
                with authorities must be done through the team captain.
                The map in each match played will be decided by doing a toss.
                A moderator would be spectating the matches at all times.
                Players notready within 15 minutes priorto their match willresult in a forfeit.
                The match will have the same rules as Standard matches. The first team to win 13
                rounds(in-game) will be declared the victor of the match and will advance.
                The initial fixture is knockouts and only one map is played.
                For Semi Finals and Finalsthere will be 2 maps, and in case of a DRAW there will
                be 3rd map (decider map) picked by the moderators.
                No changes will be made to yourteam information afterregistration closes.
                Minor changes can be done in rules which will be informed to all the participants
                before the tournament.
                Maps: Ascent, Split, Fracture, Bind, Breeze, Icebox, Haven.
                Players can carry their gear(Keyboard, mouse, mousepad, earphone) if they want.
                1.</p>
                <br/>
                <h2 class='date text-primary font-bold mb-2'>Registration Process</h2>
                <p class="leading-8">
                    ○ Participants must fill the form providing all necessary details.<br/>
                    ○ Deadline for registration is 10th May, 10pm.<br/>
                    ○ A player is allowed to have only one (1) Valorant account active on our Google Form.<br/>
                    ○ Player ID should be same at the time of registration and playing the event.<br/>
                    ○ A player can be part of only one team.<br/>
                    ○ Any deviation from the above guidelines will result in immediate disqualification forthe team.<br/>
                    ○ The tournament entering fee is <b>Rs.400 per squad (per 80 perteam)</b>.<br/>
                    ○ For Registration <a href="https://technobites.bio.link/" target="blank"><b><i>Click here</i></b></a><br/>
                </p>
            </div>
            <br><br>
            <h2 class="date text-primary font-bold mb-2 "><a href="https://drive.google.com/drive/folders/10bxTZVY__WfBONiX6jiZBzRhdgqrxPcY"><i>For all other events click here ➢</i></a></h2>
            <!-- <div class="description mt-6">
                <h3 class="text-2xl text-white uppercase font-bold mb-5">Description:</h3>
                <p class="leading-8">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500 when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap electro typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
                <p class="leading-8">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500 when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap electro typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
            </div>
            <div class="description mt-6">
                <h3 class="text-2xl text-white uppercase font-bold mb-5">Features:</h3>
                <p class="leading-8">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500 when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap electro typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
                <p class="leading-8">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500 when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap electro typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
            </div>
            <div class="description mt-6">
                <h3 class="text-2xl text-primary uppercase font-bold mb-5">Whats New!</h3>
                <p class="leading-8">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500 when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap electro typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
            </div>

            <blockquote class="py-5 mb-5">
                <p class="font-bold text-yellow italic lg:text-3xl text-xl">Lorem Ipsum is simply dummy text of the printing and typesetting industry has been the industry's standard dummy text ever since the 1500 printer took galley of type scrambled it to make a type specimen book.</p>
            </blockquote>

            <div class="additional-information-area bg-secondary-100 px-9 py-9 rounded-2xl mb-9">
                <h3 class="text-2xl text-white uppercase font-bold mb-6">Additional Information:</h3>
                <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 xl:grid-cols-5 gap-5 text-white">
                    <div class="additional_information_text">
                        <h4 class="font-bold mb-5">Updated:</h4>
                        <p class=" text-gray-400">2021-01-02</p>
                    </div>
                    <div class="additional_information_text">
                        <h4 class="font-bold mb-5">SIZE:</h4>
                        <p class=" text-gray-400">98MB</p>
                    </div>
                    <div class="additional_information_text">
                        <h4 class="font-bold mb-5">INSTALLS:</h4>
                        <p class=" text-gray-400">80,000,000+</p>
                    </div>
                    <div class="additional_information_text">
                        <h4 class="font-bold mb-5">CURRENT VERSION:</h4>
                        <p class=" text-gray-400">03.00.28.00.00</p>
                    </div>
                    <div class="additional_information_text">
                        <h4 class="font-bold mb-5">IN-APP PRODUCTS:</h4>
                        <p class=" text-gray-400">$0.85 - $985.00</p>
                    </div>
                </div>
            </div>
            <div class="description mt-6">
                <p class="leading-8">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500 when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap electro typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
                <p class="leading-8">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500 when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap electro typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
            </div> -->
        </div>
        
        <Disqus class=" mt-10" shortname='Admin' />
  </div>
</template>

<script>
import { Swiper, SwiperSlide } from 'vue-awesome-swiper';
import { Disqus } from 'vue-disqus'
export default {
    components: {
        Swiper,
        SwiperSlide,
        Disqus
    },
    props: ["games"],
    data () {
        return {    
            swiperOption: {
                slidesPerView: 1,
                spaceBetween: 30,
                pagination: false,
                navigation: {
                    nextEl: '.gameslide .gameslide-button-next',
                    prevEl: '.gameslide .gameslide-button-prev'
                }
            },
            gameslide: [
                {
                    gamingBg: "/images/others/popular-game-thumb11.png"
                },
                {
                    gamingBg: "/images/others/popular-game-thumb2.png"
                },
                {
                    gamingBg: "/images/others/popular-game-thumb3.png"
                },
                {
                    gamingBg: "/images/others/popular-game-thumb4.png"
                }
            ]
        }
    }
}
</script>