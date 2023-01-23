<template>
  <div class="directions">
    <div class="container">
      <div class="directions-text">
        <h1>Our directions and advantages</h1>
        <p>
          Integrate once and never worry about scaling again. We ensure composability between ecosystem projects by maintaining a single global state as the network scales.
        </p>
      </div>
      <div class="directions-cards">
        <div class="card">
        <img :src="card_1" alt="" class="directions-img">
        <h2 class="directions-title">Powerful for developers</h2>
        <p class="directions-card-text">Cucoin is a decentralized blockchain built to enable scalable, user-friendly apps for the world.</p>
        <a href="!#" class="directions-btn">Learn more</a>
      </div>
        <div class="card">
        <img :src="card_2" alt="" class="directions-img">
        <h2 class="directions-title">Low cost, forever</h2>
        <p class="directions-card-text">Our scalability ensures transactions remain less than $0.01 for both developers and users.</p>
        <a href="!#" class="directions-btn">Learn more</a>
      </div>
        <div class="card">
        <img :src="card_3" alt="" class="directions-img">
        <h2 class="directions-title">Decentralized</h2>
        <p class="directions-card-text">The network is spread over thousands of independent nodes,so  your transactions are always safe.</p>
        <a href="!#" class="directions-btn">Learn more</a>
        <img :src="arrow" alt="">
      </div>
      </div>
    </div>
  </div>
</template>
<script>
import card_1 from '@/assets/card_1.svg'
import card_2 from '@/assets/card_2.svg'
import card_3 from '@/assets/card_3.svg'
import aroow from '@/assets/arrow.svg'
export default {
  setup() {
    return {
      card_1,
      card_2,
      card_3,
      aroow
    }
  }
}
</script>
<style lang="scss">
  .directions {
    font-family: 'Manrope';
    padding-top: 260px;
    padding-bottom: 200px;
}
.directions-text {
  text-align: center;
  h1 {
    font-family: 'Manrope';
  font-weight: 800;
  font-size: 48px;
  line-height: 60px;
  margin-bottom: 24px;
  }
  p {
  font-weight: 400;
  font-size: 24px;
  line-height: 34px;
  margin-bottom: 48px;
  }
}
.directions-cards {
  display: flex;
  justify-content: space-between;
}
.card {
  border: 1px solid rgba(255, 255, 255, 0.1);
  border-radius: 24px;
  text-align: center;
  padding: 25.5px 45px;
  max-width: 380px;
}
.card + * {
  margin-left: 1rem;
}
.directions-img {
  margin-bottom: 1rem;
}
.directions-title {
  font-weight: 700;
  font-size: 20px;
  line-height: 25px;
  margin-bottom: 1rem;
  
}
.directions-card-text {
  font-weight: 400;
  font-size: 16px;
  line-height: 20px;
  color: rgba(255, 255, 255, 0.8);
  margin-bottom: 1rem;
}
.directions-btn {
  font-weight: 700;
  font-size: 16px;
  line-height: 20px;
}
</style>