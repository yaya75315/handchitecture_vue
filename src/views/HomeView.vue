<template>
  <nav
    class="noto-sans flex items-center fixed left-0 right-0 z-10 bg-white/75 h-[58px] backdrop-blur-[10px] px-4 py-2">
    <div class="sm:max-w-[1080px] w-full flex items-center justify-between mx-auto">
      <div class="flex items-center gap-3">
        <img class="w-[50px]" src="../assets/images/LOGO.svg" alt="" />
        <p class="text-[#2A2A2A] font-medium tracking-[10px] text-sm">
          手建築研究所
        </p>
      </div>
      <div v-if="clientWidth < 560" class="hamburger" :class="{ open: menuStatus }" @click="menuStatus = !menuStatus">
        <span></span>
        <span class="circle"></span>
        <span></span>
      </div>
      <ul class="flex items-center text-[#2B2B2B] gap-8 text-sm tracking-[5px]"
        :class="[{ menu: clientWidth < 560 }, { open: menuStatus }]">
        <li>關於手建築</li>
        <li>團隊介紹</li>
        <li>殼計畫</li>
      </ul>
    </div>
  </nav>
  <section class="mt-[58px] inline-block w-full">
    <div class="">
      <div 
        class="key-vision blur-[2px] sm:blur-none noto-serif absolute left-0 h-[calc(100vh-58px)] w-full lg:w-[calc(100%-300px)] bg-slate-100 overflow-hidden">
        <div ref="baseCoverRef" class="key-vision-base absolute w-full h-full">
          <img class="w-full h-full object-cover" src="../assets/images/base.png" alt="" />
        </div>
        <div ref="middleCoverRef" class="key-vision-text">
          <p
            class="tracking-[20px] lg:tracking-[60px] font-bold text-[30px] md:text-[42px] text-[#313131] align-middle">
            手建築研究所
          </p>
          <p class="text-[12px] md:text-[20px] tracking-[6px] lg:tracking-[14.5px] pl-1 text-[#313131] font-bold">
            Handchitecture Gallery
          </p>
        </div>
        <div ref="topCoverRef" class="key-vision-shadow absolute w-full h-full">
          <img class="w-full h-full object-cover" src="../assets/images/shadow.png" alt="" />
        </div>
      </div>
      <div  ref="titleCoverRef"
        class="key-text absolute right-6 md:right-40 top-[34vh] whitespace-nowrap lg:top-[30vh] chenyuluoyan tracking-[3px] text-[30px] text-[#343434]">
        <p class="mt-20">親手創造夢想住宅的旅途</p>
        <p>這是一趟屬於您與家人，</p>
      </div>
    </div>
    <div class="lg:px-0 block mt-[calc(100vh+65px)] noto-sans">
      <!-- 關於手建築 -->
      <div class="about-us bg-[#CABFB3]/10">
        <AboutUs />
      </div>
      <!-- 團隊介紹 -->
      <MemberIntro :clientWidth="clientWidth" />
      <!-- 殼計畫 -->
      <div class=" bg-[#CABFB3]/10 pb-16">
        <HousingPlan />
        <!-- 導引按鈕 -->
        <div class="px-4 mt-32 max-w-[920px] mx-auto text-center flex flex-col items-center gap-7">
          <button
            class="max-w-[600px] w-full text-white py-3 tracking-[5px] text-[22px] bg-[#484848] rounded-[10px] hover:bg-[#813B31] transition-colors">了解更多</button>
          <button
            class="text-[#968E85] hover:text-[white] hover:bg-[#968E85] text-xs px-6 py-2 rounded-[5px] border border-[#968E85] tracking-[2px] transition-colors">申請加入手建築</button>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref, onMounted } from "vue";
import AboutUs from "@/components/AboutUs.vue"
import MemberIntro from "@/components/MemberIntro.vue"
import HousingPlan from "@/components/HousingPlan.vue"
import { gsap } from 'gsap';
import { ScrollTrigger } from "gsap/ScrollTrigger";

// 判斷navigation bar menu狀態
// menuStatus false=關閉菜單, true=開啟菜單
const menuStatus = ref(false);
// clientWidth 監聽目前裝置寬度，以判斷是否顯示hamburger
const clientWidth = ref(null);
const baseCoverRef = ref(null) 
const middleCoverRef = ref(null) 
const topCoverRef = ref(null) 
const titleCoverRef = ref(null)
const scrollY = ref(null)

clientWidth.value = window.innerWidth;
gsap.registerPlugin(ScrollTrigger);
onMounted(() => {
  // 監聽網頁寬度
  window.addEventListener("resize", () => {
    clientWidth.value = window.innerWidth;
    console.log(clientWidth.value);
  });

  gsap.from('.key-vision', { opacity: 0, duration: 3,x:-100 ,ease: "power3"});
  gsap.from('.key-text', { opacity: 0, duration: 3,x:+200,y:100 ,ease: "power3" });

  // 監聽元素初始位置
  console.log(baseCoverRef.value)
  const baseCoverParallax = baseCoverRef.value.getBoundingClientRect().top;
  const middleCoverParallax = middleCoverRef.value.getBoundingClientRect().top;
  const topCoverParallax = topCoverRef.value.getBoundingClientRect().top;
  const rightTitleParallax = titleCoverRef.value.getBoundingClientRect().top;
  console.log('baseCoverParallax:',baseCoverParallax)

  // 在滾動事件中更新元素位置
  window.addEventListener('scroll', () => {
      scrollY.value = window.scrollY;
      console.log(scrollY.value)
      gsap.to(topCoverRef.value, {
        x: Math.min(scrollY.value * 0.2, 200) , // 根據滾動位置計算元素的新位置
        duration: 2, // 持續時間
      });

      gsap.to(middleCoverRef.value, {
        y: scrollY.value * 0.01, // 根據滾動位置計算元素的新位置
        duration: 1, // 持續時間
      });

      gsap.to(titleCoverRef.value, {
        y: Math.min(scrollY.value * 0.3,150), // 根據滾動位置計算元素的新位置
        duration: 0.5, // 持續時間
      });
    });
});
</script>

<style scoped>
nav{
  transition: font 0.3s ease-in;
}

nav ul li {
  cursor: pointer;
  padding-top: 5px;
  padding-bottom: 5px;
  padding-left: 5px;
  border-bottom: 0.5px solid transparent;
  transition: border 0.3s ease-in-out;
}

nav ul li:hover {
  border-bottom: 0.5px solid #434343;
}

.key-vision {
  transition: width 0.3s ease-in-out;
}

.key-vision-text {
  position: absolute;
  left: 60%;
  top: 50%;
  transform: translate(-60%, -50%);
  white-space: nowrap;
  transition: top 0.3s ease-in-out;
}

.key-vision-text p {
  transition: letter-spacing 0.3s ease-in-out, font-size 0.3s ease-in-out;
}

.key-text {
  transition: top 0.3s ease-in-out;
}

.key-vision-shadow {
  transform: scale(1.3);
}

.key-text {
  -webkit-writing-mode: vertical-lr;
  writing-mode: vertical-lr;
}

.hamburger {
  cursor: pointer;
  background-color: transparent;
  width: 26px;
  height: 30px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 3px;
  align-content: center;
}

.hamburger span {
  display: block;
  width: 20px;
  height: 2.5px;
  border-radius: 99px;
  background-color: #813b31;
}

.hamburger span.circle {
  height: 2.5px;
  width: 12px;
}

.hamburger span:not(:last-child) {
  margin-bottom: 4px;
}

.hamburger span:nth-child(2) {
  margin-left: auto;
  transition: background-color 0.25s, transform 0.3s;
}

.hamburger span:nth-child(1),
.hamburger span:nth-child(3) {
  transition: transform 0.45s, background-color 0.25s;
}

.hamburger.open {
  z-index: 1000;
}

.hamburger.open span {
  background-color: #fff;
}

.hamburger.open span:nth-child(2) {
  transform: translateX(20px) rotate(270deg);
  background-color: transparent !important;
}

.hamburger.open span:nth-child(1) {
  transform: translate(0%, 6px) rotate(315deg);
}

.hamburger.open span:nth-child(3) {
  transform: translate(0%, -7px) rotate(-315deg);
}

.menu {
  position: absolute;
  white-space: nowrap;
  top: 0;
  display: block;
  background: #000;
  width: 100%;
  left: 0;
  height: 100vh;
  color: #fff;
  text-align: center;
  padding-top: 30vh;
  opacity: 0.8;
  transform: translateX(-100%);
  transition: transform 0.3s ease-in-out;
}

.menu li {
  width: 100%;
  font-size: 18px;
  padding: 20px 20px;
  border: none;
  margin: 20px 0;
}

.menu li:hover {
  background: #fff;
  color: #813b31;
  border: none;
  font-weight: 600;
}

.menu.open {
  transform: translateX(0);
}

@media (max-width: 850px) {
  .key-text {
    top: 60%;
  }
}

@media (max-width: 600px) {
  .key-vision-text {
    top: 40%;
  }

  .key-text {
    top: 50%;
  }

  .key-vision-shadow {
    transform: scale(2.3);
  }
}
</style>
