<template>
      <div class="q-pa-md" style="max-width:100% ; background-color: #cccccc;">
   
        <!-- <div class="row"> -->
     <div class=" text-center q-mt-md ">
      <p>
        <!-- class=" text-weight-bold text-h4 " -->
        <!-- class=" text-weight-bold q-pa-sm text-h6" -->

      <span  style="color:#a207f0; font-size: 2.8vw; font-weight: bold; ">Enquiry Form : </span>
      <span class="q-pa-sm"
       style="background-image: linear-gradient(90deg,#a207f0,#d7a2e0); border-radius: 30px; font-size: 1.9vw;"> 
         Kindly post your queries  in the below from.We willget in touch with you shortly  </span>
        </p>
        </div>  
    <!-- </div> -->

      <q-form 
     
      @submit="onSubmit"
      class="q-gutter-md q-mt-lg"
      style=" width:100%;"
      
      
    >

    
    <div class="row q-pa-lg">
      <div class="col-12 col-md  q-pa-md">
      <q-input rounded standout bottom-slots v-model="name" label="Your Name" 
      lazy-rules
        :rules="[ val => val && val.length > 0 || 'Please type your name']"
        style="color: #a207f0;"      >  
        <template v-slot:prepend>
        <q-icon class='bx bx-user-circle' />
        </template>
        <template v-slot:append>
          <q-icon name="close" @click="name=''" class="cursor-pointer" />
        </template>

        <template v-slot:hint>
          Your Name
        </template>
      </q-input>  
    </div>  

      <div class="col-12 col-md  q-pa-md ">
      <q-input rounded standout bottom-slots v-model="email" label="Email"
      lazy-rules
      :rules="[ val => /.+@.+\..+/.test(val) || 'Please enter a valid email']">
        <template v-slot:prepend>
          <q-icon name="email" />
        </template>
        <template v-slot:append>
          <q-icon name="close" @click="email=''" class="cursor-pointer" />
        </template>

        <template v-slot:hint>
          Your Email Id
        </template>
      </q-input>
   </div>

     <div class="col-12 col-md  q-pa-md">
      <q-input rounded standout bottom-slots v-model="number" label="Mobile Number"
      lazy-rules
        :rules="[
          val => val !== null && val !== '' || 'Please type your number',
          val => val > 0 && val < 100 || 'Please type your currect  number'
        ]" 
        
        >
        <template v-slot:prepend>
          <q-icon name="phone" />
        </template>
        <template v-slot:append>
          <q-icon name="close" @click="number = ''" class="cursor-pointer" />
        </template>

        <template v-slot:hint>
          Mobile Number
        </template>
      </q-input>
       </div>

       </div>

      <div  
      class="row q-mt-lg  ">
      <div class="col-12 col-md-8  q-pr-lg text-center">
       <q-radio keep-color v-model="accept" val="purple" color="purple" 
       style="color: #a207f0; font-weight: bold; font-size:1.8vw" >
       I would Like to receive updates from ExamsDaliy Banking Accademy 
      </q-radio>
       </div>

       <div class="col-12 col-md-4 text-center">
       <q-btn label="Submit" type="submit" style="background-color: #a207f0;" />
      </div>

      </div>
    </q-form>
   

  </div>

    
    </template>
    <script>
    import { useQuasar } from 'quasar'
    import { ref } from 'vue'

    export default {
         name:'EnquiryForm',
          setup () {
    const $q = useQuasar()

    const name = ref(null)
    const email = ref(null)
    const number = ref(null)
    const accept = ref(false)

    return {
      name,
      email,
      number,
      accept,
   
      onSubmit () {
        if (accept.value !== true) {
          $q.notify({
            color: 'purple',
            textColor: 'purple',
            icon: 'warning',
            message: 'You need to accept the license and terms first'
          })
        }
        else {
          $q.notify({
            color: 'green-4',
            textColor: 'purple',
            icon: 'cloud_done',
            message: 'Submitted'
          })
        }
       
      }

    }
  }

    
    }
    </script>
    <style scoped>
    
    q-input:active{
         background-color: blueviolet;
    }
    
    
    </style>