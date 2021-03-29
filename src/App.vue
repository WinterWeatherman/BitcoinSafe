

<template>
  <div id="app">
    <body>
      <headerComp></headerComp>
      <div class="pricing-header px-3 py-3 pt-md-5 pb-md-4 mx-auto text-center">
        <h1 class="display-4">Bitcoin Safe</h1>
        <p class="lead">Bitcoin storage solutions curated by Bitcoin experts. Ratings are averaged to make it easy to pick the best solution. </p>
      </div>
      <div class="flex">
        <p class="left">High Security</p>
        <div>
          <label class="switch">
            <input v-model="highSecurity" type="checkbox">
            <span class="slider round"></span>
          </label>
        </div>
        <p class="right">Fast and Easy</p>
      </div>
      <containerTwo v-if="highSecurity"></containerTwo>
      <containerOne v-else></containerOne>
      <footerComp class='borderstyle'></footerComp>
    </body>
  </div>
</template>

<script>

import headerComp from './components/headerComp'
import containerOne from './components/containerOne'
import containerTwo from './components/containerTwo'
import footerComp from './components/footerComp'

export default {
  name: 'app',
  components: {
    headerComp,
    containerOne,
    containerTwo,
    footerComp
  },
  data () {
    return {
      highSecurity: true
    }
  }
}
</script>

<style>
html {
  font-size: 14px;
}
@media (min-width: 768px) {
  html {
    font-size: 16px;
  }
}

.container {
  max-width: 960px;
}

.pricing-header {
  max-width: 700px;
}

.card-deck .card {
  min-width: 220px;
}

.border-top { border-top: 1px solid #e5e5e5; }
.border-bottom { border-bottom: 1px solid #e5e5e5; }

.box-shadow { box-shadow: 0 .25rem .75rem rgba(0, 0, 0, .05); }


</style>
