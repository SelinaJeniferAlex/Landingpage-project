<template>
    <q-card class="CareerCard q-pa-md row justify-center" v-for="CD in CareerData">
        <q-card-section class="text-center">
            <q-img :src="CD.img" width="72px" height="72px"></q-img>
        </q-card-section>
        <q-card-section class="text-center text-h6">
            {{ CD.textContent }}
        </q-card-section>
    </q-card>
</template>
<script>
import { defineComponent } from 'vue'

   export default defineComponent ({
       name:'CareerCard',
       setup(){
           return{
                CareerData:[
                    {
                        img:"https://assets-v2.scaler.com/assets/academy/svg/employer-d308ffc80a2a4dcd539cdfc4da50dec20698c52fff259ff2dae4eea5dfb15e94.svg.gz",
                        textContent:"Access job opportunities from our 600+ employer partners"
                    },
                    {   
                        img:"https://assets-v2.scaler.com/assets/academy/svg/community-6fa9a0023c30456b10b76caa66f2de9daff9a4c74cc61bf19892cff4021c2a94.svg.gz",
                        textContent:"Exchange job opportunities with our extensive 20K+ Edex Tech student community"
                    },
                    {
                        img:"https://assets-v2.scaler.com/assets/academy/svg/mock-3ef075c86047b3d501bbef3e91e533db4d3215e30107f5e6645ce11dc7a358eb.svg.gz",
                        textContent:"Practice mock interviews with people working in the industry"
                    },
                    {
                        img:"https://assets-v2.scaler.com/assets/academy/svg/resume-b9775f453cdc3079a7031ec687839bbdab8b6cadf2c8f68ba0dfaf8e63045e2e.svg.gz",
                        textContent:"Optimize your resume & LinkedIn profile with our experienced experts"
                    }
                ]
           }
       }
    })
</script>
<style>
.CareerCard{
  width: 300px;
  height:300px;
}
</style>   
   