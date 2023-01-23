<template>
  <nav>
    <!-- <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> -->
  </nav>
  <router-view/>
</template>
  
<style lang="scss">
#app {
 
  // -webkit-font-smoothing: antialiased;
  // -moz-osx-font-smoothing: grayscale;
  color: #ffffff;
  background-color: #000;
  
  box-sizing: border-box;
  
}

*, *:before, *:after{
    box-sizing: border-box;
}

html, body, div, span, object, iframe, figure, h1, h2, h3, h4, h5, h6, p, blockquote, pre, a, code, em, img, small, strike, strong, sub, sup, tt, b, u, i, ol, ul, li, fieldset, form, label, table, caption, tbody, tfoot, thead, tr, th, td, main, canvas, embed, footer, header, nav, section, video{
    margin: 0;
    padding: 0;
    border: 0;
    font-size: 100%;
    

    font: inherit;
    vertical-align: baseline;
    text-rendering: optimizeLegibility;
    -webkit-font-smoothing: antialiased;
    text-size-adjust: none;

}
a {
  text-decoration: none;
  color: #ffffff;
}
 header, nav, section, main{
    display: block;
}

body{
    line-height: 1;
    @import url('https://fonts.googleapis.com/css2?family=Manrope:wght@400;800&family=Montserrat:wght@400;700&family=Poppins:wght@400;700&display=swap');
    font-family: 'Manrope', sans-serif;
    
}

ol, ul{
    list-style: none;
}

blockquote, q{
    quotes: none;
}

blockquote:before, blockquote:after, q:before, q:after{
    content: '';
    content: none;
}

table{
    border-collapse: collapse;
    border-spacing: 0;
}

input{
    -webkit-appearance: none;
    border-radius: 0;
}
.container {
    padding: 0 135px;
    font-family: 'Manrope', sans-serif;
    overflow: hidden;
}
</style>
