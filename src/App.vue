

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
  max-width: 43.75rem;
}

.card-header-two {
    padding: 4.25% 10%;
    margin-bottom: 0;
    background-color: #007bff;
    border-bottom: 10% solid #007bff;
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
  border: solid gray 1%;
}

.card-border-bold{
  border: 0.06rem solid #007bff;
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
  grid-template-columns: repeat(auto-fit, minmax(11.8rem, 20fr));
  grid-template-rows: auto;
  gap: 2.5rem 2rem;
  margin: auto;
  width: 100%;
  margin: auto;
  padding-left: 2rem;
  max-width: 56rem;
}

.borderstyle {
    width: 100%;
    max-width: 73.75rem;
    margin: auto;
    border-top: .25rem solid rgb(236, 239, 241);
    padding: 1.75rem 1.25rem 2.5rem;
}

.grid-item {
  height: 100%;
  min-width: 0rem;
  grid-column-end: span 1;
  grid-row-end: span 1;
  width: 11.8rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}

.grid-a {
  color: rgba(17, 51, 83, 0.6);
  cursor: pointer;
  font-size: 1rem;
  text-decoration: none;
  transition: color 0.25s ease 0s;
}

.grid-p {
  margin: 0rem;
  font-size: 1rem;
  font-weight: 400;
  color: rgba(17, 51, 83, 0.6);
  line-height: 1.5rem;
  box-sizing: border-box;
}

.grid-p-2 {
  margin: 0rem;
  font-size: 1rem;
  line-height: 2rem;
  color: rgb(5, 15, 25);
  font-weight: 600;
}

.grid-img {
  width: 100%;
  margin-bottom: 1.5rem;
  border-radius: 50%;
  border: 0.08rem solid rgb(236, 239, 241);
  padding: 0.5rem;
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
    border: 0rem solid rgba(0,0,0,.125);
    border-radius: .25rem;
}

.custom-row{
  display: flex;
  flex: wrap;
}

.right{
  margin-left: 0.6rem;
}

.left{
  margin-right: 0.6rem;
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
  top: 0.25rem;
  width: 3rem;
  height: 1rem;
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
  height: 75%;
  width: 25%;
  bottom: 12.5%;
  left: 4%;
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
  box-shadow: 0 0 0.08rem #2196F3;
}

input:checked + .slider:before {
  -webkit-transform: translateX(1.5rem);
  -ms-transform: translateX(2rem);
  transform: translateX(2rem);
}

/* Rounded sliders */
.slider.round {
  border-radius: 1.6rem;
}

.slider.round:before {
  border-radius: 50%;
}

.container {
  max-width: 60rem;
}

.pricing-header {
  max-width: 43.75rem;
}

.card-deck .card {
  min-width: 13rem;
}

.border-top { border-top: 0.06rem solid #e5e5e5; }
.border-bottom { border-bottom: 0.06rem solid #e5e5e5; }

.box-shadow { box-shadow: 0 .25rem .75rem rgba(0, 0, 0, .05); }
</style>
