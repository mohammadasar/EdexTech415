<template>
  <!-- <q-page style="background-color:#d6d0d0 ;"> -->
      <!-- <div class="q-pa-md"> -->

        <Offers></Offers>
        <!-- class="q-mt-lg " -->
    <q-carousel
    
     style="height:600px;"
      animated
      v-model="slide"
      navigation
      infinite
      :autoplay="autoplay"
      arrows
      transition-prev="slide-right"
      transition-next="slide-left"
      @mouseenter="autoplay = false"
      @mouseleave="autoplay = true"
    >
    
      <q-carousel-slide :name="1" img-src="../assets/Curosel1.png"  style=" background-position: center ;">
      <div class="text-start text-h3 text-weight-bold" style=" font-size: 5vw; position: absolute; left: 120px; bottom: 220px; color: white;  "  >
        <p >{{ heading }}</p>
        <p>{{ title }}</p>
        <p>{{ title1 }}</p>
        <p>{{ title2 }}</p>
        
        
      </div>
      <q-btn class="glossy" rounded color="purple" label="Contact Us" style=" font-size: 2vw; position: absolute; left:120px; bottom: 130px;" />
      </q-carousel-slide>

      <q-carousel-slide :name="2" img-src="../assets/curosels2.png"  style=" background-position: center ;" >
        <div class="text-start  text-weight-bold" style=" font-size: 4vw; position: absolute; left: 120px; bottom: 200px; color: white;  "  >
        <p>{{ heading1}}</p>
        <p>{{ title }}</p>
        <p>{{ title1 }}</p>
        <p>{{ title2 }}</p>
        
      </div>
      <q-btn class="glossy" rounded color="purple" label="Contact Us"  style=" font-size: 2vw; position: absolute; left:120px; bottom: 110px;"/>
      </q-carousel-slide>
    </q-carousel>
  <!-- </div> -->
<!-- </q-page> -->

  
  <EnquiryForm :is="currentView" ></EnquiryForm>
  <Choose></Choose>
  <Wedo></Wedo>
  <!-- <Facilitys></Facilitys> -->
  <SbiExams></SbiExams>
  <RbiExams></RbiExams>
  <IbpsExams></IbpsExams>
  <Footer></Footer>

</template>

<script>
import { defineComponent } from 'vue'
import EnquiryForm from '../components/EnquiryForm.vue'
import Choose from '../components/Choose.vue'
import Offers from '../components/Offer.vue'
import Wedo from '../components/WeDo.vue'
// import Facilitys from '../components/Facility.vue'
import SbiExams from '../components/SbiExams.vue'
import RbiExams from '../components/RbiExams.vue'
import IbpsExams from '../components/IbpsExams.vue'
import Footer from '../components/Footer.vue'
import { ref,computed } from 'vue'



export default defineComponent({
  name: 'IndexPage',
  components:{
    EnquiryForm,
    Choose,
    Offers,
    Wedo,
    // Facilitys,
    SbiExams,
    RbiExams,
    IbpsExams,
    Footer

  
  },
  setup () {
    return {
      slide: ref(1),
      autoplay: ref(true),
      heading:'EXAMSDAILY Academy',
      heading1:'SSC',
      title:'The Best',
      title1:'Bank Exam Coaching',
      title2:'Center In Madurai'
    }
  }

})

const routes = {
  // '/': Home,
  '/EnquiryForm': EnquiryForm
}

const currentPath = ref(window.location.hash)

window.addEventListener('hashchange', () => {
  currentPath.value = window.location.hash
})

const currentView = computed(() => {
  return routes[currentPath.value.slice(1) || '/'] || NotFound
})
</script>
