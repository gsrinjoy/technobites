<template>
    <!-- Hero Banner Start -->
    <div class="flex items-center relative bg-no-repeat bg-scroll bg-center bg-cover 2xl:h-940 xl:h-820 lg:h-780 md:h-650 sm:h-620 h-620 lg:mb-32 md:mb-20 mb-15" style="background-image:url(/images/bg/hero-bg1.webp);">
        <div class="container">
            <div class="relative 2xl:pt-20 lg:pt-16 md:pt-10 sm:pt-8 pt-8 md:mb-12 z-10 flex flex-col justify-center items-center lg:items-start lg:text-left text-center">

                <h1 class="text-white font-metal uppercase font-normal 2xl:text-7.5xl xl:text-8xl lg:text-5.5xl md:text-7xl text-5xl tracking-wide xl:mb-10 lg:mb-8 mb-5 text-shadow">Ace to <br>the pinnacle.</h1>
                <p class="text-white font-semibold font-exo lg:mb-10 md:mb-6 text-base lg:text-2xl mb-5">Are you up for a real challenge to shine bright and gather repute?</p>

                <PrimaryButton/>

            </div>
        </div>
       
        <div class="absolute bottom-0 xl:right-14 lg:right-5 right-0 left-0 lg:left-auto text-center flex justify-center">
            <!-- <img style="width:60%;" class="2xl:w-940 xl:w-780 lg:w-650 md:w-620 w-450 md:text-center" src="images/technobites.png" alt="Position BG"> -->
            <div>
                <vue-countdown-timer
      @start_callback="startCallBack('event started')"
      @end_callback="endCallBack('event ended')"
      :start-time="'2018-10-10 00:00:00'"
      :end-time="1481450115"
      :interval="1000"
      :start-label="'Until start:'"
      :end-label="'Until end:'"
      label-position="begin"
      :end-text="'Event ended!'"
      :day-txt="'days'"
      :hour-txt="'hours'"
      :minutes-txt="'minutes'"
      :seconds-txt="'seconds'">
      <template slot="start-label" slot-scope="scope">
        <span style="color: red" v-if="scope.props.startLabel !== '' && scope.props.tips && scope.props.labelPosition === 'begin'">{{scope.props.startLabel}}:</span>
        <span style="color: blue" v-if="scope.props.endLabel !== '' && !scope.props.tips && scope.props.labelPosition === 'begin'">{{scope.props.endLabel}}:</span>
      </template>
 
      <template slot="countdown" slot-scope="scope">
        <span>{{scope.props.days}}</span><i>{{scope.props.dayTxt}}</i>
        <span>{{scope.props.hours}}</span><i>{{scope.props.hourTxt}}</i>
        <span>{{scope.props.minutes}}</span><i>{{scope.props.minutesTxt}}</i>
        <span>{{scope.props.seconds}}</span><i>{{scope.props.secondsTxt}}</i>
      </template>
 
      <template slot="end-label" slot-scope="scope">
        <span style="color: red" v-if="scope.props.startLabel !== '' && scope.props.tips && scope.props.labelPosition === 'end'">{{scope.props.startLabel}}:</span>
        <span style="color: blue" v-if="scope.props.endLabel !== '' && !scope.props.tips && scope.props.labelPosition === 'end'">{{scope.props.endLabel}}:</span>
      </template>
 
      <template slot="end-text" slot-scope="scope">
        <span style="color: green">{{ scope.props.endText}}</span>
      </template>
    </vue-countdown-timer>
            </div>
        </div>
        
    </div>
    <!-- Hero Banner End -->
</template>


<script>
    export default {
        name: 'Timer',
  methods: {
    startCallBack: function(x) {
      console.log(x);
    },
    endCallBack: function(x) {
      console.log(x);
    },
  },
        components: {
            PrimaryButton: () => import('@/components/Button/PrimaryButton')
        }
    };
</script>