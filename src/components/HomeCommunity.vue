<template>
  <div class="community">
   <div class="container">
    <div class="community-content">
        <h1>The World’s Fastest Growing Crypto Community</h1>
      <p>A highly-curated platform for creating, collecting and trading unique NFTs. Trade with confidence on the world’s fastest and most secure crypto exchange</p>
<form class="example" action="/action_page.php" style="margin:auto;max-width:436px">
  <input type="text" placeholder="Your email address" name="search2">
  <a class="btn-join btn-position" type="submit">Join our community</a>
</form>
<!-- <img :src="image1" class="community-img"/> -->
<div class="figure">
<div class="shadow"></div>
<div class="elipse"></div>
</div>
    </div>
   </div>
   
  </div>
</template>

<script>
import image1 from '@/assets/Mask group.png'
export default {
 setup () {
    return {
      image1
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
  .community {
    padding-top: 100px;  
    // padding-bottom: 120px; 
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;  
    text-align: center; 
  
}

.community-content {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  position: relative;
  z-index: 100;
  h1 {
    font-family: 'Manrope';
    max-width: 1030px;
    font-weight: 800;
    font-size: 80px;
    line-height: 110%;
    letter-spacing: -0.04em;
    padding-bottom: 29px;
  }
  p {
    font-family: 'Manrope';
    max-width: 710px;
    font-weight: 400;
    font-size: 24px;
    line-height: 34px;
    color: rgba(255, 255, 255, 0.8);
    padding-bottom: 48px;
}
}
// style for email
form.example input[type=text] {
  position: relative; 
  width: 430px;
  height: 80px;
  font-size: 16px;
  background: transparent;
  border: 2px solid #EAEAEA;
  border-radius: 100px;
  float: right;
}
form.example input::placeholder {
  color: #fff;
  padding-left: 23px;
}
/* Style the submit button */
.btn-join {
  width: 191px;
  margin: 8px 8px 8px 230px;
  padding: 24px 18px;
  background: #FF00E5E5;
  color: white;
  font-size: 17px;
  border-radius: 100px;
  cursor: pointer;
}
.btn-position {
  position: absolute;
}
.btn-join:hover {
  background: #b309a2e5;
}


/* Clear floats */
form.example::after {
  content: "";
  clear: both;
  display: table;
}

.figure {
  padding-top: 15px;
}
.shadow {
  // z-index: -10;
  position: absolute;
width: 600px;
height: 600px;
// left: 131px;
background: linear-gradient(270.77deg, #7000FF 26.72%, #AE2727 73.69%);
box-shadow: inset 0px 36px 76px rgba(255, 0, 229, 0.7);
filter: blur(170px);
}
.elipse {
  // z-index: 100;
  border: 1px solid rgba(255, 0, 229, 0.7);
  width: 650px;
height: 650px;
border-radius: 50% 50% 0 0;
border-top: 1px solid rgba(255, 0, 229, 0.7);
background: linear-gradient(53.86deg, #120D13 51.83%, #000000 88.66%);
box-shadow: inset 0px 36px 76px rgba(255, 0, 229, 0.7);
}
// .elipse {
//   /* Create the circle */
//   width: 600px;
//   height: 600px;
//   border: 1px solid rgba(255, 0, 229, 0.7);
//   background: linear-gradient(53.86deg, #120D13 51.83%, #000000 88.66%);
//   border-radius: 50%;
//   /* Halve the circle */
//   border-bottom-color: transparent;
//   border-left-color: transparent;
//   /* Rotate the circle */
//   transform: rotate(-45deg);
// }
</style>
