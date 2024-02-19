<template>
    <div class="card_wrapper q-ma-sm row justify-center">
      <div class="q-pa-md">
        <div class="row">
          <div class="col text-center aos-init aos-animate" data-aos="fade-down">
            <div class="text-h4">
              Gain confidence in Full Stack concepts, taught by experienced instructors
            </div>
            <p class="q-py-lg text-h6">
              Our faculty comprises experts from Amazon, Google, Hotstar, Facebook, Microsoft to name a few, who have successfully built scalable systems                
            </p>
          </div>
        </div>
        <div class="row">    
          <div class="col aos-init aos-animate" data-aos="fade-up">
            <div class="q-pa-md row justify-center q-gutter-md">
                <template v-for="(instructor, index) in instructors" :key="index">
                  <q-card class="my-card shadow rounded-borders q-my-md">
                    <img :src="instructor.image" width="200" height="200">
                    <q-card-section>
                      <div class="text-h6 text-center">{{ instructor.name }}</div>
                    </q-card-section>
                  </q-card>
                </template>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'CarouselCard',
    data() {
      return {
        instructors: [
          { name: 'Rajeev', image: 'src/assets/image/ins1.jpg' },
          { name: 'Piyuesh', image: 'src/assets/image/ins2.jpg' },
          { name: 'Keshave', image: 'src/assets/image/ins3.jpg' },
          { name: 'Kamalpreet', image: 'src/assets/image/ins4.jpg'},
          { name: 'Sekhar', image: 'src/assets/image/ins5.jpg' },
          { name: 'Navdeep', image: 'src/assets/image/ins6.jpg' },
          { name: 'Mandeep', image: 'src/assets/image/ins7.jpg' },
          { name: 'Nidhi', image: 'src/assets/image/ins8.jpg' },
          { name: 'Krishna', image: 'src/assets/image/ins9.jpg' },
          { name: 'Divya', image: 'src/assets/image/ins10.jpg' }
        ]
      }
    }
  }
  </script>
  
  <style>
  .my-card{
    width: 100%;
    max-width: 250px;
    max-height: 250px;
}
.card_wrapper .my-card{
	transition: .3s;
	height: 300px;
}

.card_wrapper .my-card:hover {
	transform: translateY(-10px);
}
.slider_carousel .owl-nav{
	 position: absolute;
	 top: 50%;
	 width: 100%;
}

.slider_carousel .owl-prev, .slider_carousel .owl-next {
	width: 20px;
	height: 20px;
	background-color: tomato;
	color: white;
	display: flex;
	align-items: center;
	justify-content: center;
	border-radius: 50%;
	position: absolute;
	top: 50%;	
	margin-left: 3px;
	margin-right: 3px;
}

.slider_carousel .owl-next {
    right: -30px;
}

.slider_carousel .owl-prev {
    left: -30px;
}
@media screen and (max-width:576px)
{
	.slider_carousel .owl-next {
		right: -25px;
	}
	
	.slider_carousel .owl-prev {
		left: -25px;
	}	
}
  </style>
  