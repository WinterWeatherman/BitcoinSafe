<template>
  <div class="headerComp">

    <header class="d-flex flex-column flex-md-row align-items-center p-3 px-md-4 mb-3 bg-body border-bottom shadow-sm">
      <p class="h5 my-0 me-md-auto fw-normal">Bitcoin Safe.io</p>
    </header>
  </div>
</template>

<script>
export default {
  name: 'headerComp',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 0.8rem;
}

a {
  color: #42b983;
}
html {
  font-size: 14px;
}
@media (min-width: 768px) {
  html {
    font-size: 16px;
  }
}

.divvid{
    height: 500;
    width: 500;
}


.line{
    width: 100%;
    max-width: 1180px;
    margin: auto;
    border-top: 4px solid rgb(236, 239, 241);
    padding: 2rem 2rem 3rem;
}

.margin-bottom{
  padding-bottom: 2rem;
}

.container {
  max-width: 960px;
}

.pricing-header {
  max-width: 700px;
}

.btn-primary {
    color: #fff;
    background-color: white;
    border-color: #007bff;
    color: black;
}

.btn-bold {
    color: #fff;
    background-color: #007bff;
    border-color: #007bff;
}

.card-header-two {
    padding: .75rem 1.25rem;
    margin-bottom: 0;
    background-color: #007bff;
    border-bottom: .006rem solid #007bff;
    color: white;
}



@media only screen and (min-width: 729px) {
  .longimg {
    max-width: 50%;
    height: auto;
    width: auto;
    padding-bottom: 3rem;
  } 
}


@media only screen and (max-width: 729px){
  .longimg {
    display: none!important;
  }
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

.p {
    margin-top: 0;
    margin-bottom: 1rem;
    display: block;
}

.a{
  color: black;
}


.grid{
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(11.8rem, 20fr));
  grid-template-rows: auto;
  gap: 2.5rem 2rem;
  margin: auto;
  width: 100%;
  padding-top: 2.5rem;
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
  justify-self: center;
}

.grid-a {
  color: rgba(17, 51, 83, 0.6);
  cursor: pointer;
  font-size: 1rem;
  text-decoration: none;
  transition: color 0.25s ease 0s;
}

.grid-p {
  margin: 0px;
  font-size: 16px;
  font-weight: 400;
  color: rgba(17, 51, 83, 0.6);
  line-height: 1.5rem;
  box-sizing: border-box;
}

.grip-p {
  margin: 0px;
  font-size: 16px;
  font-weight: 400;
  color: rgba(17, 51, 83, 0.6)!important;
  line-height: 1.5rem;
  box-sizing: border-box;
}


.grid-p-2 {
  margin: 0rem;
  font-size: 1rem;
  line-height: 2rem;
  color: rgb(5, 15, 25);
  font-weight: 600;
  color: black!important;
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
  display: inline-block;
  width: 60px;
  height: 34px;
  top: -0.3rem;
}

.switch {
  position: relative;
  display: inline-block;
  width: 60px;
  height: 34px;
}

.switch input {
  opacity: 0;
  width: 0;
  height: 0;
}

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
  -webkit-transition: .3s;
  transition: .3s;
}

.slider.round {
  border-radius: 1.6rem;
}

.slider.round:before {
  border-radius: 50%;
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

.container {
  max-width: 60rem;
}

.pricing-header {
  max-width: 43.75rem;
}

.headertext{
  margin: 0rem 0rem 0.75rem;
    font-size: 2.12rem;
    font-weight: 700;
    line-height: 2.12rem;
    margin-left: 1.8rem;
}

.card-deck .card {
  min-width: 13rem;
}

.border-top { border-top: 0.06rem solid #e5e5e5; }
.border-bottom { border-bottom: 0.06rem solid #e5e5e5; }

.box-shadow { box-shadow: 0 .25rem .75rem rgba(0, 0, 0, .05); }

</style>

