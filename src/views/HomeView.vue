<script setup>
import TheWelcome from "../components/TheWelcome.vue";
import Links from "../components/Links.vue";
</script>

<template>
  <main>
    <!-- <TheWelcome /> -->
    <div class="h-[100vh] bg-[black] pt-[50px] pb-[50px]">
      <div
        class="h-[100%] w-[100%] bg-[black] flex flex-col justify-between max-w-[1820px] mx-[auto]"
      >
        <div class="w-[100%] flex justify-between items-center">
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
        <div
          class="rotate-[90deg] w-[400px] absolute right-[-130px] top-[50%] flex justify-between"
        >
          <router-link to="/about"
            class="text-white text-[22px] cursor-pointer hover:text-[orange] duration-[.5s] font-[600 ]"
            >ABOUT</router-link
          >
          <router-link to="/projects"
            class="text-white text-[22px] cursor-pointer hover:text-[orange] duration-[.5s] font-[600 ]"
            >PROJECTS</router-link
          >
          <span
            class="text-white text-[22px] cursor-pointer hover:text-[orange] duration-[.5s] font-[600 ]"
            >RESUME</span
          >
        </div>
        <div class="w-[100%] flex justify-between items-center min-h-[40px]">
          <p class="text-[white] font-[600] text-[30px]">
            Frontend Developer <br />
            <span class="text-[#C0C0C0] text-[26px] font-[400] mr-[10px]"
              >From</span
            >
            <span class="text-[28px] text-[#EFEB00]">Liberty Code</span>
          </p>
          <div class="flex">
            <img class="ml-[30px]" src="../assets/inst.png" alt="" />
            <img class="ml-[30px]" src="../assets/inst.png" alt="" />
            <img class="ml-[30px]" src="../assets/inst.png" alt="" />
            <img class="ml-[30px]" src="../assets/inst.png" alt="" />
          </div>
        </div>
      </div>
    </div>

    <div
      class="animate h-[100vh] w-[300px] z-[10] absolute top-[-150px] left-[50%] translate-x-[-50%]"
    >
      <div class="block">
        <div class="shadow"></div>
      </div>
      <div class="block">
        <div class="shadow"></div>
      </div>
      <div class="block">
        <div class="shadow"></div>
      </div>
    </div>

    <Links/>

    <img
      src="../assets/person.png"
      class="absolute bottom-[0] z-[10] h-[75vh] left-[50%] translate-x-[-50%]"
      alt=""
    />
    <span class="text-[150px] pointer-events-none z-[2] w-[100%] text-center text-[#090909] font-[neue] font-[600] top-[50%] translate-x-[-50%] translate-y-[-50%] absolute left-[50%]">
      ALMAMEDOV KHAKIM
    </span>
  </main>
</template>

<style scoped>
.animate {
  width: 600px;
  height: 100vh;
  overflow: hidden;
}
.block {
  width: 300px !important;
  margin: auto;
  height: 300px !important;
  animation-name: identifier1;
  animation-timing-function: linear;
  animation-duration: 50s;
  animation-iteration-count: infinite;
  border-radius: 100%;
  display: flex;
  align-items: center;
  animation-direction: alternate-reverse;
  justify-content: center;
  margin-bottom: 50px;
  border: 15px solid #0003e1;
  box-shadow: 0 0 40px #0003e1, inset 0 0 20px #0003e1;
}
.shadow {
  box-shadow: 0 0 120px 90px #0003e1;
  height: 1px;
  width: 1px;
  animation-name: inner;
  animation-direction: alternate-reverse;
  animation-timing-function: linear;
  animation-duration: 50s;
  animation-iteration-count: infinite;
}
.block:nth-child(2) {
  animation-name: identifier21 !important;
  animation-timing-function: linear;
  animation-duration: 80s;
  animation-direction: normal;
  animation-iteration-count: infinite;
  border: 15px solid #7af37c;
  box-shadow: 0 0 40px #7af37c, inset 0 0 20px #7af37c;
}

.block:nth-child(2) .shadow {
  box-shadow: 0 0 120px 90px #7af37c;
  animation-name: inner2;
  animation-direction: normal;
  animation-timing-function: linear;
  animation-duration: 80s;
  animation-iteration-count: infinite;
}
.block:nth-child(1) {
  animation-name: identifier1;
  animation-timing-function: linear;
  animation-duration: 115s;
  animation-direction: normal;
  animation-iteration-count: infinite;
  border: 15px solid #e40037;
  box-shadow: 0 0 40px #e40037, inset 0 0 20px #e40037;
}
.block:nth-child(1) .shadow {
  animation-name: inner;
  animation-direction: normal;
  animation-timing-function: linear;
  animation-duration: 115s;
  animation-iteration-count: infinite;
  box-shadow: 0 0 120px 90px #e40037;
}
@keyframes identifier1 {
  0% {
    border: 15px solid #e40037;
    box-shadow: 0 0 40px #e40037, inset 0 0 20px #e40037;
  }
  12% {
    border: 15px solid #f97f02;
    box-shadow: 0 0 40px #f97f02, inset 0 0 20px #f97f02;
  }
  24% {
    border: 15px solid #efeb00;
    box-shadow: 0 0 40px #efeb00, inset 0 0 20px #efeb00;
  }
  36% {
    border: 15px solid #7af37c;
    box-shadow: 0 0 40px #7af37c, inset 0 0 20px #7af37c;
  }
  48% {
    border: 15px solid #0003e1;
    box-shadow: 0 0 40px #0003e1, inset 0 0 20px #0003e1;
  }
  60% {
    border: 15px solid #f700f5;
    box-shadow: 0 0 40px #f700f5, inset 0 0 20px #f700f5;
  }
  72% {
    border: 15px solid #e40037;
    box-shadow: 0 0 40px #e40037, inset 0 0 20px #e40037;
  }
}
@keyframes identifier21 {
  0% {
    border: 15px solid #7af37c;
    box-shadow: 0 0 40px #7af37c, inset 0 0 20px #7af37c;
  }
  12% {
    border: 15px solid #f97f02;
    box-shadow: 0 0 40px #f97f02, inset 0 0 20px #f97f02;
  }
  24% {
    border: 15px solid #efeb00;
    box-shadow: 0 0 40px #efeb00, inset 0 0 20px #efeb00;
  }
  36% {
    border: 15px solid #7af37c;
    box-shadow: 0 0 40px #7af37c, inset 0 0 20px #7af37c;
  }
  48% {
    border: 15px solid #0003e1;
    box-shadow: 0 0 40px #0003e1, inset 0 0 20px #0003e1;
  }
  60% {
    border: 15px solid #f700f5;
    box-shadow: 0 0 40px #f700f5, inset 0 0 20px #f700f5;
  }
  72% {
    border: 15px solid #e40037;
    box-shadow: 0 0 40px #e40037, inset 0 0 20px #e40037;
  }
}

@keyframes inner2 {
  0% {
    box-shadow: 0 0 120px 90px #7af37c;
  }
  12% {
    box-shadow: 0 0 120px 90px #f97f02;
  }
  24% {
    box-shadow: 0 0 120px 90px #efeb00;
  }
  36% {
    box-shadow: 0 0 120px 90px #7af37c;
  }
  48% {
    box-shadow: 0 0 120px 90px #0003e1;
  }
  60% {
    box-shadow: 0 0 120px 90px #f700f5;
  }
  72% {
    box-shadow: 0 0 120px 90px #e40037;
  }
}
@keyframes inner {
  0% {
    box-shadow: 0 0 120px 90px #e40037;
  }
  12% {
    box-shadow: 0 0 120px 90px #f97f02;
  }
  24% {
    box-shadow: 0 0 120px 90px #efeb00;
  }
  36% {
    box-shadow: 0 0 120px 90px #7af37c;
  }
  48% {
    box-shadow: 0 0 120px 90px #0003e1;
  }
  60% {
    box-shadow: 0 0 120px 90px #f700f5;
  }
  72% {
    box-shadow: 0 0 120px 90px #e40037;
  }
}


.cur:hover {
  cursor: url("../assets/hr.png"), pointer !important;
}

h1 {
  font-family: Neue;
}
</style>
