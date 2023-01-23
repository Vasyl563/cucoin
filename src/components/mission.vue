<template>
  <div class="mission">
    <div class="container">
    <div class="mission-content">
      <div class="mission-text">
        <h2>
          Our goal and mission
        </h2>
        <p>Whether you’re an experienced trader or just getting started, Cucoin has all the tools you need. Execute your trading strategies with the professional level crypto trading platform.</p>
    </div>
      <div class="mission-goal">
        <img :src="libra" class="mission-goal-img"/>
        <div class="mission-goal-text">
        <p class="mission-goal-text__line line1">An accessible way to buy, sell, and store non-fungible tokens (NFTs) – digital art on the blockchain. You can expect the same industry-leading security technology.</p>
        <p class="mission-goal-text__line line2">The project aims to build increasing connectivity to Ethereum and the wider blockchain ecosystem. AVAX, Avalanche’s native token, is the network’s unit of your persocnal account.</p>
        <p class="mission-goal-text__line line3">High performance tools for active traders and industry-leading security from day one.</p>
        <a  href="!#" class="button-position btn-join">Join our community</a>
        </div>
      </div>
    </div>
  </div>
  </div>
</template>
<script>
import libra from '@/assets/Libra.png'
export default {
  setup () {
    return {
      libra
    }
  }
}
</script>
<style lang="scss">
 .mission {
    padding-top: 118px;
    z-index: 10000;
}
.mission-content {
  
}


.mission-text{
  text-align: center;
  h2 {
    font-weight: 800;
    font-size: 48px;
    line-height: 60px;
    padding-bottom: 1.5rem;
  }
  p {
    font-weight: 400;
    font-size: 24px;
    line-height: 34px;
    padding-bottom: 2.5rem;
  }
}
.mission-goal {
  display: flex;
  justify-content: space-between;
  max-width: 497px;
}
.mission-goal-img {
  margin-right: 87px;
  max-width: 583px;
}
.mission-goal-text{
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: left;
}
.mission-goal-text {
  p {
    padding-bottom: 2.5rem;
    font-weight: 400;
    font-size: 18px;
    line-height: 25px;
    // width: 471px;
  }
}
.mission-goal-text__line {
  max-width: 470px;
  // margin-left: 87px;
  /* необходим для формирования позиций линий */
  position: relative;
  /* блок будет занимать ширину по размеру контента в нём*/
  display: inline-block;
}

.mission-goal-text__line:before{ 
  content: " ";
  background: rgba(255, 139, 243, 0.6);
  width: 5px;
  // height: 70px;
  /* линия смещена на 10px слева от текста*/
  left: -28px;
  /* включаем абсолютное позиционирование относительно блока с relative */
  position: absolute;
}
.line1::before{
  height: 70px;
}
.line2::before{
  height: 100px;
}
.line3::before{
  height: 50px;
}

.button-position {
  left: 0;
}
</style>