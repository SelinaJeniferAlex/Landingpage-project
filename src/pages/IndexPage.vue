<template>
<q-page>
  <div class="bg-banner">
    <div class="row q-pa-md">
      <div class="col-12 col-md text-white">
        <div style="max-width: 650px;" class="q-ml-auto q-mr-auto">
          <div class="text-center text-h3 text-bold q-ma-lg q-py-xl">Full Stack Developer Course by Edex Tech</div>
          <div class="text-h5 q-px-xl">
            <ul>
              <li>Upskill in DSA & System Design with this Full Stack Developer Course</li>
              <li>Build real-world projects by mastering React, MERN, JavaScript, etc.</li>
              <li>Learn the essential Full Stack development concepts from scratch</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-12 col-md">
        <div style="max-width: 650px;" class="q-ml-auto q-mr-auto">
          <div class="q-ma-xl bg-white rounded-borders">
            <div class="text-center text-h6 q-pa-sm">
              <p>Request a callback to <br> Start your journey with Edex Tech!</p>
            </div>
            <div class="">
              <div class="q-px-xl q-py-md">
                <q-form
                  @submit="onSubmit"
                  class="q-gutter-sm"
                >
                  <q-input
                    filled
                    v-model="email"
                    label="Email-Id *"
                    lazy-rules
                    :rules="[ val => val && val.length > 0 || 'Please type email']"
                  />
                  <q-input
                    filled
                    v-model="year"
                    label="Graduation Year *"
                    lazy-rules
                    :rules="[ val => val && val.length > 0 || 'Please type something']"
                  />
                  
                  <q-select 
                    filled 
                    v-model="jobTitle" 
                    :options="options" 
                    label="Job Title *" 
                    lazy-rules
                    :rules="[ val => val && val.length > 0 || 'Please select title']"
                  />
                  
                  <q-input 
                    filled 
                    v-model="tel" 
                    type="tel" 
                    label="Telephone number"
                    lazy-rules
                    :rules="[ val => val && val.length > 0 || 'Please type mobile no']"  
                  />
                  <div class="flex flex-center q-ma-lg">
                    <q-btn label="Request" type="submit" color="primary"/>
                  </div>
                </q-form>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="container-fluid">
    <div class="container q-ma-md">
      <div class="row q-pa-xl" style="text-align: center;">
        <div class="text-h4 text-dark col">
          Full Stack Web Development Course Overview
        </div>
      </div>
      <div class="row">
        <div class="col-12 col-lg">
          <div class="q-pa-md items-start q-gutter-md">
            <q-card dark bordered class="bg-blue-6 shadow-7 my-card-over">
              <q-card-section>
                <div class="text-h5">About Edex Tech's Full Stack Developer Course</div>
              </q-card-section>

              <q-separator dark inset />

              <q-card-section class="text-h6">
                <ul>
                  <li>Learn practical coding skills through real-life projects</li>
                  <li>Structured curriculum covering programming constructs, DSA, CS fundamentals, and software/system design taught by industry veterans via live classes</li>
                  <li>Industry-expert faculty and 1:1 mentorship with a peer group of 2,000+ Edex Tech students and alumni.</li>
                </ul>
              </q-card-section>
            </q-card>
          </div>
        </div>
        <div class="col-12 col-lg">
          <div class="q-pa-md items-start q-gutter-md">
            <q-card dark bordered class="bg-blue-6 shadow-7 my-card-over">
              <q-card-section>
                <div class="text-h5">What is Full Stack Web Development and why is it important to learn?</div>
              </q-card-section>

              <q-separator dark inset />

              <q-card-section  class="text-h6">
                <div>
                  Full Stack Development is a software profession/stream where a developer deals with both the Frontend (client-side) and Backend (server-side) of a tech product. A Full Stack Developer is proficient in several technologies that help in developing a robust tech product, and thus play a major role in making decisions for the company. It is one of the high-demand jobs in the software industry.
                </div>
              </q-card-section>
            </q-card>
          </div>
        </div>
        <div class="col-12 col-lg">
          <div class="q-pa-md items-start q-gutter-md">
            <q-card dark bordered class="bg-blue-6 shadow-7 my-card-over">
              <q-card-section>
                <div class="text-h5">What skills will I master with this full stack course?</div>
              </q-card-section>

              <q-separator dark inset />

              <q-card-section  class="text-h6">
                <div>
                  Skills that you will master with this full-stack course are:
                </div>
                <ul>
                  <li>Programming constructs, algorithms, and data structures.</li>
                  <li>Advanced data structures, problem-solving, and computer science fundamentals.</li>
                  <li>Develop software and systems using OOP principles and system design techniques.</li>
                  <li>Build full-stack apps using technologies like REST APIs, MVC, and databases like MongoDB.</li>
                  <li>Build efficient data processing systems with ETL pipelines, big data tech, and cloud services.</li>
                </ul>
              </q-card-section>
            </q-card>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="bg-cyan-1 q-py-lg">
    <div class="text-center">
      <div class="row q-ma-md q-pa-md text-h4">
        <div class="col">Key highlights of the Edex Tech's Full Stack Developer Program</div>
      </div>
      <div class="row text-h6 text-blue-grey-13 q-pa-md">      
        <div class="col">Edex Tech's full-stack development program helps you learn exactly everything that you need to solidify your tech career</div>
      </div>
    </div>
    <div class="q-pa-md row q-gutter-lg justify-center">
      <Card></Card>
    </div>
  </div>
  <div class="bg-cyan-1 q-my-xl q-py-md">
    <div class="text-center">
      <div class="row q-ma-md q-pa-md text-h4">
        <div class="col">Curriculum is designed to make you a solid engineer</div>
      </div>
    </div>
    <div class="q-pa-md q-ma-md row justify-center gt-sm">
      <TabPanel></TabPanel>
    </div>
    <div class="q-ma-sm row justify-center lt-md">
      <TabAccordian></TabAccordian>
    </div>
  </div>
  <div class="q-my-lg q-py-md">
    <div class="text-center">
      <div class="row q-ma-sm q-pa-md text-h4">
        <div class="col">Career services</div>
      </div>
      <div class="row text-h6 text-blue-grey-13 q-pa-md">      
        <div class="col">Along with upskilling and preparing you to be a solid engineer, we will help you with your job search and interview preparation as well!</div>
      </div>
    </div>
    <div class="q-pa-md row q-gutter-lg justify-center">
      <CareerCard></CareerCard>
    </div>
  </div>
  <div class="bg-cyan-1 q-my-xl q-py-md">
    <div class="text-center">
      <div class="row q-ma-md q-pa-md text-h4">
        <div class="col">Edex Tech alumni work at reputed tech organizations and promising startups</div>
      </div>
    </div>
    <div class="q-pa-md q-ma-md q-gutter-lg row justify-center">
      <div class="col-12 col-md text-center">
        <q-img src="https://excelr.in/full-stack-development-course/assets/images/alumini/6.png" width="150px" height="100px"></q-img>
      </div>
      <div class="col-12 col-md text-center">
        <q-img src="https://excelr.in/full-stack-development-course/assets/images/alumini/2.jpg" width="150px" height="100px"></q-img>
      </div>
      <div class="col-12 col-md text-center">
        <q-img src="https://excelr.in/full-stack-development-course/assets/images/alumini/10.png" width="150px" height="100px"></q-img>
      </div>
      <div class="col-12 col-md text-center">
        <q-img src="https://excelr.in/full-stack-development-course/assets/images/alumini/20.png" width="150px" height="100px"></q-img>
      </div>
    </div>
  </div>
  <div class="q-my-xl q-py-md">
    <CarouselCard></CarouselCard>
  </div>
  <div class="q-my-xl">
    <div class="row justify-center q-pa-xl  bg-clr">
      <div class="col-12 col-md text-center text-h4 q-pa-md">
        Connect with an Academic Counsellor
      </div>
      <div class="col-12 col-md text-center q-pa-md">
        <q-btn color="red" glossy label="Request A Callback" />
      </div>
    </div>
  </div> 
  <div class="q-my-xl">
    <div class="row text-center">
      <div class="col text-h4 q-pa-md">
        Full Stack Development Course Fee
      </div>
    </div>
    <div class="row q-ma-md">
      <div class="col text-center q-pa-md">
        <q-img src="https://assets-v2.scaler.com/assets/academy/svg/money-logo-3bd15c9dc2c03678b1a868d7c8fc3c5bf01b7a2167be52d1ef8d6874d3abea56.svg.gz" width="65px" height="65px"></q-img>
      </div>
    </div>
    <div class="row">
      <div class="col text-center text-h5 q-pa-md">
        With scholarship & EMI options, your payment can be as low as Rs. 8,628 per month - that's like your monthly grocery bill!
      </div>
    </div>
    <div class="row">
      <div class="col text-center text-h6 text-blue-grey-14 q-pa-md">
        Total fee: Rs 3.69L inclusive of GST at super affordable EMI options. Try the course for the first 2 weeks - full money-back guarantee if you choose to withdraw.
      </div>
    </div>
    <div class="row">
      <div class="col text-center q-pa-md">
        <q-btn color="red" glossy label="View emi plans" />
      </div>
    </div>
  </div>
  <!-- FAQs -->
  <div class="q-pa-xl">
    <div class="row">
      <div class="col text-center text-h4 q-pa-md">
        Full Stack Web Development Course FAQs
      </div>
    </div>
    <div class="row justify-center q-my-md text-h6">
      <div class="col" style="max-width: 120vh;">
        <q-list bordered class="rounded-borders">
          <q-expansion-item>
            <template v-slot:header>
              <q-item-section>
                What is Edex Tech's full-stack development program?
              </q-item-section>
            </template>

            <q-card>
              <q-card-section>
                <div class>
                  <ul>
                    <li>Structured curriculum that covers CS Fundamentals and System Design via a project based approach. This curriculum has been industry-vetted and reverse-engineered by analysing what it takes to be a great engineer</li>
                    <li>Live classes that are held twice a week, with the timings determined by students in the batch</li>
                    <li>Tutors who have built scalable systems in the past and understand the real-life importance of DSA and System Design, not just interview-relevant material</li>
                    <li>Quick doubt resolution from our 100+ Teaching Assistants</li>
                    <li>Aspirational peer group and access to EdexTechChat, our internal communication tool wherein you can collaborate with others on projects, get authentic interview experiences and share job-referrals</li>
                    <li>Flexible curriculum that help you continue learning despite your hectic work schedule. We provide recorded lectures to view later and also allow you to move between batches at NO cost</li>
                    <li>Career support - we provide job opportunities via our 600+ employer partners, mock interview services and career planning services</li>
                  </ul>
                </div>
              </q-card-section>
            </q-card>
          </q-expansion-item>

          <q-separator />

          <q-expansion-item>
            <template v-slot:header>
              <q-item-section>
                Who is eligible for Edex Tech's Full Stack course?
              </q-item-section>
            </template>

            <q-card>
              <q-card-section>
                <div>
                  Software engineers with any number of years of experience can choose to join Edex Tech's Full Stack program. Applicants currently in college (1st, 2nd, 3rd or final year of college) could consider to join Scaler Edge, our college student focused product. Please visit www.edextech.com/edge for more detail
                </div>
              </q-card-section>
            </q-card>
          </q-expansion-item>
          <q-separator />

          <q-expansion-item>
            <template v-slot:header>
              <q-item-section>
                When are the live classes held?
              </q-item-section>
            </template>

            <q-card>
              <q-card-section>
                <div>
                  Live classes are normally held 2 times a week, with the exact class days and timings being determined by the batch. However, given all learners would be software engineers that are currently working, the classes would be held in the late evening or night on weekdays and any suitable time over the weekends.            </div>
              </q-card-section>
            </q-card>
          </q-expansion-item>
          <q-separator />

          <q-expansion-item>
            <template v-slot:header>
              <q-item-section>
                What happens if I miss a lecture in this online full stack developer course?          </q-item-section>
            </template>

            <q-card>
              <q-card-section>
                <div>
                  All lectures are recorded and you will have access to the recordings after the lecture is completed.            </div>
              </q-card-section>
            </q-card>
          </q-expansion-item>
          <q-separator />

          <q-expansion-item>
            <template v-slot:header>
              <q-item-section>
                Can I attend this full stack developer training part-time?          </q-item-section>
            </template>

            <q-card>
              <q-card-section>
                <div>
                  The program has a fixed schedule, during which you would attend live-lectures with a dedicated instructor, Teaching Assistant, and personal mentor. 15 hour weekly commitment is required for the duration of the program in order to achieve positive results.            </div>
              </q-card-section>
            </q-card>
          </q-expansion-item>
        </q-list>
      </div>
    </div>
  </div>
  <div class="bg-cyan-1 q-pa-md q-mt-md">
    <div class="text-h5 text-red text-weight-bolder text-center">Edex Tech</div>
      <div class="text-center text-h6 q-pa-sm flex flex-center">
             <div class="q-ma-sm">
          <q-icon name="location_on" class="q-mr-sm" />AVM Complex, Annai Theresa Street, Kalavasal, Madurai
        </div>
        <div class="q-ma-sm">
          <q-icon name="email" class="q-mr-sm" /> hello@edex.com
        </div>
        <div class="q-ma-sm">
          <q-icon name="phone" class="q-mr-sm" /> +919085299999
        </div>
      </div>
  </div>
</q-page>
</template>

<script>
import { defineComponent } from 'vue'
import Card from 'components/Card.vue'
import TabPanel from 'components/TabPanel.vue'
import CareerCard from 'src/components/CareerCard.vue'
import CarouselCard from 'src/components/CarouselCard.vue'
import TabAccordian from 'src/components/TabAccordian.vue'
import demo from 'src/components/demo.vue'

export default defineComponent({
  name: 'IndexPage',
  components:{
    Card,TabPanel,CareerCard,CarouselCard,TabAccordian,demo
  },
  setup(){
    return{
      
    }
  }
})
</script>
<style>
.bg-clr{
  background:linear-gradient(109deg, rgba(231,243,255,0.8) 52%, #a5d2ff 89%);
}
.bg-banner{
  background-image: url(https://assets-v2.scaler.com/assets/course_page/banner/banner-svg-b723839c1463b82a3ad793feab1036dc2b1bae9627985de45bb8f9a9dcbbab07.svg.gz);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
.my-card-over{
  height: 600px;
} 
@media (max-width:1024px){
  .my-card-over{
    height:auto;
  }
}
</style>
