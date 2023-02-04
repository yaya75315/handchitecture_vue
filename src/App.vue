

<template>
<div class="sm:max-w-[1080px] mx-auto">
    <HomeView />
</div>

</template>

<script setup>
import HomeView from "./views/HomeView.vue";

</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Noto+Serif+TC:wght@200;300;400;500;600;700;900&display=swap');
@font-face {
  font-family: 'chenyuluoyan';
  src: url('../assets/font/ChenYuluoyan-Thin.woff') format("woff"),
}

@font-face {
  font-family: 'chenyuluoyan monospaced';
  src: url('../assets/font/ChenYuluoyan-Thin-Monospaced.woff') format("woff"),
}


.noto-serif{
    font-family: 'Noto Serif TC', serif;
}

.chenyuluoyan{
    font-family: 'chenyuluoyan', serif;
}

.chenyuluoyan-monospaced{
    font-family: 'chenyuluoyan monospaced', serif;
}
</style>
