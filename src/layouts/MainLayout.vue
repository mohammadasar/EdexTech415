<template>
  <q-layout view="lHh Lpr lFf" >
    <q-header style="background-color:#a207f0; height: 60px; display: flex; align-items: center; justify-content: center;" >
      <q-toolbar>
      

        <q-toolbar-title class=" text-h5 text-weight-bold ">
          ExamsDaily
        </q-toolbar-title>   
        <div class="text-weight-bold gt-sm ">
          <q-btn flat rounded color="gray-1" label="Home" />
          <q-btn flat rounded color="gray-1" label="Enquiry" />
          <q-btn flat rounded color="gray-1" label="Contact Us" />
        </div>
        <!-- <q-btn flat round dense icon="menu" class="q-mr-sm lt-md" /> -->
        <q-btn flat @click="drawerRight = !drawerRight" round dense icon="menu"  class="q-mr-sm lt-md"/>


      </q-toolbar> 
  
    </q-header>

    <q-drawer
        side="right"
        v-model="drawerRight"
        :mini="miniState"
        @mouseover="miniState = false"
        @mouseout="miniState = true"
        mini-to-overlay
        :width="200"
        :breakpoint="500"
        bordered
        :class="$q.dark.isActive ? 'bg-grey-9' : 'bg-grey-3'"
      >
        <q-scroll-area class="fit" :horizontal-thumb-style="{ opacity: 0 }">
          <q-list padding>
            <q-item clickable v-ripple>
              <q-item-section avatar>
                <q-icon name="home" />
              </q-item-section>

              <q-item-section>
               Home
              </q-item-section>
            </q-item>

            <q-item  clickable v-ripple>
              <q-item-section avatar>
                <q-icon   class="bx bxs-book-content"/>
              </q-item-section>

              <q-item-section>
                Enquiry Form
              </q-item-section>
            </q-item>

            <q-item clickable v-ripple>
              <q-item-section avatar>
                <q-icon  class="bx bxs-phone-call" />
                
              </q-item-section>

              <q-item-section>
                Contact Us
              </q-item-section>
            </q-item>

          </q-list>
        </q-scroll-area>
      </q-drawer>



    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from 'vue'



export default defineComponent({
  name: 'MainLayout',

  // setup () {
  //   const rightDrawerOpen = ref(false)

  //   return {
  //     rightDrawerOpen,
  //     toggleRightDrawer () {
  //       rightDrawerOpen.value = !rightDrawerOpen.value
  //     },
  //     miniState: ref(true)
  //   }
  // },
  setup () {
    return {
      drawerRight: ref(false),
      miniState: ref(true)
    }
  }

})
</script>
