
<template>
<div class="q-pa-md">
    <q-parallax :height="250" :speed="0.5">
      <template v-slot:media >
        
        <img src="../assets/IBPS.jpg" width="100%" style="background-repeat: no-repeat;
         background-position: center ;
          background-attachment: fixed; 
          padding: 80px 0px 80px;">
          <section  style="position: absolute; left: 0; right: 0; width: 100%; height: 100%; background-color: rgba(0,0,0,0.80);"></section>
      </template>
      <div style="position: absolute; left: 100px; top: 90px; color:white;" >
        <p class="text-weight-bold" style="font-size: 1.5vw;">EXAMSDAILY</p>
        <p class="text-weight-bold" style="font-size: 3vw; border-bottom: 4px solid purple;">IBPS EXAMS</p>
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
          <div >
            <P class="text-h6 text-weight-bold">IBPS PO Exam Coaching Center</P>
            <p>{{ para1 }}</p>
          </div>

          <div>
            <P class="text-h6 text-weight-bold">IBPS EXAMS</P>
            <p>{{ para2 }}</p>
            <p>{{ para3 }}</p>
          </div>

          <div>
            <p class="text-h6 text-weight-bold">IBPS PO</p>
            <p>{{ para4 }}</p>
            <p>{{ para5 }}</p>
          </div>

          <div>
            <p class="text-h6 text-weight-bold">IBPS PO Notification</p>
            <p>{{ para6 }}</p>
            <p>{{ para7 }}</p>
            <p>The exam is conducted in 3 phases:</p>
            <p>
                <ul>
                    <li>1. The IBPS PO Preliminary Exam</li>
                    <li>2. The IBPS PO Mains Exam</li>
                    <li>3. Interview</li>
                </ul>
            </p>
            <p>The IBPS PO preliminary examination is a 60 mins online examination.</p>
            <P>IBPS tests aspirants for 3 sections Quantitative Ability, Logical Reasoning & English Language.</P>
            <p>The IBPS PO Prelims has 100 questions in total with a maximum score of 100 marks</p>
            <p>There is negative marking of 1/4th marks for every wrong answer.</p>
           <p>{{ para8 }}</p>
           <P>{{ para9 }}</P>
           <P>{{ para10 }}</P>
           <p>{{ para11 }}</p>
           <p>EXAMSDAILY ACADEMY Online exam platform</p>
           <p>{{ para12 }}</p>
           <p>{{ para13 }}</p>
           <p>
            <ul>
                <li> Topic wise practice sets</li>
                <li> Sectional Tests</li>
                <li> Exam specific Full-Length Tests</li>
                <li> Exam specific booster tests on our app</li>
                <li> Effective and hassle-free analysis of your performance</li>
            </ul>
           </p>
           <p>{{ para14 }}</p>

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
      para1:'EXAMSDAILY ACADEMY IS THE BEST BANK EXAM COACHING IN MADURAI AND one of the most trusted educational institution to learn, progress, and build careers in major governmental organizations.WE caters the need of the aspiring students in different places across Tamil Nadu providing exceptional services and courses. More than 500 candidates and aspiring government job seekers take up competitive exam courses from us AND EVEN THEY clear ALL exams INSTANTLY to find opportunities. Our COACHING IS MAINLY focused on student development mock recruiting interviews, exam research, and enterprise knowledge sharing.',
      para2:'Our Bank exam classroom course prepares students in areas like Quantitative Aptitude (including Data Interpretation & Data Sufficiency), Reasoning & Logical Ability (including Non-Verbal Reasoning), English Language & Grammar, General Awareness (including socio-economic & financial awareness), Marketing Aptitude and Computer Knowledge',
      para3:'Students can get to a classroom programme for BANK PO AND CLERK EXAMS preparation. This course has been prepared based on our facultie expert team. Our Course ensures comprehensive coverage of all basic concepts, with solved examples, short-cuts and strategies for improvement of performance. The basic concepts that are taught in the classroom sessions, covering various test areas, are put together in the form of booklets that will ensure that you derive the same benefits as from the classroom programme. Vimu academy is no 1 bank exam coaching in Chennai. You are given a lot of practice tests, on different topics, covering all the test areas. Our study material and test papers are prepared after carefully researching test papers of previous years, ensuring that you get the best and most relevant course material. This is also revised and updated over time to ensure that you get material that accurately reflects the latest paper pattern. Our course material is widely acknowledged by students as the most exhaustive and update in the market. The course enables the students to learn at a pace that is convenient to them. The material is comprehensive and developed with great care to ensure phased learning. Every module has been developed keeping in mind the various patterns and question types that have appeared over several years.Vimu accadey has placed one amoung top 10 bank exam coaching centre in Chennai,best ibps bank exam coaching centre in Chennai,best SBI clerk exam coaching in Chennai,best SBI PO exam coaching centre in Chennai,best RBI exam coaching centre in Chennai. Our study material coherently helps the student develop the skills required in different areas. The large number of practice exercises creates test conditions and also provides vital practice.',
      
      para4:'IBPS (Institute of Banking Personnel Selection) conducts a common written exam or CWE every year for the probationary officers in multiple banks all over the country. All public sector banks use CWE as a base to fill the vacancies for this pos',
      para5:'IBPS is conducting po exam for every year and hence named IBPS po CWE . The IBPS po CWE exam is conducted on THREE levels- preliminary exam , mains EXAM AND INTERVIEW. Students qualifying in these exams are thus selected for the post.',
     
      para6:'IBPS will be releasing the Official Notification for IBPS po Exam shortly. The Exam dates have been released by IBPS through Exam Calendar for every year. The Online Registration for IBPS po will start after the release of Official Notification.',
      para7:'The Institute of Banking Personnel Selection [IBPS] is an autonomous body in the field of Employment Testing, Selection, Assessment, and Management of Human Resources in India. IBPS offers its services to all Regional Rural Banks (RRBs) and to about 27 Public-Sector Banks, SBI, Associate Banks of SBI, RBI, NABARD, SIDBI, LIC & Insurance companies and regular member Banks of the IBPS society. In the last few years, IBPS conducts the PO CWE, for hiring candidates, online',
      para8:'The IBPS PO Mains Examination is an online examination. This year IBPS has added a descriptive paper in its Mains exam worth 25 marks with a time duration of 30 mins. Thus, the total time allotted for the exam is 180 mins + 30 mins. With the recent updates to the exam, the IBPS PO Mains exam now has 5 sections (4 + 1)(Reasoning& Computer Aptitude, English Language, Data Analysis & Interpretation, General Economy & Banking Awareness and English Language (Letter Writing & Essay)with a maximum achievable score of 200 + 25 marks. In the Mains exam, IBPS also decides on sectional cut-offs depending on the difficulty levels of the exam',
      para9:'The Interview round is a face-to-face interaction. This round carries 100 marks. Only those candidates, who clear cut-offs in the IBPS PO mains examination, qualify for this round. It, "s a 15 to 20 minutes round. The candidate"s knowledge on topics related to Banking, Current Affairs, Government updates, etc is tested.',
      para10:'The Final Scores are then calculated on the basis of the marks obtained in the Mains Examination & the interview round individually where the weightage is spread in an 80:20 ratio respectively.',
      para11:'Our (Examsdaily ACADEMY) IBPS PO BANK EXAMclassroom course helps the students in preparing for various Bank Entrance exams conducted by different BOARDS LIKE IBPS,SBI,RBI,etc across India. Our course is of 4 months duration that is designed for students who require exposure to fundamental concepts and adequate practice for preparation.',
      para12:'We offer an exhaustive platform which conducts online examinations to measure the knowledge of the participants on the given exam syllabus. With our platform, students can attempt a wide variety of tests online, at the most convenient time, using any visual device, regardless of the location.',
      para13:'We have a wide range of question types to choose from. To name a few, we have included multiple choice text questions, Multiple choice image questions, Fill in the blanks and free text questions.',
      para14:'Our Reports & Analysis tool allows learners to monitor their progress and to identify competency gaps with added insights. Our platform also encourages collaboration by allowing learners to ask questions and get answers from the relevant subject matter experts in the designed forums.',

    
    
    }
  }
}


</script>
<style>

</style>