<template>
  <form class="example" action="/action_page.php" style="margin:auto;max-width:436px">
  <input type="text" placeholder="Your email address" name="search2">
  <a type="submit">Join our community</a>
</form>
</template>
<script>
import { defineComponent } from '@vue/composition-api'

export default defineComponent({
  setup() {
    
  },
})
</script>


<style lang="scss">
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
form.example a {
  position: absolute;
  width: 191px;
  margin: 8px 8px 8px 230px;
  padding: 24px 18px;
  background: #FF00E5E5;
  color: white;
  font-size: 17px;
  border-radius: 100px;
  cursor: pointer;
}

form.example a:hover {
  background: #0b7dda;
}


/* Clear floats */
form.example::after {
  content: "";
  clear: both;
  display: table;
}
</style>