

<template>
<div class="sm:max-w-[1080px] mx-auto">
    <HomeView />
</div>

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
