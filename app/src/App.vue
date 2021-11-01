<template>
  <q-layout view="hHh lpR lFr">

    <q-header reveal bordered class="bg-primary text-white" height-hint="98">
      <q-toggle v-model="CNLang" color="blue"  model-value="CNlang"/>
      <q-toggle v-model="darkTheme" color="gray" model-value="darkTheme"/>
    </q-header>

    <q-page-container>
      <div class="row">
        <div class="col-0 col-xl-2"></div>
        <div class="col-12 col-xl-8">
          <div class="row">
            <!--          sidebar-->
            <div class="col-12 col-md-2">
              <h1> Hui Chong </h1>
              <div class="bg-primary" style="height: 300px"></div>
              Research assistant
              Fudan University
              Email: huichong.me@gmail.com
              Office: 220, Handan Road, Yangpu District, Shanghai, China

              GitHub
              Google Scholar
              ORCID
            </div>
            <div class="col-12 col-md-10">
              <div class="row">
                <div class="col-12">
                  <h2>Education</h2>
                  <ul>
                    <li>BSc Bioinformatics, <span class="text-bold">Huazhong University of Science and Technology</span></li>
                  </ul>
                </div>
              </div>
              <div class="row">
                <div class="col-12">
                  <h2>Research</h2>
                  Currently my research is mainly focused on applications of deep learning in microbiome data mining.
                </div>
              </div>
              <div class="row">
                <div class="col-12">
                  <h2>Publication</h2>
                  <div class="row bg-secondary" style="height: 500px">
                    xxxxxx
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-0 col-xl-2"></div>
      </div>
    </q-page-container>

  </q-layout>
</template>

<script>
import { ref } from 'vue'

export default {
  setup () {
    const leftDrawerOpen = ref(false)

    return {
      leftDrawerOpen,
      toggleLeftDrawer () {
        leftDrawerOpen.value = !leftDrawerOpen.value
      }
    }
  }
}
</script>