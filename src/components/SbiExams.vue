<template>
  <div class="text-center q-mt-md " style="color:purple"><P class="text-h4 text-weight-bold" >Bank Exams</p>
  </div>
    <div class="q-pa-md">
      <q-parallax :height="250" :speed="0.5">
        <template v-slot:media >
          
          <img src="../assets/sbi.jpg" width="100%" style="background-repeat: no-repeat;
           background-position: center ;
           
            padding: 80px 0px 80px;">
            <section  style="position: absolute; left: 0; right: 0; width: 100%; height: 100%; background-color: rgba(0,0,0,0.80);"></section>
        </template>
        <div style="position: absolute; left: 100px; top: 90px; color: white;" >
          <p class="text-weight-bold" style="font-size: 1.5vw;">EXAMSDAILY</p>
          <p class="text-weight-bold" style="font-size: 3vw;  border-bottom: 4px solid purple;">SBI EXAMS</p>
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
          <!-- <div class="text-h4 text-weight-bold q-mb-md">SBI Exams</div> -->
          <div>
            <p class="text-h6 text-weight-bold">SBI Exam Coaching center in Madurai</p>
            <p>ExamsDaily Academy is the best bank exam coaching center in madurai was founded in 2011,we are providing extensive coaching for various competitive exams like</p>
          </div>
          <div>
            <p class="text-h6 text-weight-bold " >SBI EXAmS</p>
            <p>{{ para1 }}</p>
            <p>{{ para2 }}</p>
            <p>{{ para3 }}</p>
            <p>{{ para4 }}</p>
          </div>
          <div>
            <p class="text-h6 text-weight-bold " >SBI PO</p>
            <p>{{ para5 }}</p>
            <p>{{ para6 }}</p>
            <p>{{ para7 }}</p>
            <p>
              <ul>
              <li> Brand value of SBI and reputation associated with SBI PO post</li>
              <li> Lucrative pay scale which is highest among PSU Banks</li>
              <li> Growth opportunities where even a PO can progress to the level of Chairperson</li>
              <li> Job satisfaction and social prestige</li>
              </ul>
            </p>
            <p>{{ para8 }}</p>
            <div>
              <p class="text-h6 text-weight-bold " >SBI PO Notification DATE</p>
              <p>{{ para9 }}</p>
              <p>{{ para10 }}</p>
            </div>

            <div>
              <p class="text-h6 text-weight-bold " >SBI PO Preliminary Examination</p>
              <p>It is a 100 marks MCQ based paper with a time duration of 1 hour (60 mins). There are 3 sections (subjects) in this exam. Those are English Language, Numerical Ability & Reasoning Ability.</p>

            </div>

            <div>
              <p class="text-h6 text-weight-bold " >SBI PO Main Examination</p>
              <p>Its consists 2 parts - Objective Test (200 marks) and a descriptive test (50 marks).</p>
              <p>SBI PO Mains - Objective Test Paper pattern</p>
              <p>SBI PO Mains - Descriptive Test pattern</p>
              <p>SBI PO - Final</p>
              <p>Aspirants have to score an aggregate high in both parts, of Stage 2, to qualify for this round. SBI arranges these aggregate marks of all applicants in the descending order.</p>
              <p>{{ para11 }}</p>
              <p>{{ para12 }}</p>
            </div>

            <div>
              <p class="text-h6 text-weight-bold " >EXAMSDAILY ACADEMY Online exam platform</p>
              <P>{{ para13 }}</P>
              <p>{{ para14 }}</p>
              <p>Topic wise practice sets</p>
              <p>Sectional Tests</p>
              <p>Exam specific Full-Length Tests</p>
              <p>Effective and hassle-free analysis of your performance</p>
              <p>Our Reports & Analysis tool allows learners to monitor their progress and to identify competency gaps with added insights</p>
              <p>Our platform also encourages collaboration by allowing learners to ask questions and get answers from the relevant subject matter experts in the designed forums</p>

            </div>

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
      splitterModel: ref(100), // start at 50%

      para1:'EXAMSDAILY ACADEMY IS THE BEST TNPSC COACHING IN MADURAI AND one of the most trusted educational institution to learn, progress, and build careers in major governmental organizations.WE caters the need of the aspiring students in different places across Tamil Nadu providing exceptional services and courses. More than 500 candidates and aspiring government job seekers take up competitive exam courses from us AND EVEN THEY clear ALL exams INSTANTLY to find opportunities. Our COACHING IS MAINLY focused on student development mock recruiting interviews, exam research, and enterprise knowledge sharing.',
      para2:'Our Bank exam classroom course prepares students in areas like Quantitative Aptitude (including Data Interpretation & Data Sufficiency), Reasoning & Logical Ability (including Non-Verbal Reasoning), English Language & Grammar, General Awareness (including socio-economic & financial awareness), Marketing Aptitude and Computer Knowledge.',
      para3:'ExamsDaily academy, the leader in classroom courses in chennai for Bank PO/Clerk Exams, also brings you the most comprehensive Correspondence Coaching for for Bank PO/Clerk Exams.dhrona’s acadey is best bank exam coaching centre in Chennai.',
      para4:'Students can get to a classroom programme for BANK PO AND CLERK EXAMS preparation. This course has been prepared based on our facultie expert team. Our Course ensures comprehensive coverage of all basic concepts, with solved examples, short-cuts and strategies for improvement of performance. The basic concepts that are taught in the classroom sessions, covering various test areas, are put together in the form of booklets that will ensure that you derive the same benefits as from the classroom programme. Vimu academy is no 1 bank exam coaching in Madurai. You are given a lot of practice tests, on different topics, covering all the test areas. Our study material and test papers are prepared after carefully researching test papers of previous years, ensuring that you get the best and most relevant course material. This is also revised and updated over time to ensure that you get material that accurately reflects the latest paper pattern. Our course material is widely acknowledged by students as the most exhaustive and update in the market. The course enables the students to learn at a pace that is convenient to them. The material is comprehensive and developed with great care to ensure phased learning. Every module has been developed keeping in mind the various patterns and question types that have appeared over several years.dhrona’s accadey has placed one amoung top 10 bank exam coaching centre in Chennai,best ibps bank exam coaching centre in Chennai,best SBI clerk exam coaching in Chennai,best SBI PO exam coaching centre in Chennai,best RBI exam coaching centre in Chennai. Our study material coherently helps the student develop the skills required in different areas. The large number of practice exercises creates test conditions and also provides vital practice.',
     
      para5:'State Bank of India conducts SBI PO exam to select eligible candidates to the post of Probationary Officer.The SBI PO recruitment exam is top notch among the public-sector bank exams in India. It is considered a little difficult compared to other bank entrance exams.',
      para6:'An aspiring candidate appearing for the SBI PO exam has to pass 3 complex stages to clear the recruitment process',
      para7:'SBI PO 2019 exam will be conducted by State Bnak of India (SBI) to select eligible candidates to the post of Probationary Officer. SBI PO is one of the most coveted jobs in Banking industry and a dream job for millions of aspirants across India. SBI PO is considered as a premium job opportunity in Banking sector because of following reasons:',
      para8:'Before beginning with your preparation, you should get an idea about the latest updates, selection procedure, eligibility, exam pattern, syllabus, previous year cut off etc. Please go through this article to get all the important information for the SBI PO Exam.',
      
      para9:'The SBI PO 2019 Notification has been released by SBI IN April MONTH OF EVERY YEAR to recruit Probationary Officers (PO). SBI PO 2019 Prelims exam recruitment process has started after the release of official notification and it will be conducted for selection of candidates to the post of PO in State Bank of India and its Associate banks. The candidates selected are liable to be posted anywhere in India.',
      para10:'Eligible and interested Candidates are required to register online for the recruitment process. The 3-tier selection process consists of Preliminary and Main Exams which will be conducted online, followed by Interview. Candidates must pass each exam to get shortlisted and progress to the next stage. Final selection will be based on merit',
     
      para11:'Our (EXAMSDAILY ACADEMY) Bank sbi po classroom course helps the students in preparing for various Bank Entrance exams conducted by different BOARDS LIKE IBPS,SBI,RBI,etc across India. Our course is of 4 months duration that is designed for students who require exposure to fundamental concepts and adequate practice for preparation ',

      para12:'We even offer coaching for students beyond the above said duration for free of cost upto their placements. Our students will also be given study material that includes booklets for fundamentals apart from Class Exercises and Mock Tests.',
     
      para13:'We offer an exhaustive platform which conducts online examinations to measure the knowledge of the participants on the given exam syllabus. With our platform, students can attempt a wide variety of tests online, at the most convenient time, using any visual device, regardless of the location.',
      para14:'We have a wide range of question types to choose from. To name a few, we have included multiple choice text questions, Multiple choice image questions, Fill in the blanks and free text questions.',

    }
  }
}


</script>
<style scoped>


</style>