<template>
  <div class="container-root">

  <!-- Meta Tags -->
  <Head>
    <Title>Bijsluiters - Dierenarts Verboom & de Kok</Title>

    <meta name="description" content="Online kunt u ook de bijsluiters vinden van de medicijnen die wij in de praktijk gebruiken. Zo heeft u altijd snel toegang tot belangrijke informatie over dosering, toepassing en eventuele bijwerkingen voor uw hond, kat, konijn of duif."/> 
    <Meta name="keywords" content="bijsluiters, medicijnen huisdieren, diergeneeskunde, hond, kat, konijn, duif, gezelschapsdieren, vaccinaties, ontwormen, vlooienbestrijding, hartworm, antibioticum, pijnstilling, ontstekingsremmers, parasieten, diergeneeskundige zorg, medische bijsluiters, Dierenarts Verboom & de Kok, Kapelle, Zeeland, spoed, infecties, allergieën, dieetvoeding, voeding bij ziekte, hondenziekten, katziekten, konijnenziekten, luchtweginfecties, maag- en darmproblemen, huidproblemen"/>

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
    <Meta property="og:description" content="Online kunt u ook de bijsluiters vinden van de medicijnen die wij in de praktijk gebruiken. Zo heeft u altijd snel toegang tot belangrijke informatie over dosering, toepassing en eventuele bijwerkingen voor uw hond, kat, konijn of duif."/>
    <Meta property="og:image" content="dierenartsverboom.nl/img/logo-big.30fd7711.png"/>
    <Meta property="og:locale" content="nl_NL"/>
    <Meta name="og:region" content="Zeeland"/>

    <!-- Apple Meta Tags -->
    <Meta name="apple-mobile-web-app-capable" content="yes"/>
    <Meta content="yes" name="apple-touch-fullscreen" />
    <Meta name="format-detection" content="telephone=yes"/>
    <Meta name= "viewport" content = "width = device-width"/>

    <Link rel="canonical" href="https://www.dierenartsverboom.nl/bijsluiters"/>
    <Link rel="icon" href="favicon.ico" type="image/x-icon"/>
  </Head>

  <HeaderComponent />

  <main>

    <div class="container-main">

      <h1>Bijsluiters</h1>

        <div class="container-above">

          <div class="animal">
            <NuxtLink to="/bijsluiters/hond" exact class="nav-link">
              <img src="../../assets/hond.png" alt="hond">
              <h2>Hond</h2>
            </NuxtLink>
          </div>
                        
          <div class="animal">
            <router-link to="/bijsluiters/kat" exact class="nav-link">
              <img src="../../assets/kat.png" alt="kat">
              <h2>Kat</h2>
            </router-link>
          </div>

        </div>

        <div class="container-below">

          <div class="animal">
            <router-link to="/bijsluiters/konijn" exact class="nav-link">
              <img src="../../assets/konijn.png" alt="konijn">
              <h2>Konijn</h2>
            </router-link>

          </div>

          <div class="animal">
            <router-link to="/bijsluiters/duif" exact class="nav-link">
              <img src="../../assets/duif.png" alt="duif">
              <h2>Duif</h2>
            </router-link>
          </div>

        </div>

    </div>

    </main>

    <BottomComponent />

    <a class="whatsapp" href="https://wa.me/message/POZDDNGDMO6JM1" target="_blank">
      <img class="whatsapp-img" src="../../assets/whatsapp.png" alt="wa">
    </a>

  </div>
</template>

<script setup lang="ts">
useHead({
  title: 'Dierenarts Verboom & de Kok',
})
</script>

<style>
/* Main Section */

.container-main {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 10px;

  margin-top: 25px;
  margin-inline: 35px;

  padding-bottom: 200px;
}

@media (min-width: 940px) {       
  main > .container-main {
    margin-top: 45px;
    margin-inline: 45px;
            
    padding-bottom: 100px;
  }
}

@media (min-width: 1400px) {      
  main > .container-main {
    flex-direction: column;

    margin-top: 65px;
    margin-inline: 45px;
        
    padding-bottom: 300px;
  }
}

.container-above {
  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 20px;

  margin-top: 10px;
  margin-bottom: 10px;
}

.container-below {
  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 20px;

  margin-top: 10px;
}

.container-main > h1 {
  font-size: 18px;
  font-weight: 600;
}

.animal {
  display: flex;
  justify-content: center;
  align-items: center;

  background-color: #fff;

  max-width: 140px;
  height: 140px;
}

.animal > a {
  padding-inline: 43px;

  text-decoration: none;
}

.animal > a > h2 {
  text-align: center;
  font-weight: 500;
  color: var(--text-black);
}

.container-below > .animal > a > h2 {
  margin-top: 5px;
}

@media (min-width: 1400px) {
  .container-main > h1 {
    font-size: 20px;
    font-weight: 600;
        
    margin-bottom: 15px;
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