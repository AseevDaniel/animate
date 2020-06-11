<template>
  <div id="app">



    <div class="preloader">
      <div class="preloader__row">
        <div class="preloader__item"></div>
        <div class="preloader__item"></div>
      </div>
    </div>
    <div id="header">
      <div
       class="logo"
       data-aos="fade-down"
       data-aos-delay="400"
       data-aos-duration="2000"
       ata-aos-anchor-placement="right-left"
     >
     <img src="./assets/logo.svg">
     </div>

     <div class="title">
       <div class="space">
         <div data-aos="fade-right"
         data-aos-delay="350"
         data-aos-duration="2000"
         ata-aos-anchor-placement="right-left"
         >
           <span>S</span>
         </div>
         <div data-aos="fade-right"
         data-aos-delay="300"
         data-aos-duration="2000"
         ata-aos-anchor-placement="right-left"
         >
           <span>P</span>
         </div>
         <div data-aos="fade-right"
         data-aos-delay="250"
         data-aos-duration="2000"
         ata-aos-anchor-placement="right-left"
         >
           <span>A</span>
         </div>
         <div data-aos="fade-right"
         data-aos-delay="200"
         data-aos-duration="2000"
         ata-aos-anchor-placement="right-left"
         >
           <span>C</span>
         </div>
         <div data-aos="fade-right"
         data-aos-delay="150"
         data-aos-duration="2000"
         ata-aos-anchor-placement="right-left"
         >
           <span>E</span>
         </div>
       </div>
       <h2 @click="reload()">RELOAD</h2>
       <div class="whale">
         <div data-aos="fade-right"
         data-aos-delay="600"
         data-aos-duration="2000"
         ata-aos-anchor-placement="right-left"
         >
           <span>W</span>
         </div>
         <div data-aos="fade-right"
         data-aos-delay="650"
         data-aos-duration="2000"
         ata-aos-anchor-placement="right-left"
         >
           <span>H</span>
         </div>
         <div data-aos="fade-right"
         data-aos-delay="700"
         data-aos-duration="2000"
         ata-aos-anchor-placement="right-left"
         >
           <span>A</span>
         </div>
         <div data-aos="fade-right"
         data-aos-delay="750"
         data-aos-duration="2000"
         ata-aos-anchor-placement="right-left"
         >
           <span>L</span>
         </div>
         <div data-aos="fade-right"
         data-aos-delay="800"
         data-aos-duration="1800"
         ata-aos-anchor-placement="right-left"
         >
           <span>E</span>
         </div>
       </div>
     </div>

     <div id="triger" class="circle"
     data-aos="fade-up"
     data-aos-delay="1000"
     data-aos-duration="1200">
     </div>
    </div>
    <div >

    </div>
    <div class="menu"
         data-aos="fade-down"
         data-aos-anchor="#triger"
         data-aos-duration="1000"
         data-aos-anchor-placement="top-top">
         <img src="./assets/logo.svg" alt="">
      <ul>
        <a href="#"><li>Home</li></a>
        <a href="#"><li>About us</li></a>
        <a href="#"><li>Projects</li></a>
        <a href="#"><li>Contacts</li></a>
      </ul>
    </div>

    <div id="content">
      <div
        class="content-text"
        data-aos="fade-right"
        data-aos-offset="100"
        data-aos-delay="100"
        data-aos-duration="1000"
        data-aos-easing="ease-in-out"
        data-aos-mirror="true"
        data-aos-once="false"
      >
      <p>Lorem ipsum dolor sit amet</p>
      </div>
      <div
        class="content-text"
        data-aos="flip-up"
      >
      <p>Lorem ipsum dolor sit amet</p>
      </div>
      <div
        class="content-text"
        data-aos="zoom-in-down"
      >
      <p>Lorem ipsum dolor sit amet</p>
      </div>
      <div
        class="anim-text"
        data-aos="zoom-out"
        data-aos-offset="50"
      >
      <p>Lorem ipsum dolor sit amet</p>
      </div>
    </div>
  </div>
</template>

<script>
window.onload = function () {
    document.body.classList.add('loaded_hiding');
    window.setTimeout( () => {
      document.body.classList.add('loaded');
      document.body.classList.remove('loaded_hiding');
    }, 500);
  }
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  methods: {
    reload(){
      location.reload()
    }
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700&display=swap');
@import './style/keyframes.scss';
@import './style/loader.scss';
@import './style/header.scss';
@import './style/content.scss';

body{
  overflow-x: hidden;
    background: #222;
    margin: 0;
    padding: 0;
    font-family: 'Montserrat', 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #fff;
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
  margin: 0 10px;
}

</style>
