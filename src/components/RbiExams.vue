<template>
<div class="q-pa-md">
    <q-parallax :height="250" :speed="0.5">
      <template v-slot:media >
        
        <img src="../assets/rbi.jpg" width="100%" style="background-repeat: no-repeat;
         background-position: center ;
          
          padding: 80px 0px 80px;">
          <section  style="position: absolute; left: 0; right: 0; width: 100%; height: 100%; background-color: rgba(0,0,0,0.80);"></section>
      </template>
      <div style="position: absolute; left: 100px; top: 90px; color:white;" >
        <p class="text-weight-bold" style="font-size: 1.5vw;">EXAMSDAILY</p>
        <p class="text-weight-bold" style="font-size: 3vw; border-bottom: 4px solid purple;">RBI EXAMS</p>
      </div>
      
    </q-parallax>
  </div>

  <!-- para -->
  <div class="q-pa-md">
    <q-splitter
      v-model="splitterModel"
      horizontal
      style="height: 400px"
    >

      <template v-slot:before>
        <div class="q-pa-md">
          <!-- <div class="text-h4 q-mb-md">Before</div> -->
          <div>
            <p class="text-h6 text-weight-bold">RBI Exam Coaching Center</p>
            <p>{{ para1 }}</p>
          </div>

          <div>
            <p class="text-h6 text-weight-bold">RBI Exams</p>
            <p>{{ para2 }}</p>
             <p>{{ para3 }}</p> 
             <p>{{ para4 }}</p> 
             <p>{{ para5 }}</p>
          </div>
        </div>


      </template>

     

    </q-splitter>
  </div>
  </template>
  <script>
  import { ref } from 'vue'

export default {
  setup () {
    return {
      splitterModel: ref(100), // start at 100%
      para1:'EXAMSDAILY ACADEMY IS THE BEST TNPSC COACHING IN CHENNAI AND one of the most trusted educational institution to learn, progress, and build careers in major governmental organizations.WE caters the need of the aspiring students in different places across Tamil Nadu providing exceptional services and courses. More than 500 candidates and aspiring government job seekers take up competitive exam courses from us AND EVEN THEY clear ALL exams INSTANTLY to find opportunities. Our COACHING IS MAINLY focused on student development mock recruiting interviews, exam research, and enterprise knowledge sharing.',
      para2:'Our Bank exam classroom course prepares students in areas like Quantitative Aptitude (including Data Interpretation & Data Sufficiency), Reasoning & Logical Ability (including Non-Verbal Reasoning), English Language & Grammar, General Awareness (including socio-economic & financial awareness), Marketing Aptitude and Computer Knowledge.',
      para3:'Dhrona’s academy, the leader in classroom courses in chennai for Bank PO/Clerk Exams, also brings you the most comprehensive Correspondence Coaching for for Bank PO/Clerk Exams.dhrona’s acadey is best bank exam coaching centre in Chennai.',
      para4:'Students can get to a classroom programme for BANK PO AND CLERK EXAMS preparation. This course has been prepared based on our facultie expert team. Our Course ensures comprehensive coverage of all basic concepts, with solved examples, short-cuts and strategies for improvement of performance. The basic concepts that are taught in the classroom sessions, covering various test areas, are put together in the form of booklets that will ensure that you derive the same benefits as from the classroom programme. Dhrona,s academy is no 1 bank exam coaching in Chennai. You are given a lot of practice tests, on different topics, covering all the test areas. Our study material and test papers are prepared after carefully researching test papers of previous years, ensuring that you get the best and most relevant course material. This is also revised and updated over time to ensure that you get material that accurately reflects the latest paper pattern. Our course material is widely acknowledged by students as the most exhaustive and update in the market. The course enables the students to learn at a pace that is convenient to them. The material is comprehensive and developed with great care to ensure phased learning. Every module has been developed keeping in mind the various patterns and question types that have appeared over several years.dhrona’s accadey has placed one amoung top 10 bank exam coaching centre in Chennai,best ibps bank exam coaching centre in Chennai,best SBI clerk exam coaching in Chennai,best SBI PO exam coaching centre in Chennai,best RBI exam coaching centre in Chennai. Our study material coherently helps the student develop the skills required in different areas. The large number of practice exercises creates test conditions and also provides vital practice.',
      para5:'It’s time to put on makeup. It’s time to dress up right. It’s time to raise the curtain on the Muppet Show tonight. The mate was a mighty sailin’ man the Skipper brave and sure.',

    }
  }
}

</script>
<style>

</style>