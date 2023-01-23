<template>
  <div class="header">
    <div class="container">
      <div class="header-content">
        <div class="logo">
          <img :src="Dollar" class="logo">
        </div>
        
        <nav class="header-nav">
          <ul>
            <li><a href="">Licence</a></li>
            <li><a href="">About us</a></li>
            <li><a href="">How to start</a></li>
          </ul>
          <a class="header-btn btn" href="#">Join us</a>
        </nav>
     </div>
   </div>
  </div>
</template>
<script>
import Dollar from '@/assets/logo.png'
export default {
  setup () {
    return {
      Dollar
    }
  }
}
</script>

<style lang="scss">
.header {
  padding-top: 14px;
  // padding-bottom: 39px;
  
  }
  .header-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-bottom: 2px solid rgba(255, 255, 255, 0.06);
    padding-bottom: 1rem;
  }
  .header-nav {
    display: flex;
    // margin-left: 576px;

    ul {
      display: flex;
      align-items: center;
      justify-content: space-between;
     
      li {
        a {
          font-weight: 400;
          font-size: 18px;
          line-height: 120%;
          color: rgba(255, 255, 255, 0.92);
        }
      }
       
      li + * {
        padding-left: 40px;

      }
    }
 
  }
  .header-btn {
    color: #FF00E5;
    width: 103px;
    height: 50px;
    background: rgba(255, 255, 255, 0.08);
    border-radius: 56px;
    display: flex;
    align-items: center;
    justify-content: center;
    margin-left: 40px;
  }


</style>