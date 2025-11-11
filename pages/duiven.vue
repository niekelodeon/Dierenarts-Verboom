<template>
  <div class="container-root">

    <!-- Meta Tags -->
    <Head>
      <Title>Duiven - Dierenarts Verboom & de Kok</Title>

      <Meta name="description" content="Specialistische zorg voor duiven en duivensport. Vaccinaties, mestonderzoek, keeluitstrijkjes en advies voor gezonde en sterke duiven. Deskundige begeleiding voor liefhebbers in Zeeland."/>
      <Meta name="keywords" content="duiven, duivensport, vaccinaties duiven, trichomonas, paramyxo, rotavirus, adenovirus, pokken, mestonderzoek duiven, keeluitstrijkje, luchtweginfecties, dikke koppen, ornithose, verzorging duiven, kweek duiven, controle duiven, dierenarts duiven, Zeeland, Kapelle, Goes, Yerseke, duivenarts"/>

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
      <Meta property="og:description" content="Specialistische zorg voor duiven en duivensport. Vaccinaties, mestonderzoek, keeluitstrijkjes en advies voor gezonde en sterke duiven. Deskundige begeleiding voor liefhebbers in Zeeland."/>
      <Meta property="og:image" content="dierenartsverboom.nl/img/logo-big.30fd7711.png"/>
      <Meta property="og:locale" content="nl_NL"/>
      <Meta name="og:region" content="Zeeland"/>

      <!-- Apple Meta Tags -->
      <Meta name="apple-mobile-web-app-capable" content="yes"/>
      <Meta content="yes" name="apple-touch-fullscreen" />
      <Meta name="format-detection" content="telephone=yes"/>
      <Meta name= "viewport" content = "width = device-width"/>

      <Link rel="canonical" href="https://www.dierenartsverboom.nl/duiven"/>
      <Link rel="icon" href="favicon.ico" type="image/x-icon"/>
    </Head>

    <HeaderComponent/>

    <main>

      <div class="container-main">

        <div class="container-about">

          <div class="text-container-1">

            <h1>Duiven</h1>

            <p>
              De moderne duivensport is een complex samenspel van diverse factoren.
              Onder andere de
              kwaliteit van de duiven, de verzorging, het hok (ventilatie) en de motivatie spelen een
              belangrijke rol.
              Maar bij dit alles speelt de gezondheid een grote rol.
            </p>

          </div>

          <div class="text-container-2">

            <h1>Wij doen:</h1>
            <h2>Vaccinaties:</h2>

            <ul class="vaccinaties">
              <li>Nobilis paramyxo p201 (paramyxo)</li>
              <li>RP vac (paramyxo + rotavirus)</li>
              <li>Pharmavac Columbi 2 + diftovac (paramyxo + pokken)</li>
              <li>Pharmavac PHA (paramyxo + herpes + adenovirus)</li>
            </ul>

          </div>

          <div class="text-container-3">

            <h2>Parasitair Onderzoek:</h2>

            <ul class="onderzoek">
              <li>Mestonderzoek (wormen + coccidiose)</li>
              <li>Keeluitstrijkje (trichmonas / ’t geel)</li>
              <li>Luizen</li>
            </ul>

          </div>

          <div class="text-container-4">

            <h2>Bestrijding luchtweginfecties:</h2>

            <ul class="bestrijding">
              <li>Ornithose</li>
              <li>Slijm in de keel / Dikke koppen</li>
            </ul>

          </div>

          <div class="text-container-5">

            <h2>Controles voor de kweek:</h2>

            <p>1 maand van te voren de dierenarts bezoeken, breng van ieder hok 2 duiven en een mestmonster mee.</p>

          </div>

        </div>

        <div class="container-image">
          <img src="../assets/duiven.jpg" alt="duiven">
        </div>

      </div>

    </main>

    <BottomComponent/>

    <a class="whatsapp" href="https://wa.me/message/POZDDNGDMO6JM1" target="_blank">
      <img class="whatsapp-img" src="../assets/whatsapp.png" alt="wa">
    </a>
  </div>
</template>

<script setup lang="ts">
useHead({
  title: 'Dierenarts Verboom & de Kok',
})
</script>

<style scoped>
/* Font Import */

@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&display=swap');

/* Main Section */

main > .container-main {
  display: flex;
  flex-direction: column;
  gap: 40px;

  margin-top: 25px;
  margin-inline: 35px;

  padding-bottom: 50px;
}

.container-about {
  display: flex;
  flex-direction: column;
  gap: 25px;
}

.vaccinaties, .onderzoek, .bestrijding {
  position: relative;
  left: 20px;
}

.container-about > .text-container-1 > h1 {
  font-size: 18px;
  font-weight: 600;

  margin-bottom: 10px;
}

.container-about > .text-container-2 > h1 {
  font-size: 18px;
  font-weight: 500;

  margin-bottom: 10px;
}

.container-hills > .download-app-container {
  display: flex;
  justify-content: center;
  text-decoration: none;
  gap: 15px;
}

.container-hills > .download-app-container > a > img {
  height: 43px;
  width: 119px;
}

.container-about > .text-container-3 > h1 {
  font-size: 18px;
  font-weight: 500;

  margin-bottom: 10px;
}

.container-about > .text-container-4 > h1 {
  font-size: 18px;
  font-weight: 500;

  margin-bottom: 10px;
}
        
.container-about > .text-container-5 > h1 {
  font-size: 18px;
  font-weight: 500;

  margin-bottom: 15px;
}

h2 {
  font-size: 16px;
  font-weight: 500;

  margin-bottom: 5px;
}

.container-about > p {
  display: flex;
  flex-direction: column;
  margin-bottom: 20px;

  font-size: 16px;
  font-weight: 400;
}

.container-image {
  display: flex;
  flex-direction: row;
  justify-content: center;
  gap: 20px;
}

.container-image > img {
  width: 206px;
  height: 274px;
}

@media (min-width: 560px) {
  .container-about > .download-app-container {
    display: flex;
    justify-content: start;

    padding-left: 25px;

    gap: 45px;
  }
        
  .container-about > .download-app-container > a > img {
    display: flex;
    justify-content: center;
    text-decoration: none;
    gap: 35px;

    height: 100%;
    width: 100%;
  }

  .container-image > img {
    width: 305px;
    height: 406px;
  }
}

@media (min-width: 940px) {
        
  main > .container-main {
    display: flex;
    flex-direction: row;
    gap: 70px;

    margin-top: 45px;
    margin-left: 75px;
    margin-right: 45px;

    padding-bottom: 100px;
  }
        
  .container-image {
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 20px;

    margin-right: 10px;
  }
        
  .container-about {
    display: flex;
    flex-direction: column;
    gap: 25px;
  }

  .container-about > .download-app-container {
    display: none;
  }
        
  .container-about > .download-app-container > a > img {
    display: flex;
    justify-content: center;
    text-decoration: none;
    gap: 35px;

    height: 100%;
    width: 100%;
  }
        
  .container-image {
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 200px;
  }
}

@media (min-width: 1400px) { 

  .container-about {
    display: flex;
    flex-direction: column;
    gap: 35px;
  }

  .container-about > .text-container-1 > h1 {
    font-size: 20px;
    font-weight: 600;

    margin-bottom: 15px;
  }
        
  .container-about > .text-container-2 > h1 {
    font-size: 18px;
    font-weight: 500;

    margin-bottom: 15px;
  }
            
  .container-about > .text-container-3 > h1 {
    font-size: 18px;
    font-weight: 500;

    margin-bottom: 15px;
  }
        
  .container-about > .text-container-4 > h1 {
    font-size: 18px;
    font-weight: 500;
    
    margin-bottom: 15px;
  }
        
  .container-about > .text-container-5 > h1 {
    font-size: 18px;
    font-weight: 500;

    margin-bottom: 15px;
  }
        
  main > .container-main {
    display: flex;
    flex-direction: row;
    gap: 500px;

    margin-top: 65px;
    margin-left: 150px;
    margin-right: 45px;

    padding-bottom: 100px;
  }
        
  .container-image {
    display: flex;
    flex-direction: column;
    justify-content: center;

    margin-right: 150px;
  }
}
</style>