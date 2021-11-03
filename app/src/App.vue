<template>
  <q-layout view="lHr Lpr lFr">
    <q-header reveal bordered height-hint="98" class="bg-dark txt-white">
      <div class="row">
        <div class="col-0 col-xl-2 "></div>
        <div class="col-12 col-xl-8 ">
          <div class="row ">
            <div class="col-4 q-pa-md">
              <div class="text-h6">Hui Chong's Homepage</div>
            </div>
            <div class="col-4 offset-4 q-pa-md">
              <span>
                <q-btn-toggle v-model="language" no-caps rounded unelevated toggle-color="dark" color="white" text-color="dark"
                              :options="[{label: 'English', value: 'en'},{label: '中文', value: 'cn'}]"/>
                <q-btn-toggle v-model="theme" no-caps rounded unelevated toggle-color="dark" color="white" text-color="dark"
                              :options="[{label: 'Bright', value: 'bright'},{label: 'Dark', value: 'dark'}]"/>
              </span>
            </div>
          </div>
        </div>
        <div class="col-0 col-xl-2 "></div>
      </div>
    </q-header>
    <q-page-container>
      <div class="row">
        <div class="col-0 col-xl-2"></div>
        <div class="col-12 col-xl-8">
          <div class="row">
            <div class="col-12 col-md-4 q-pa-lg">
              <div class="text-h3 q-pa-lg">Hui Chong</div>
              <div class="q-pa-lg bg-secondary" style="height: 300px"></div>
              <div class="text-body1 q-pa-lg">
                Research assistant
                Fudan University
                Email: huichong.me@gmail.com
                Office: 220, Handan Road, Yangpu District, Shanghai, China

                GitHub
                Google Scholar
                ORCID
              </div>
            </div>
            <div class="col-12 col-md-8 q-pa-lg">
              <div class="row">
                <div class="col-12">
                  <h4>Education</h4>
                  <ul>
                    <li>BSc Bioinformatics, <span class="text-bold">Huazhong University of Science and Technology</span>
                    </li>
                  </ul>
                  <hr>
                </div>
              </div>
              <div class="row">
                <div class="col-12">
                  <h4>Research</h4>
                  Currently my research is mainly focused on applications of deep learning in microbiome data mining.
                  <hr>
                </div>
              </div>
              <div class="row">
                <div class="col-12">
                  <h4>Publication</h4>
                  <div class="row" style="height: 500px">
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
import {ref} from 'vue'

export default {
  setup() {
    const leftDrawerOpen = ref(false)

    return {
      leftDrawerOpen,
      toggleLeftDrawer() {
        leftDrawerOpen.value = !leftDrawerOpen.value
      }
    }
  },
  data() {
    return {
      language: 'en',
      theme: 'bright'
    }
  },
  methods: {

  }
}
</script>