<template>
  <div class="container-root">

    <!-- Meta Tags -->
    <Head>
      <Title>Dierenarts Verboom & de Kok</Title>

      <Meta name="title" content="Dierenarts Verboom & de Kok"/>
      <Meta name="description" content="Uw dierenarts in Kapelle, Professionele zorg voor uw huisdieren en duiven. Persoonlijk contact, goede begeleiding kennis en kunde."/>
      <Meta name="keywords" content="dierenarts, dierenkliniek, dierenpraktijk, DAP, spoedeisend, spoedeisende hulp, gezelschapsdieren, diergeneeskundige zorg, Kapelle, Goes, Yerseke, Wemeldinge, Zeeland, Zuid-Beveland, hond, kat, konijn, vee, kleindieren, kleindier, cavia, duif, vogel, knaagdier, puppy, kitten, zieke hond, zieke kat, enting, vaccinaties, chippen, operatie, castratie, sterilisatie, gebitsbehandeling, spoed, spoeddierenarts, consult, spreekuur, afspraak maken, verzorging, dieet, dieetvoer, Hills, voeding, voer, advies, ontwormen, vlooienbestrijding, parasieten, bijsluiters, medicatie, medicijnen, behandeling, kleinschalig, persoonlijk, online, deskundig, online contact, WhatsApp, telefoon, openingstijden, zorg voor dieren, diergeneeskunde, duivensport, huisdieren, dierenzorg, lange ervaring, dierenarts bij mij in de buurt"/>

      <Meta name="format-detection" content="telephone=yes,email=no,address=yes"/>
      <Meta name="category" content="dierenarts"/>
      <meta name="subject" content="dierenarts">
      <Meta name="author" content="Dierenarts Verboom & de Kok"/>
      <Meta name="copyright" content="© 2025 Dierenarts Verboom & de Kok. All rights reserved."/> 

      <Meta name="HandheldFriendly" content="true"/>
      <Meta name="MobileOptimized" content="370"/>
      <Meta name="theme-color" content="#4CAF50"/>
      <Meta name="viewport" content="width=device-width, initial-scale=1"/>

      <Meta name="robots" content="index, follow"/>
      <Meta name="revisit-after" content="2 days"/>

      <!-- OpenGraph Meta Tags -->
      <Meta property="og:title" content="Dierenarts Verboom & de Kok"/>
      <meta name="og:phone_number" content="0113-290800"/>
      <meta name="og:email" content="info@dierenartsverboom.nl"/>
      <Meta property="og:description" content="Uw dierenarts in Kapelle, Professionele zorg voor uw huisdieren en duiven. Persoonlijk contact, goede begeleiding kennis en kunde."/>
      <Meta property="og:image" content="dierenartsverboom.nl/img/logo-big.30fd7711.png"/>
      <Meta property="og:locale" content="nl_NL"/>
      <Meta name="og:region" content="Zeeland"/>

      <!-- Apple Meta Tags -->
      <Meta name="apple-mobile-web-app-capable" content="yes"/>
      <Meta content="yes" name="apple-touch-fullscreen" />
      <Meta name="format-detection" content="telephone=yes"/>
      <Meta name= "viewport" content = "width = device-width"/>

      <Link rel="canonical" href="https://www.dierenartsverboom.nl/"/>
      <Link rel="icon" href="favicon.ico" type="image/x-icon"/>
    </Head>

    <HeaderComponent />

    <main>
      <div class="container-frontpage">
        <!-- <img class="desktop-img" src="../assets/voorkant.jpg" alt="desktop-img">
        <img class="mobile-img" src="../assets/voorkant-mobile.jpg" alt="mobile-img"> -->

        <h1 class="hidden-text">Al sinds 1987 zetten wij ons in voor de beste zorg voor uw huisdier. Persoonlijk contact, goede begeleiding en kunde. Voor spoedgevallen te bereiken op 0113 - 290800 voor klanten van onze praktijk.</h1>
      </div>
    </main>

    <BottomComponent />

    <LanguageComponent />

    <a class="whatsapp" href="https://wa.me/message/POZDDNGDMO6JM1" target="_blank">
      <img class="whatsapp-img" src="../assets/whatsapp.png" alt="wa">
    </a>
    
  </div>
</template>

<script setup lang="ts">
useHead({
  title: 'Dierenarts Verboom & de Kok',
  meta: [
    {
      name: 'description',
      content: 'Uw dierenarts in Kapelle, Professionele zorg voor uw huisdieren en duiven. Persoonlijk contact, goede begeleiding kennis en kunde.',
    },
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

.container-frontpage > .hidden-text {
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