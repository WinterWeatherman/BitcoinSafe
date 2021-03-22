<template>
  <div>
  <center class="switchComp">
    <label class="switch">
        <input type="checkbox">
        <span class="slider round"></span>
    </label>
  </center>
  <containerOne></containerOne>
  <containerTwo></containerTwo>
</div>
</template>


<script>

import containerOne from './components/containerOne'
import containerTwo from './components/containerTwo'

export default {
  name: 'switchComp',
  components: {
    containerOne,
    containerTwo,
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
  margin: 0 10px;
}

a {
  color: #42b983;
}



</style>


