<template>
  <nav
    class="noto-serif flex items-center fixed left-0 right-0 z-10 bg-white/10 h-[58px] backdrop-blur-[4px] px-4 py-2">
    <div class="sm:max-w-[1080px] w-full flex items-center justify-between mx-auto">
      <div class="flex items-center gap-3">
        <img class="w-[50px]" src="../assets/images/LOGO.svg" alt="" />
        <p class="text-[#2A2A2A] font-semibold tracking-[10px] text-sm">
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
        <div class="key-vision-base absolute w-full h-full">
          <img class="w-full h-full object-cover" src="../assets/images/base.png" alt="" />
        </div>
        <div class="key-vision-text">
          <p class="tracking-[20px] lg:tracking-[60px] font-bold text-[30px] md:text-[42px] text-[#313131] align-middle">
            手建築研究所
          </p>
          <p class="text-[12px] md:text-[20px] tracking-[6px] lg:tracking-[14.5px] pl-1 text-[#313131] font-bold">
            Handchitecture Gallery
          </p>
        </div>
        <div class="key-vision-shadow absolute w-full h-full">
          <img class="w-full h-full object-cover" src="../assets/images/shadow.png" alt="" />
        </div>
      </div>
      <div
        class="key-text absolute right-6 md:right-40 top-[34vh] whitespace-nowrap lg:top-[30vh] chenyuluoyan tracking-[3px] text-[30px] text-[#343434]">
        <p class="mt-20">親手創造夢想住宅的旅途</p>
        <p>這是一趟屬於您與家人，</p>
      </div>
    </div>
    <div class="px-4 lg:px-0 block mt-[calc(100vh+65px)] noto-sans max-w-[920px] mx-auto">
      <div>
        <div class="big-title text-center py-16">
          <p>關於手建築</p>
        </div>
        <div class="block-content text-base md:text-[18px] tracking-[5px] flex flex-col gap-7  text-justify">
          <p>手建築有限公司創立於2022年11月22日，主要的核心理念為：居住是基本人權，每個人都應當擁有「親手創造住宅」並「安居其中」的權利。</p>
          <p>然而手建築並非「建商」也不會成為「建設公司」，我們提出我們的想法來創造新的自建模式，與其說是模式，手建築更期望成為一場「運動」，一場由每一位消費者所發起的「互助 、 互惠、 共學」導向的運動。</p>
          <p>手建築期望以家人的角度帶領居住者在找尋住所的過程「去中間商化」，從源頭消費，在不假人他人之手的過程增添住宅更多「手的溫度」。</p>
        </div>
        <div class="mt-32 tracking-[2px] text-[#343434]">
          <p class="text-center ">簡單來說！ 手建築與一般建商和自建的差異就是⋯⋯</p>
          <div class="mt-[50px]  w-full text-center grid grid-cols-1 md:grid-cols-3 gap-16">
            <div>
              <div class="flex flex-col items-center w-full md:w-[240px]">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 21h19.5m-18-18v18m10.5-18v18m6-13.5V21M6.75 6.75h.75m-.75 3h.75m-.75 3h.75m3-6h.75m-.75 3h.75m-.75 3h.75M6.75 21v-3.375c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125V21M3 3h12m-.75 4.5H21m-3.75 3.75h.008v.008h-.008v-.008zm0 3h.008v.008h-.008v-.008zm0 3h.008v.008h-.008v-.008z" />
                </svg>
                <p class="mt-[2px]">建設公司模式</p>
              </div>
              <p class="mt-5 py-5 w-full md:w-[240px] h-[130px] bg-[#EFEFEF] rounded-[5px] flex items-center justify-center text-sm">建設公司統包</p>
            </div>
            <div >
              <div class="flex flex-col items-center w-full md:w-[240px]">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 21v-4.875c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125V21m0 0h4.5V3.545M12.75 21h7.5V10.75M2.25 21h1.5m18 0h-18M2.25 9l4.5-1.636M18.75 3l-1.5.545m0 6.205l3 1m1.5.5l-1.5-.5M6.75 7.364V3h-3v18m3-13.636l10.5-3.819" />
                </svg>
                <p class="mt-[2px]">自地自建模式</p>
              </div>
              <p class="mt-5 py-5 w-full md:w-[240px] h-[130px] bg-[#EFEFEF] rounded-[5px] flex items-center justify-center text-sm">營造廠商統包<br/>or<br/>自行發包</p>
            </div>
            <div>
              <div class="flex flex-col items-center w-full md:w-[240px]">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M10.05 4.575a1.575 1.575 0 10-3.15 0v3m3.15-3v-1.5a1.575 1.575 0 013.15 0v1.5m-3.15 0l.075 5.925m3.075.75V4.575m0 0a1.575 1.575 0 013.15 0V15M6.9 7.575a1.575 1.575 0 10-3.15 0v8.175a6.75 6.75 0 006.75 6.75h2.018a5.25 5.25 0 003.712-1.538l1.732-1.732a5.25 5.25 0 001.538-3.712l.003-2.024a.668.668 0 01.198-.471 1.575 1.575 0 10-2.228-2.228 3.818 3.818 0 00-1.12 2.687M6.9 7.575V12m6.27 4.318A4.49 4.49 0 0116.35 15m.002 0h-.002" />
                </svg>
                <p class="mt-[2px] text-[#813B31]">手建築的模式</p>
              </div>
              <p class="mt-5 py-5 w-full md:w-[240px] h-[130px] bg-[#EFEFEF] rounded-[5px] flex items-center justify-center text-sm">消費者統包<br/>+<br/>專業建築經理<br/>+<br/>營造廠只包主結構體</p>
            </div>
          </div>
        </div>
      </div>
      <div class="mt-32 max-w-[920px] mx-auto">
        <div class="big-title text-center py-16">
        <p>團隊介紹</p>
      </div>
      <div class="block-content text-[18px] tracking-[5px] flex flex-col gap-7 max-w-[920px] mx-auto text-justify">
        <div>
          <div class="flex items-center gap-8">
            <p class="px-4 py-2 bg-[#968E85] text-white font-semibold rounded-[3px]">手建築姐</p>
            <p class="text-[#968E85] font-semibold text-[20px]">Sylvia</p>
          </div>
          <p class="mt-[40px] font-medium text-base">把建築輕鬆帶過，顯然並不適合。 我們不得不面對一個非常尷尬的事實，那就是，若發現問題比我們想像的還要深奧，那肯定不簡單。帶著這些問題，我們一起來審視建築。儘管如此，別人往往卻不這麼想。透過逆向歸納，得以用最佳的策略去分析建築。</p>
          <div class="flex flex-wrap md:flex-nowrap  items-start justify-between gap-10 md:gap-[100px] mt-4">
            <div>
              <p class="font-medium text-base">建築改變了我的命運。建築，到底應該如何實現。問題的核心究竟是什麼？契訶夫說過一句經典的名言，蚜蟲吃青草，銹吃鐵，虛偽吃靈魂。這讓我對於看待這個問題的方法有了巨大的改變。</p>
              <img class="mt-4 ml-auto" src="@/assets/images/sign_wang.png" alt="">
            </div>
            <div class="w-full md:w-[360px] flex flex-col gap-0.5 border-l-[5px] border-[#D9D9D9] pl-[16px] py-1">
              <div class="w-full flex items-center justify-between text-[#968E85] whitespace-nowrap text-sm font-medium tracking-wide md:tracking-[5px] ">
                <div class="w-[90px] md:w-[110px] flex  justify-between shrink-0">
                  <p>2023- </p>
                  <p class="mr-[-0.025em] md:mr-[-5px]">至今</p>
                </div>
                <p>手建築有限公司 Founder</p>
              </div>
              <div class="w-full flex items-center justify-between text-[#968E85] whitespace-nowrap text-sm font-medium tracking-wide md:tracking-[5px]">
                <div class="w-[90px] md:w-[110px] flex justify-between shrink-0">
                  <p>2021- </p>
                  <p class="mr-[-0.025em] md:mr-[-5px]">至今</p>
                </div>
                <p>前端網頁設計師</p>
              </div>
              <div class="w-full flex items-center justify-between text-[#968E85] whitespace-nowrap text-sm font-medium tracking-wide md:tracking-[5px]">
                <div class="w-[90px] md:w-[110px] flex justify-between shrink-0">
                  <p>2019-</p>
                  <p>2021</p>
                </div>
                <p>北科互動設計系 碩士</p>
              </div>
              <div class="w-full flex items-center justify-between text-[#968E85] whitespace-nowrap text-sm font-medium tracking-wide md:tracking-[5px]">
                <div class="w-[90px] md:w-[110px] flex justify-between shrink-0">
                  <p>2016-</p>
                  <p>2019</p>
                </div>
                <p>南臺創新產品設計系 學士</p>
              </div>
            </div>
          </div>
          
          <div class="w-full flex justify-end">
            <p></p>
            <img class="w-[200px] h-[200px]" src="@/assets/images/avatar_wang.png" alt="">
          </div>
        </div>
      </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref, onMounted } from "vue";

/**
 * 判斷navigation bar menu狀態
 * @params menuStatus false=關閉菜單, true=開啟菜單
 * @params clientWidth 監聽目前裝置寬度，以判斷是否顯示hamburger
 */

const menuStatus = ref(false);
const clientWidth = ref(null);

clientWidth.value = window.innerWidth;
onMounted(() => {
  window.addEventListener("resize", () => {
    clientWidth.value = window.innerWidth;
    console.log(clientWidth.value);
  });
});
</script>

<style scoped>
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
  transition: transform 0.8s ease-in-out;
}

.key-vision-shadow:hover {
  transform: scale(1.3) translateX(80px);
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


.big-title p {
  display: inline-block;
  text-align: center;
  color: #813b31;
  font-size: 24px;
  width: auto;
  position: relative;
  padding: 0 130px;
  letter-spacing: 5px;
  white-space: nowrap;
}

.big-title p:before {
  content: "";
  display: block;
  max-width: 96px;
  width: 60%;
  height: 0.5px;
  background: #000;
  left: 0px;
  top: 50%;
  position: absolute;
}

.big-title p:after {
  content: "";
  display: block;
  max-width: 96px;
  width: 60%;
  height: 0.5px;
  background: #000;
  right: 0px;
  top: 50%;
  position: absolute;
}

@media (max-width: 850px){
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
    transform: scale(1.6);
    transition: transform 0.8s ease-in-out;
  }

  .key-vision-shadow:hover {
    transform: scale(1.6) translateX(60px);
  }


.big-title p {
  display: inline-block;
  text-align: center;
  color: #813b31;
  font-size: 24px;
  width: auto;
  position: relative;
  padding: 0 90px;
  letter-spacing: 5px;
  white-space: nowrap;
}

.big-title p:before {
  content: "";
  display: block;
  max-width: 56px;
  width: 60%;
  height: 0.5px;
  background: #000;
  left: 0px;
  top: 50%;
  position: absolute;
}

.big-title p:after {
  content: "";
  display: block;
  max-width: 56px;
  width: 60%;
  height: 0.5px;
  background: #000;
  right: 0px;
  top: 50%;
  position: absolute;
}
}

</style>
