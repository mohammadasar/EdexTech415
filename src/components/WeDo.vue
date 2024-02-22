<template>
    
        <div class="row q-pa-lg q-mt-md">
            <div class="col-12 col-sm-5  q-pa-lg">
                <div class="text-h4 text-weight-bold q-pl-xl" ><p style="border-bottom: 4px solid #a207f0; border-;">What We Do</p></div>
                <div class="text-subtitle1 q-pa-xl  " style="display: flex; flex-direction: column; justify-content: center; align-items: center;" >
                   <p>{{ para1 }}</p>
                    <p> {{ para2 }}</p>
                  </div>
                  <div class="q-pl-xl">
                    <q-btn class="glossy shadow-8 text-h6 text-weight-bold" rounded color="purple" label="Read More"  />
                  </div>
                
            </div>
            <div class="col-12 col-sm-7">
                <div class="row q-pa-lg">
                    <div class="col-12 col-sm-6  q-pa-md"> 
                      <div class="q-pa-lg shadow-up-8" style="border: 1px solid #a207f0; border-radius: 5px;">
                        <div>
                        <img src="../assets/chair.png " >
                        </div>
                        <div class="text-h5">
                            <p>Our Mission</p>
                        </div>
                        <div class="text-subtitle1">
                           <p>{{ para3 }}</p>
                        </div>
                        <div>
                            <q-btn flat style="color:#a207f0" label="Read More.." class="text-h6 text-weight-bold"/>
                        </div>
                    </div>
                    </div>

                    <div class="col-12 col-sm-6 q-pa-md" >
                       <div class="q-pa-lg shadow-up-8" style="border: 1px solid #a207f0; border-radius: 5px;" >
                        <div>
                        <img src="../assets/sketch.png " >
                        </div>
                        <div class="text-h5">
                            <p>Our Activity</p>
                        </div>
                        <div class="text-subtitle1">
                           <p>{{ para4 }}</p>
                        </div>
                        <div>
                            <q-btn flat style="color:#a207f0" label="Read More.." class="text-h6 text-weight-bold" />
                        </div>
                    </div>
                    </div>
                </div>
                <!-- second row -->
                <div class="row q-pa-lg">
                    <div class="col-12 col-sm-12 q-pa-sm "> 
                       <div class="q-pa-lg shadow-10" style="border: 1px solid #a207f0; border-radius: 5px; ">
                        <div>
                        <img src="../assets/pallete.png " >
                        </div>
                        <div class=" text-h5">
                            <p>Our Vision</p>
                        </div>
                        <div class=" text-subtitle1">
                           <p>{{ para5 }}</p>
                        </div>
                        <div>
                            <q-btn flat style="color:#a207f0" label="Read More.."  class="text-h6 text-weight-bold" />
                        </div>
                    </div>
                    </div>
                    </div>
            </div>

        </div>
    

</template>
<script>
export default{
    name:'WeDo',
    setup(){
    return{
        para1:'EXAMSDAILY ACADEMY IS NO1 BANK EXAM COACHING CENTRE IN MADURAI AND one of the most trusted educational institution to learn progress, and build careers in major governmental organizations.WE caters the need of the aspiring students in different places across Tamil Nadu providing exceptional services and courses.',
        para2:'More than 500 candidates and aspiring government job seekers take up competitive exam courses from us AND EVEN THEY clear ALL exams INSTANTLY to find opportunities. Our COACHING IS MAINLY focused on student development mock recruiti interviews, exam research, and enterprise knowledge sharing. Salient features § EXAMSDAILY academyis the first and only institute of the country to give concepts and techniques for all types of questions.',
        para3:'Our COACHING IS MAINLY focused on student development mock recruiting interviews,exam research,and enterprise knowledge sharing.',
        para4:'ExamsDaily academy is the first and only institute of the country to give concepts and techniques for all types of questions.',
        para5:'Our COACHING IS MAINLY focused on student development mock recruiting interviews, exam research, and enterprise knowledge sharing.'
    }
}
}

</script>
<style scoped>

</style>