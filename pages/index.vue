<template>
  <div class="container-root">

    <!-- Meta Tags -->
    <Head>
      <Title>Dierenarts Verboom</Title>

      <Meta name="title" content="Dierenarts Verboom"/>
      <Meta name="description" content="Uw dierenarts in Kapelle, Professionele zorg voor uw huisdieren en duiven. Persoonlijk contact, goede begeleiding kennis en kunde."/>
      <Meta name="viewport" content="width=device-width, initial-scale=1"/>
      <Meta name="keywords" content="dierenarts, hond, kat, ziek, konijn, duif, kapelle, goes, zeeland, dier, bijsluiters, diergeneeskundige, zorg, gezelschapsdieren, yerseke, praktijk, whatsapp, hills, voer, duivensport, vaccinaties, verzorging, online, spoed"/>
      <Meta name="category" content="dierenarts"/>
      <Meta name="robots" content="index, follow"/>
      <Meta name="revisit-after" content="2 days"/>
      <Meta name="og:title" content="Dierenarts Verboom"/>
      <Meta name="og:description" content="Uw dierenarts in Kapelle, Professionele zorg voor uw huisdieren en duiven. Persoonlijk contact, goede begeleiding kennis en kunde."/>
      <Meta name="og:image" content="dierenartsverboom.nl/img/logo-big.30fd7711.png"/>
      <Meta name="og:region" content="Zeeland"/>

      <Link rel="canonical" href="https://www.dierenartsverboom.nl/"/>
      <Link rel="icon" href="favicon.ico" type="image/x-icon"/>
    </Head>

    <HeaderComponent />

    <main>
      <div class="container-frontpage">
        <img class="desktop-img" src="../assets/voorkant.jpg">
        <img class="mobile-img" src="../assets/voorkant-mobile.jpg">
      </div>
    </main>

    <BottomComponent />

    <a class="whatsapp" href="https://wa.me/message/POZDDNGDMO6JM1" target="_blank">
      <img class="whatsapp-img" src="../assets/whatsapp.png" alt="wa">
    </a>
    
  </div>
</template>

<script setup lang="ts">
  useHead({
    title: 'Dierenarts Verboom',
    meta: [
      { name: 'description', content: 'Uw dierenarts in Kapelle, Professionele zorg voor uw huisdieren en duiven. Persoonlijk contact, goede begeleiding kennis en kunde.' }
    ],
  })
</script>

<style>
/* Font Import */

@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;

  font-family: 'Inter', sans-serif;
  font-size: 16px;
  line-height: 1.6;
}

/* Variables */

:root {
  --main-green: #14823B;
  --wa-green: #25D366;
  --main-orange: #F8931F;
  --main-orange-hover: #ff8800de;
  --text-black: #000;
  --main-gray: #545454;
}

/* Keyframes */

@keyframes fadeIn {
  0% { opacity: 0; }
  100% { opacity: 1; }
}

/* Main Section */

main {
  min-height: 450px;

  animation: fadeIn 0.25s;
}

.container-frontpage {
  display: flex;
  justify-content: center;
}

.container-frontpage > img {
  height: auto;
  width: 100%;
}

.desktop-img {
  display: none;
}

@media (min-width: 800px) {
  .desktop-img {
    display: block;
  }

  .mobile-img {
    display: none;
  }
}
    
/* Whatsapp Button */

.whatsapp {
  z-index: 3;
}

.whatsapp-img {
  height: 50px;
  width: 50px;
        
  position: fixed;
  right: 20px;
  bottom: 20px;

  border-radius: 40px;

  transition: 0.5s;
}

.whatsapp-img:hover {
  transform: scale(1.2);
  transition: 0.3s linear;
}

@media (min-width: 560px) {
  .whatsapp-img {
    height: 75px;
    width: 75px;

    position: fixed;
    right: 30px;
    bottom: 50px;

    animation: fadeIn 0.35s;
  }
}
</style>