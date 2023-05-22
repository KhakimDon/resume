<script setup>
import Links from "../components/Links.vue";
import Progress from "../components/Progress.vue";
</script>

<template>
  <div>
    <!-- <TheWelcome /> -->
    <div class="min-h-[100vh] bg-[black] pt-[50px] pb-[50px]">
      <div
        class="w-[100%] bg-[black] flex flex-col justify-between max-w-[1820px] mx-[auto]"
      >
        <div class="w-[100%] fixed z-[20] max-w-[1820px] flex justify-between items-center">
          <figure>
            <img src="../assets/log.png" alt="" />
          </figure>

          <div>
            <router-link to="/">
            <p
              class="font-[Neue] cur hover:text-[#7AF37C] duration-[.3s] font-[600] text-[40px] break-word text-right text-[white]"
            >
              ALMAMEDOV <br />
              <span class="font-[1000]">KHAKIM</span>
            </p>
          </router-link>
          </div>
        </div>

        <div class="absolute items right-[350px] top-[0]">
            <div class="item"></div>
            <div class="item"></div>
            <div class="item"></div>
            <div class="item"></div>
            <div class="item"></div>
            <div class="item"></div>
          </div>



        <div class="mt-[200px]  z-[100] border-solid border-[1px] border-[silver] h-[700px] mx-[auto] w-[1100px] ">
          <div class="aboutBg h-[130px] bg-[black] pl-[70px]">
            <span class="font-[700] text-white text-[80px] z-[10]"
              >ABOUT ME</span
            >
          </div>
          <div class="flex">
            <div class="figure">
              <img src="../assets/Image (7).png" alt="">
            </div>
            <div class="pack">
              <img src="../assets/Image (9).png" alt="">
            </div>
          </div>
          </div>

          <div class="w-[1100px] z-[10] mx-[auto] mt-[280px]">
            <p class="text-[30px] text-white font-[600]">
              Connor, also known as Crypto Chad, is a dynamic individual with a diverse set of passions and expertise. As a visual designer, he specializes in creating stunning user interface designs for mobile apps and websites. In addition to his professional pursuits, Connor is an avid fitness enthusiast, with a love for the gym and staying physically fit. His entrepreneurial spirit has led him to launch multiple businesses in the mobile app and e-commerce space, and he's also a spiritual and psychedelic enthusiast who has delved into meditation and kundalini yoga. To top it all off, he's also a talented house and EDM DJ, using music as a way to express himself and connect with others.
            </p>

            <Progress/>
          </div>




      </div>
    </div>
    <Links  />
  </div>
</template>


<style scoped>

.item{
  background: radial-gradient(#F700F5,rgba(0, 0, 255, 0));
  box-shadow: 0 0 20px #F700F5, inset 0 0 20px #F700F5;
  border: 10px solid #F700F5; 
}
.item:nth-child(2){
  background: radial-gradient(#0003E1,rgba(0, 0, 255, 0));
  box-shadow: 0 0 20px #0003E1, inset 0 0 20px #0003E1;
  border: 10px solid #0003E1; 
}
.item:nth-child(3){
  background: radial-gradient(#7AF37C,rgba(0, 0, 255, 0));
  box-shadow: 0 0 20px #7AF37C, inset 0 0 20px #7AF37C;
  border: 10px solid #7AF37C; 
}
.item:nth-child(4){
  background: radial-gradient(#EFEB00,rgba(0, 0, 255, 0));
  box-shadow: 0 0 20px #EFEB00, inset 0 0 20px #EFEB00;
  border: 10px solid #EFEB00; 
}
.item:nth-child(5){
  background: radial-gradient(#F97F02,rgba(0, 0, 255, 0));
  box-shadow: 0 0 20px #F97F02, inset 0 0 20px #F97F02;
  border: 10px solid #F97F02; 
}
.item:nth-child(6){
  background: radial-gradient(#E40037,rgba(0, 0, 255, 0));
  box-shadow: 0 0 20px #E40037, inset 0 0 20px #E40037;
  border: 10px solid #E40037; 
}
.items{
  top: -100px;
}
.item{
  height: 200px;
  margin-bottom: 50px;
  width: 200px;
  border-radius: 100%;
}
.pack{
  height: 570px;
  backdrop-filter: blur(10px);
  flex: 1;
  position: relative;
  width: 100%;
  border-bottom: 1px solid silver;
  background-image: url("../assets/2.png");
  background-size: cover;
}
.pack img{
    position: absolute;
    left: -200px;
    bottom: -200px;
}
.figure{
  width: 660px;
  height: 570px;
}
.figure img {
  height: 100% !important;
  width: 100% !important;
  object-fit: cover;
}
.aboutBg {
  background-image: url("../assets/aboutbg.png");
  background-size: cover;
  position: relative;
  z-index: 2;
  background-position: center center;
}
.aboutBg::after {
  height: 100%;
  left: 0;
  top: 0;
  z-index: -1;
  width: 100%;
  content: "";
  background: rgba(0, 0, 0, 0.173);
  position: absolute;
}
</style>
