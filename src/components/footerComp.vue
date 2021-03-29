<template>
  
  <div class="footerComp">
    <footer>
      <h2 class='contributors'>Contributors</h2> 
      <a class='footerLinkText' href="https://docs.google.com/spreadsheets/d/1BxAiGnhCfFifd6T6Ky1m3gwdePvuS6QteXsc5KadlPI">See individal reviews and comments</a>
     
      <div class="grid">
        <div class="grid-item">
          <a class="grid-a">
            <img class="grid-img" src="../assets/bjdwecktwtimg.jpg">
            <p class="grid-p-2">BJ Dweck</p>
          </a>
          <p class="grid-p">@bjdweck</p>
          <p class="grip-p">Professional Bitcoin Consultant</p>
        </div>
        <div class="grid-item">
          <a class="grid-a">
            <img class="grid-img" src="../assets/zachherberttwrimg.jpg">
            <p class="grid-p-2">Zach Herbert</p>
          </a>
          <p class="grid-p">@zachherbert</p>
          <p class="grip-p">Founder, Foundation Devices</p>
        </div>
        <div class="grid-item">
          <a class="grid-a">
            <img class="grid-img" src="../assets/garylelandtwrimg.jpg">
            <p class="grid-p-2">Gary Leland</p>
          </a>
          <p class="grid-p">@GaryLeland</p>
          <p class="grip-p">Founder Bit Block Boom Bitcoin Conference</p>
        </div>
        <div class="grid-item">
          <a class="grid-a">
            <img class="grid-img" src="../assets/thibaudtwrimg.jpg">
            <p class="grid-p-2">Thibaud Maréchal</p>
          </a>
          <p class="grid-p">@thibm_</p>
          <p class="grip-p">Founder, Knox Custody</p>
        </div>
        <div class="grid-item">
          <a class="grid-a">
            <img class="grid-img" src="../assets/martindaletwrimg.jpg">
            <p class="grid-p-2">Eric Martindale</p>
          </a>
          <p class="grid-p">@martindale</p>
          <p class="grip-p">Bitcoin Side Chain Architect</p>
        </div>
        <div class="grid-item">
          <a class="grid-a">
            <img class="grid-img" src="../assets/somsenrubentwrimg.jpg">
            <p class="grid-p-2">Somsen Ruben</p>
          </a>
          <p class="grid-p">@SomsenRuben</p>
          <p class="grip-p">Bitcoin Side Chain Architect</p>
        </div>
        <div class="grid-item">
          <a class="grid-a">
            <img class="grid-img" src="../assets/sanket1729twrimg.jpg">
            <p class="grid-p-2">Sanket Kanjalkar</p>
          </a>
          <p class="grid-p">@sanket1729</p>
          <p class="grip-p">R&D at Blockstream</p>
        </div>
        <div class="grid-item">
          <a class="grid-a">
            <img class="grid-img" src="../assets/guyswannimg.png">
            <p class="grid-p-2">Guy Swan</p>
          </a>
          <p class="grid-p">@TheCryptoconomy</p>
          <p class="grip-p">Host of Bitcoin Audible and Shitcoin Insider</p>
        </div>
        <div class="grid-item">
          <a class="grid-a">
            <img class="grid-img" src="../assets/jwweatherman_twrimg.jpg">
            <p class="grid-p-2">JW Weatherman</p>
          </a>
          <p class="grid-p">@jwweatherman_</p>
          <p class="grip-p">Sofware Security Expert</p>
        </div>
        <div class="grid-item">
          <a class="grid-a">
            <img class="grid-img" src="../assets/AaronvanWtwrimg.jpg">
            <p class="grid-p-2">Aaron van Wirdum</p>
          </a>
          <p class="grid-p">@AaronvanW</p>
          <p class="grip-p">Technical Edtor, Bitcoin Magazine</p>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'footerComp',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.text-center{
  text-align: center;
}

.contributors{
  margin: 0rem 0rem 0.75rem;
    font-size: 2.12rem;
    font-weight: 700;
    line-height: 2.12rem;
    margin-left: 1.8rem;
}

.footerLinkText{
  font-weight: 700;
  margin-left: 2.12rem;
  color: gray;
  margin-bottom: 1.5rem;
}


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
</style>
