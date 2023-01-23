<template>
  <div class="footer">
    <div class="container">
      <div class="footer-content">
      <div class="footer-contact">
        <div class="footer-icons">
          <a href="https://www.facebook.com/" class="footer-icons_position" target="_blank"><img :src="Facebook" alt="Facebook"></a>
          <a href="https://t.me/v_dyakovich" class="footer-icons_position" target="_blank"><img :src="Telegram" alt="Telegram"></a>
          <a href="https://www.instagram.com/" class="footer-icons_position" target="_blank"><img :src="Instagram" alt="Instagram"></a>
          <a href="https://twitter.com/" class="footer-icons_position" target="_blank"><img :src="Twitter" alt="Twitter"></a>
        </div>
        <h4>“The one who owns the information — owns the world!”</h4>
          <div class="footer-container">
          <span class="footer-nav">
            <img :src="location" alt="location">
            Los Angeles, Lamen St. 45, 23-000
          </span>
          <span class="footer-nav">
            <img :src="call" alt="call">
            +8-567-283-9983
          </span>
          <span class="footer-nav">
            <img :src="mail" alt="mail">
            cucoin@gmail.com
          </span>
        </div>
      </div>
      <div class="footer-join">
        <h3>Join our community</h3>
        <form @submit.prevent="formSubmit" >
          <input type="text" v-model="name" class="footer-log" :placeholder="inputOne" required>
          <input type="text" v-model="surname" class="footer-log" :placeholder="inputSecond" required>
          <input type="email" v-model="email" class="footer-log" :placeholder="clue" required>
          <button class="footer-btn" type="submit" @click="formSubmit">Sign up</button>
        </form>
      </div>
    </div>
    </div>
  </div>
</template>
<script>
import Facebook from '@/assets/Facebook.svg'
import Instagram from '@/assets/instagram.svg'
import Telegram from '@/assets/Telegram.svg'
import Twitter from '@/assets/Twitter.svg'
import call from '@/assets/call.svg'
import location from '@/assets/location.svg'
import mail from '@/assets/mail.svg'

export default {
   data() {
    return {
      Facebook,
      Telegram,
      Instagram,
      Twitter,
      mail,
      location,
      call,
      
      name: '',
      surname: '',
      email: "",
      clue: "Email",
      inputOne: "Name",
      inputSecond: "Surname"
    }
  },
  methods: {
    formSubmit() {
      this.name
      console.log("hi");
    }
  }
  }

</script>
<style lang="scss">
.footer {
  padding-bottom: 5rem;
  .container {
  padding: 0 120px;
}
}

.footer-content {
  display: flex;
  justify-content: space-around;
}
.footer-contact {
  margin-right: 11rem;
  h4 {
    font-weight: 400;
    font-size: 24px;
    line-height: 34px;
    margin-top: 3rem;
    margin-bottom: 52px;
  }
}
.footer-icons {
  display: flex;
}
.footer-icons_position + * {
  margin-left: 2rem;
}
.footer-container {
  display: flex;
  flex-direction: column;
}
.footer-nav {
  display: flex;
  align-items: center;
  font-weight: 700;
  font-size: 16px;
  line-height: 20px;
  margin-bottom: 2rem;
  img {
    margin-right: 0.9rem;
    background: rgba(0, 0, 0, 0);
  }
}
.footer-join {
  display: flex;
  flex-direction: column;
  align-items: flex-start;

  input, textarea {
    // outline: none;
    border-top: none;
    border-left: none;
    border-right: none;
    border-bottom: 1px solid #FFFFFF;
    background: transparent;
  }

    .footer-btn {
      background: #FF00E5E5;
      color: white;
      font-size: 17px;
      border-radius: 100px;
      padding: 23px 30px;
      text-align: center;
      cursor: pointer;
      margin-top: 3rem;
    }
    .footer-btn:hover {
      background: #b309a2e5;
    }
  h3 {
    font-weight: 800;
    font-size: 48px;
    line-height: 60px;
    margin-bottom: 3rem;
    white-space: nowrap;
  }
}
.footer-log {
  margin-right: 1.5rem;
  color: #FFFFFF;
  &:last-child {
    margin-top: 50px;
  }
}
.footer-btn {
  
}

@media (max-width: 1000px) {
  .container {
    padding: 0 100px;
  }
  .footer {
  padding-bottom: 4rem;
  .container {
  padding: 0 120px;
}
}

.footer-content {
  display: flex;
  justify-content: space-around;
}
.footer-contact {
  margin-right: 11rem;
  h4 {
    font-weight: 400;
    font-size: 24px;
    line-height: 34px;
    margin-top: 3rem;
    margin-bottom: 52px;
  }
}
.footer-icons {
  display: flex;
}
.footer-icons_position + * {
  margin-left: 2rem;
}
.footer-container {
  display: flex;
  flex-direction: column;
}
.footer-nav {
  display: flex;
  align-items: center;
  font-weight: 700;
  font-size: 16px;
  line-height: 20px;
  margin-bottom: 2rem;
  img {
    margin-right: 0.9rem;
    background: rgba(0, 0, 0, 0);
  }
}
.footer-join {
  display: flex;
  flex-direction: column;
  align-items: flex-start;

  input, textarea {
    // outline: none;
    border-top: none;
    border-left: none;
    border-right: none;
    border-bottom: 1px solid #FFFFFF;
    background: transparent;
  }

    .footer-btn {
      background: #FF00E5E5;
      color: white;
      font-size: 17px;
      border-radius: 100px;
      padding: 23px 30px;
      text-align: center;
      cursor: pointer;
      margin-top: 3rem;
    }
    .footer-btn:hover {
      background: #b309a2e5;
    }
  h3 {
    font-weight: 800;
    font-size: 30px;
    line-height: 60px;
    margin-bottom: 3rem;
    white-space: nowrap;
  }
}
.footer-log {
  margin-right: 1.5rem;
  color: #FFFFFF;
  &:last-child {
    margin-top: 50px;
  }
}
.footer-btn {
  
}
}
</style>