<template>
    <q-card class="card q-pa-md row justify-center" v-for="C in cardData" :style="{backgroundColor:C.clr}">
        <q-card-section class="text-center">
            <q-img :src="C.img" width="104px" height="72px"></q-img>
        </q-card-section>
        <q-card-section class="text-center text-h5">
            {{ C.textContent }}
        </q-card-section>
    </q-card>
</template>
<script>
import { defineComponent } from 'vue'

   export default defineComponent ({
       name:'Card',
       setup(){
           return{
            cardData: [
            {
              clr:"#0f8cff",
              img:"https://assets-v2.scaler.com/assets/academy/svg/at-a-glance/structured-c36517d8d41efb3a24cbcb3fe1c8b27ffcfacb6b1462ec3e60516504a07eaff6.svg.gz",
              textContent:"Structured, industry-vetted curriculum"
            },
            {
              clr:"#ea576f",
              img:"https://assets-v2.scaler.com/assets/academy/svg/at-a-glance/live-classes-afff2e39f63a26a19ee4ae844d4b0891c20c50e4b670a224564640cbb973f867.svg.gz",
              textContent:"Live classes by faculty who have been there, done that"
            },
            {
              clr:"#5cdb57",
              img:"https://assets-v2.scaler.com/assets/academy/svg/at-a-glance/project-0bb55588beaf037c5e46bbae951691f151400448579f0b7b516e9499fad41e4a.svg.gz",
              textContent:"Practical experience through real-life projects"
            },
            {
              clr:"#a768d7",
              img:"https://assets-v2.scaler.com/assets/course_page/svg/Aspirational-Network-78875977e997d138a67f82b59c51b4d72f45c015383b24c80cc71d93b12c151e.svg.gz",
              textContent:"Aspirational peer group of 2,000+ Edex Tech students & alumni"
            },
            {
              clr:"#fca733",
              img:"https://assets-v2.scaler.com/assets/course_page/svg/Career-Support-1c9f39867c1f2a4466d4466284d4724186f0d0216413c09449b6b12fa050525c.svg.gz",
              textContent:"Regular 1:1 mentorship from industry veterans"
            },
            {
              clr:"#4c96e5",  
              img:"https://assets-v2.scaler.com/assets/course_page/svg/Mentorship-b164f5d6fea02d5854f31e49686542629be67a644c73e3d95c5e1a3bc63e37aa.svg.gz",
              textContent:"Career support via a dedicated recruitment team, alumni network, etc"
            }
          ]
           }
       }
    })
</script>
<style>
.card{
  width: 400px;
  height:270px
}
</style>   
   