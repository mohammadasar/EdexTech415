<template>
    <div class="row" style="background-color:black; color:purple">
        <div class="col-12 col-md  q-pa-md"> 
            <div class="text-h5 text-weight-bold q-pa-md " ><p class="q-pb-sm" style="border-bottom: 4px solid purple;  border-radius: 10px;">EXAMSDAILY</p></div>
            <div class="q-pa-md">
        <P class="text-weight-bold">
          EXAMSDAILY ACADEMY IS NO1 BANK,TNPSC,RAILWAY,LIC,SSC EXAM COACHING CENTRE IN MADURAI AND one of the most trusted educational institution to learn, progress, and build careers in major governmental organizations.WE caters the need of the aspiring students in different places across Tamil Nadu providing exceptional services and courses.
        </P>
        <div class="text-h5 text-weight-bold" style="display: felx; justify-content:space-evenly; ">
           Follow Us:
           
            <img src="../assets/facebook.png" class="q-mr-sm q-ml-sm " >
            <img src="../assets/google.png" class="q-mr-sm q-ml-sm">
            <img src="../assets/instagram.png" class="q-mr-sm q-ml-sm">
            <img src="../assets/twitter.png" class="q-mr-sm q-ml-sm"> 
            
        </div>
        </div>

        </div>

        <div class="col-12 col-md q-pa-md">
            <div class="text-h5 text-weight-bold q-pa-md" >
                <p class="q-pb-sm" style="border-bottom: 4px solid purple;  border-radius: 10px;">Contact US</p>
            </div>
            <div class="text-weight-bold q-mt-md q-pa-md">
                <p><span class=" text-subtile1 text-weight-bold">Cell:</span>9361570033</p>
                <p><span class=" text-subtile1 text-weight-bold">write:</span>info@examsdaily.in</p>
               <p><span class="text-subtile1  text-weight-bold">Find us:</span> 2, Annai Theresa Street, Bethaniapuram, Madurai, Tamil Nadu 625016</p>
            </div>
        </div>
        <div class="col-12 col-md q-pa-md">
            <div class="q-pa-md">
            <p class=" text-h5 text-weight-bold q-pb-sm"  style="border-bottom: 4px solid purple; border-radius: 10px;">Join Our Newsletter</p>
            </div>
            <div class="q-mt-md">
                <q-input rounded outlined bg-color="white" color="purple" label="email"  v-model="text" style="text-color: purple;" 
                lazy-rules
                :rules="[ val => /.+@.+\..+/.test(val) || 'Please enter a valid email']"
>
        <template v-slot:append>
          
          <q-icon class="bx bx-envelope" color="purple"></q-icon>
        </template>
      </q-input>
            </div>
            <div class="q-mt-md " >
                <q-btn unelevated rounded color="purple" label="Submit" class="q-pa-md" style="width: 100%;  " />
            </div>
           
        </div>
    </div>
    

</template>
<script>
import { ref } from 'vue'

export default {
  setup () {
    return {
      text: ref(''),
      
    }
  }
}

</script>
<style>

</style>