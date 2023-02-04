<template>
  <nav
    class="noto-serif flex items-center fixed left-0 right-0 z-10 bg-white/10 h-[58px] backdrop-blur-[4px] px-4 py-2"
  >
    <div
      class="sm:max-w-[1080px] w-full flex items-center justify-between mx-auto"
    >
      <div class="flex items-center gap-3">
        <img class="w-[50px]" src="../assets/images/LOGO.svg" alt="" />
        <p class="text-[#2A2A2A] font-semibold tracking-[10px] text-sm">
          手建築研究所
        </p>
      </div>
      <ul class="flex items-center text-[#2B2B2B] gap-8 text-sm tracking-[5px]">
        <li>關於手建築</li>
        <li>團隊介紹</li>
        <li>殼計畫</li>
      </ul>
    </div>
  </nav>
  <section class="mt-[58px] inline-block">
    <div class="">
      <div
        class="key-vision noto-serif absolute left-0 h-[750px] w-[1000px] bg-slate-100 overflow-hidden"
      >
        <div class="key-vision-base absolute w-full h-full">
          <img class="w-full h-full" src="../assets/images/base.png" alt="" />
        </div>
        <div class="key-vision-text">
          <p
            class="tracking-[60px] font-bold text-[42px] text-white align-middle"
          >
            手建築研究所
          </p>
          <p class="text-[20px] tracking-[14.5px] pl-1 text-white font-bold">
            Handchitecture Gallery
          </p>
        </div>
        <div class="key-vision-shadow absolute w-full h-full">
          <img class="w-full h-full" src="../assets/images/shadow.png" alt="" />
        </div>
      </div>
      <div class="key-text absolute right-20 top-[30%] chenyuluoyan tracking-[3px] text-[30px] text-[#343434]">
        <p class="mt-20">親手創造夢想住宅的旅途</p>
        <p>這是一趟屬於您與家人，</p>
      </div>
    </div>
  </section>
</template>

<script setup></script>

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

.key-vision-text {
  position: absolute;
  left: 60%;
  top: 50%;
  transform: translate(-60%, -50%);
  white-space: nowrap;
}

.key-vision-shadow {
  transform: scale(1.2);
  transition: transform 0.8s ease-in-out;
}

.key-vision-shadow:hover {
  transform: scale(1.2) translateX(80px);
}

.key-text {
  -webkit-writing-mode: vertical-lr;
  writing-mode: vertical-lr;
}
</style>
