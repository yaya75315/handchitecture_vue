

<template>
  <div class="content">
    <HomeView />
  </div>
  <footer class="bg-[#CABFB3]/10 pt-56">
    <div class="bg-[#813B31] h-20 px-4 w-full flex items-center justify-between">
      <div class="gap-10 sm:max-w-[1080px] w-full  flex items-center justify-between mx-auto">
        <div class="flex items-center gap-3">
          <a href="https://www.facebook.com/HandchitectureGallery" target="_blank">
            <img src="@/assets/images/fb.svg" alt="">
          </a>
          <a href="https://lin.ee/HYpX7NC" target="_blank">
            <img src="@/assets/images/line.svg" alt="">
          </a>
          <a href="" target="_blank">
            <img src="@/assets/images/notion.svg" alt="">
          </a>
          <a href="mailto:handchitecture@gmail.com" target="_blank">
            <img src="@/assets/images/email.svg" alt="">
          </a>
        </div>
        <div class="text-white font-medium text-sm tracking-[1px]">Copyright © 2022 手建築有限公司</div>
      </div>
    </div>


  </footer>

</template>

<script setup>
import HomeView from "./views/HomeView.vue";

</script>
<style>
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

@media (max-width: 600px) {
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
