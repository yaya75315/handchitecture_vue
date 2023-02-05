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
      <div
        v-if="clientWidth < 560"
        class="hamburger"
        :class="{ open: menuStatus }"
        @click="menuStatus = !menuStatus"
      >
        <span></span>
        <span></span>
        <span></span>
      </div>
      <ul
        class="flex items-center text-[#2B2B2B] gap-8 text-sm tracking-[5px]"
        :class="[{ menu: clientWidth < 560 }, { open: menuStatus }]"
      >
        <li>關於手建築</li>
        <li>團隊介紹</li>
        <li>殼計畫</li>
      </ul>
    </div>
  </nav>
  <section class="mt-[58px] inline-block">
    <div class="">
      <div
        class="key-vision noto-serif absolute left-0 h-[calc(100vh-58px)] w-full lg:w-[calc(100%-300px)] bg-slate-100 overflow-hidden"
      >
        <div class="key-vision-base absolute w-full h-full">
          <img
            class="w-full h-full object-cover"
            src="../assets/images/base.png"
            alt=""
          />
        </div>
        <div class="key-vision-text">
          <p
            class="tracking-[20px] lg:tracking-[60px] font-bold text-[30px] md:text-[42px] text-white align-middle"
          >
            手建築研究所
          </p>
          <p
            class="text-[12px] md:text-[20px] tracking-[6px] lg:tracking-[14.5px] pl-1 text-white font-bold"
          >
            Handchitecture Gallery
          </p>
        </div>
        <div class="key-vision-shadow absolute w-full h-full">
          <img
            class="w-full h-full object-cover"
            src="../assets/images/shadow.png"
            alt=""
          />
        </div>
      </div>
      <div
        class="key-text absolute right-6 md:right-40 top-[62vh] whitespace-nowrap lg:top-[30vh] chenyuluoyan tracking-[3px] text-[30px] text-[#343434]"
      >
        <p class="mt-20">親手創造夢想住宅的旅途</p>
        <p>這是一趟屬於您與家人，</p>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref, onMounted } from "vue";

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

@media (max-width: 600px) {
  .key-vision-text {
    top: 40%;
  }
}

.key-vision-shadow {
  transform: scale(1.5);
  transition: transform 0.8s ease-in-out;
}

.key-vision-shadow:hover {
  transform: scale(1.5) translateX(80px);
}

.key-text {
  -webkit-writing-mode: vertical-lr;
  writing-mode: vertical-lr;
}

.hamburger {
  cursor: pointer;
  background-color: transparent;
  width: 40px;
  height: 20px;
  margin-left: auto;
}

.hamburger span {
  display: block;
  width: 30px;
  height: 3px;
  background-color: #000;
}

.hamburger span:not(:last-child) {
  margin-bottom: 5px;
}
.hamburger span:nth-child(2) {
  margin-left: auto;
  transition: background-color 0.25s, transform 0.3s;
}
.hamburger span:nth-child(1),
.hamburger span:nth-child(3) {
  transition: transform 0.45s;
}

.hamburger.open {
  z-index: 1000;
}

.hamburger.open span {
  background-color: #fff;
}

.hamburger.open span:nth-child(2) {
  transform: translateX(-20px);
  background-color: transparent !important;
}
.hamburger.open span:nth-child(1) {
  transform: translate(0%, 6px) rotate(315deg);
}
.hamburger.open span:nth-child(3) {
  transform: translate(0%, -11px) rotate(-315deg);
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
  padding: 58px;
  opacity: 0.8;
  transform: translateX(-100%);
  transition: transform 0.3s ease-in-out;
}

.menu.open {
  transform: translateX(0);
}
</style>
