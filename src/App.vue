

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

.pricing-header{
  max-width: 700px;
}

.card-header-two {
    padding: .75rem 1.25rem;
    margin-bottom: 0;
    background-color: #007bff;
    border-bottom: 1px solid #007bff;
    color: white;
}

.avatar{
  margin-right: auto;
  margin-left: auto;
  vertical-align: middle;
  width: 50%;
  height: 50%;
  border-radius: 50%;
  display: block;
  border: solid gray 10px;
}

.card-border-bold{
  border: 1px solid #007bff;
}

#app {
  width:100%;
}

.p {
    margin-top: 0;
    margin-bottom: 1rem;
    display: block;
}

.grid{
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(190px, 20fr));
  grid-template-rows: auto;
  gap: 40px 32px;
  margin: auto;
  width: 100%;
  margin: auto;
  padding-left: 2rem;
  max-width: 900px;
}

.borderstyle {
    width: 100%;
    max-width: 1180px;
    margin: auto;
    border-top: 4px solid rgb(236, 239, 241);
    padding: 28px 20px 40px;
}

.grid-item {
  height: 100%;
  min-width: 0px;
  grid-column-end: span 1;
  grid-row-end: span 1;
  width: 190px;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}

.grid-a {
  color: rgba(17, 51, 83, 0.6);
  cursor: pointer;
  font-size: 16px;
  text-decoration: none;
  transition: color 0.25s ease 0s;
}

.grid-p {
  margin: 0px;
  font-size: 16px;
  font-weight: 400;
  color: rgba(17, 51, 83, 0.6);
  line-height: 24px;
  box-sizing: border-box;
}

.grid-p-2 {
  margin: 0px;
  font-size: 16px;
  line-height: 32px;
  color: rgb(5, 15, 25);
  font-weight: 600;
}

.grid-img {
  width: 100%;
  margin-bottom: 24px;
  border-radius: 50%;
  border: 2px solid rgb(236, 239, 241);
  padding: 8px;
}

.card-two {
    position: relative;
    display: -ms-flexbox;
    display: flex;
    -ms-flex-direction: column;
    flex-direction: column;
    min-width: 0;
    word-wrap: break-word;
    background-color: #007bff;
    background-clip: border-box;
    border: 1px solid rgba(0,0,0,.125);
    border-radius: .25rem;
}

.custom-row{
  display: flex;
  flex: wrap;
}

.right{
  margin-left: 10px;
}

.left{
  margin-right: 10px;
}

.flex {
  margin-right: auto;
  margin-left: auto;
  display: flex;
  justify-content: center;
}

.center {
  margin-right: auto;
  margin-left: auto;
  display: block;
}

.switch {
  position: relative;
  top: 4px;
  width: 50px;
  height: 18px;
}

/* Hide default HTML checkbox */
.switch input {
  opacity: 0;
  width: 0;
  height: 0;
}

/* The slider */
.slider {
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #2196F3;
  -webkit-transition: .4s;
  transition: .4s;
}

.slider:before {
  position: absolute;
  content: "";
  height: 15px;
  width: 15px;
  bottom: 1.5px;
  right: 33.5px;
  background-color: white;
  -webkit-transition: .3s;
  transition: .3s;
}


.lead {
    font-size: 1.25rem;
    font-weight: 300;
}

input:checked + .slider {
  background-color: #2196F3;
}

input:focus + .slider {
  box-shadow: 0 0 2px #2196F3;
}

input:checked + .slider:before {
  -webkit-transform: translateX(26px);
  -ms-transform: translateX(26px);
  transform: translateX(32px);
}

/* Rounded sliders */
.slider.round {
  border-radius: 30px;
}

.slider.round:before {
  border-radius: 50%;
}
</style>
