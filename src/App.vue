

<template>
  <div id="app">
    <body>
      <headerComp></headerComp>
      <div class="flex">
        <p class="left">High Security</p>
        <div>
          <label class="switch">
            <input v-model="highSecurity" type="checkbox">
            <span class="slider round"></span>
          </label>
        </div>
        <p class="right">Fast Setup</p>
      </div>
      <containerTwo v-if="highSecurity"></containerTwo>
      <containerOne v-else></containerOne>

      <footerComp></footerComp>
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
/* The switch - the box around the slider */

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

#app {
  width:100%;
}

.grid{
  display: grid;
  grid-template-columns: repeat(2fr, minmax(250px, 1fr));
  grid-template-rows: auto;
  gap: 40px 32px;
  margin: auto;
  width: 100%;
  margin: auto;
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
  width: 60px;
  height: 34px;
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
  height: 26px;
  width: 26px;
  left: 4px;
  bottom: 4px;
  background-color: white;
  -webkit-transition: .4s;
  transition: .4s;
}

input:checked + .slider {
  background-color: #2196F3;
}

input:focus + .slider {
  box-shadow: 0 0 1px #2196F3;
}

input:checked + .slider:before {
  -webkit-transform: translateX(26px);
  -ms-transform: translateX(26px);
  transform: translateX(26px);
}

/* Rounded sliders */
.slider.round {
  border-radius: 34px;
}

.slider.round:before {
  border-radius: 50%;
}
</style>
