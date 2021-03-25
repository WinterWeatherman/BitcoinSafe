<template>
  
  <div class="containerTwo">
    <div>
      <div class="container">
        <div class="card-deck mb-3 text-center">
          <div class="card mb-4 box-shadow">
            <div class="card-header">
              <h4 class="my-0 font-weight-normal">Blue Wallet</h4>
            </div>
            <div class="card-body">
              <h1 class="card-title pricing-card-title">$0</h1>
              <ul class="list-unstyled mt-3 mb-4">
                <li>1 Minute to Spend</li>
                <li>20 Minutes to Setup</li>
                <li>Terrible Privacy</li>
                <li>Bad Theft Prevention</li>
              </ul>
              <a type="button" class="btn btn-lg btn-block btn-primary" href="https://Bluewallet.io/#">Get started</a>
            </div>
          </div>
          <div class="card mb-4 box-shadow">
            <div class="card-header">
              <h4 class="my-0 font-weight-normal">Eclair</h4>
            </div>
            <div class="card-body">
              <h1 class="card-title pricing-card-title">$0</h1>
              <ul class="list-unstyled mt-3 mb-4">
                <li>1 Minute to Spend</li>
                <li>1 Hour to Setup</li>
                <li>Terrible Privacy</li>
                <li>Bad Theft Prevention</li>
              </ul>
              <a type="button" class="btn btn-lg btn-block btn-primary" href="https://play.google.com/store/apps/details?id=fr.acinq.eclair.wallet.mainnet2&hl=en_US&gl=US">Get started</a>
            </div>
          </div>
          <div class="card card-border-bold mb-4 box-shadow">
            <div class="card-header card-header-two">
              <h4 class="my-0 font-weight-normal">Green Address</h4>
            </div>
            <div class="card-body">
              <h1 class="card-title pricing-card-title">$0</h1>
              <ul class="list-unstyled mt-3 mb-4">
                <li>1 Minute to Spend</li>
                <li>1 Hour to Setup</li>
                <li>Bad Privacy</li>
                <li>Good Theft Prevention</li>
              </ul>
              <a type="button" class="btn btn-lg btn-block btn-primary" href='https://greenaddress.it/en/'>Get started</a>
            </div>
          </div>
        </div>
      </div>
    </div> 
  </div>
</template>


<script>
export default {
  name: 'containerTwo',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
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
