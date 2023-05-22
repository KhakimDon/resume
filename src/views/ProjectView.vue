<script setup>
import Links from "../components/Links.vue";
</script>


<template>
  <div>
    <!-- <TheWelcome /> -->
    <div class="min-h-[100vh] bg-[black] pt-[50px] pb-[50px]">
      <div
        class="w-[100%] bg-[black] flex flex-col justify-between max-w-[1820px] mx-[auto]"
      >
        <div
          class="w-[100%] fixed z-[20] max-w-[1820px] flex justify-between items-center"
        >
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

        <div class="w-[1100px] z-[10] mx-[auto] mt-[130px]">
          <div class="flex mb-[150px] justify-center">
            <img src="../assets/project.png" alt="" />
          </div>

          <div class="w-[100%] mb-[80px] h-[578px]   flex items-center">
            <div
              class="w-[150px] flex justify-center text-white text-[50px] font-[neue] items-center h-[110px] border-[solid] border-white border-[1px]"
            >
              01
            </div>

            <div class="mx-[30px] h-[100%] w-[400px] bg-[aqua]">
              <img
                class="h-[100%] w-[100%] object-cover"
                src="../assets/applepro.png"
                alt=""
              />
            </div>

            <div class="h-[100%] bg-[#1C1C1C] flex-[1] p-[43px]">
              <img class="h-[97px]" src="../assets/apple.png" alt="" />
              <p class="mt-[26px] mb-[30px] text-[20px] text-white  ">#1 Web3 Wellness App on App Store</p>
              <h2 class="text-[45px] font-[neue] text-white font-[600]">Zenbase Meditation With Crypto Rewards</h2>
              <p class="text-[#C0C0C0] mt-[30px]">
                <button class="bg-[#333] h-[80px] w-[250px] text-[23px] hover:border-[solid] hover:border-[1px] hover:border-[silver]">
                    VIEW WEBSITE...
                </button>
              </p>
            </div>
          </div>
          <div class="w-[100%] mb-[80px] h-[578px]   flex items-center">
            <div
              class="w-[150px] flex justify-center text-white text-[50px] font-[neue] items-center h-[110px] border-[solid] border-white border-[1px]"
            >
              02
            </div>

            <div class="mx-[30px] h-[100%] w-[400px] bg-[aqua]">
              <img
                class="h-[100%] w-[100%] object-cover"
                src="../assets/googlepro.png"
                alt=""
              />
            </div>

            <div class="h-[100%] bg-[#1C1C1C] flex-[1] p-[43px]">
              <img class="h-[97px]" src="../assets/google.png" alt="" />
              <p class="mt-[26px] mb-[30px] text-[20px] text-white  ">Free Google Chrome Extension</p>
              <h2 class="text-[45px] font-[neue] text-white font-[600]">  Amazon True Reviews
Reddit Comments</h2>
              <p class="text-[white] mt-[30px]">
                <button class="bg-[#333] h-[80px] w-[250px] text-[23px] hover:border-[solid] hover:border-[1px] hover:border-[silver]">
                    VIEW WEBSITE...
                </button>
              </p>
            </div>
          </div>


        </div>

        
    </div>
</div>
<Links />
</div>
</template>

<script>
export default {};
</script>

<style>
</style>