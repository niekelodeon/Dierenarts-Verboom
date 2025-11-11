<template>
  <div class="container-root">

    <!-- Meta Tags -->
    <Head>
      <Title>Hill’s voeding - Dierenarts Verboom & de Kok</Title>

      <Meta name="description" content="Hill’s voeding voor hond en kat bij Dierenarts Verboom & de Kok in Kapelle. Gezonde voeding met goede vetten, eiwitten en vitamines. Bespaar via de Hill’s Korting App en ontvang deskundig advies van uw dierenarts."/>
      <Meta name="keywords" content="hills voeding, hond, kat, dieetvoer, huisdieren, gezonde voeding, hondenvoer, kattenvoer, Hills app, korting voeding, voer advies, dierenarts advies, gezelschapsdieren, Dierenarts Verboom & de Kok, Kapelle, Zeeland, huisdieren voeding, Hills dieet, voer kopen, premium voer"
      />

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
      <Meta property="og:description" content="Hill’s voeding voor hond en kat bij Dierenarts Verboom & de Kok in Kapelle. Gezonde voeding met goede vetten, eiwitten en vitamines. Bespaar via de Hill’s Korting App en ontvang deskundig advies van uw dierenarts."/>
      <Meta property="og:image" content="dierenartsverboom.nl/img/logo-big.30fd7711.png"/>
      <Meta property="og:locale" content="nl_NL"/>
      <Meta name="og:region" content="Zeeland"/>

      <!-- Apple Meta Tags -->
      <Meta name="apple-mobile-web-app-capable" content="yes"/>
      <Meta content="yes" name="apple-touch-fullscreen" />
      <Meta name="format-detection" content="telephone=yes"/>
      <Meta name= "viewport" content = "width = device-width"/>

      <Link rel="canonical" href="https://www.dierenartsverboom.nl/hillsvoeding"/>
      <Link rel="icon" href="favicon.ico" type="image/x-icon"/>
    </Head>

    <HeaderComponent/>

    <main>

      <div class="container-main">

        <div class="container-hills">

          <div class="text-container-1">

            <h1>Hill’s voeding</h1>

            <p>
              In onze praktijk promoten wij een gezonde levensstijl voor uw huisdier. Hierbij hoort ook een goede voeding. Een goede voeding bevat waardevolle ingrediënten, zoals goede
              eiwitten, mineralen en vitamines, maar ook voldoende vezels en echt goede vetten.
              De waarde van goede vetten wordt regelmatig onderschat. Het is belangrijk dat er veel
              meervoudig, onverzadigde vetzuren in de voeding aanwezig zijn. Dit is essentieel voor een
              goede hersenwerking, een goede werking van het hart en voor een goede vacht.
              Om die reden raden wij Hill’s voer aan voor uw hond en kat.
            </p>

          </div>  

          <div class="text-container-2">

            <h1>Hill’s korting app</h1>

            <p>
                Hill’s maakt het mogelijk voor ons als praktijk, dat u uw Hill’s voeding met extra korting bij
                ons kan kopen.
                Door het dowloaden van de Hill’s app is het voor ons mogelijk om de bij ons
                aangekochte voeding aan uw app toe te voegen. Hier mee spaart u voor direct korting of een
                gratis nieuwe zak.
                Daarnaast kunnen wij u voor elk dier 2 keer per jaar een quick-reco aanbieden, waar u uw
                streepjes-code moet plakken van uw aangekochte zak voer, waarmee u van Hill’s afhankelijk
                van de grote van de zak € 7,50 of € 15,00 op uw bankrekening krijg toegevoegd.
            </p>
            
          </div>

          <div class="text-container-3">

            <h1>Hill’s is ontwikkeld door dierenartsen</h1>

            <p>
              In de jaren 70 van de vorige eeuw is een dierenarts in de Verenigde Staten begonnen met
              voeding te maken voor een nierpatiënt. Er was toen nog geen enkele voeding voor zieke
              dieren op de markt.
              Hill’s heeft zich sindsdien steeds meer toegelegd op het maken van een kwalitatief
              hoogwaardig voer voor honden en katten die iets mankeren.
            </p> 

          </div>

          <div class="text-container-4">

            <h1>Waarom geen geweldige voeding voor de gezonde hond en kat?</h1>
            
            <p>
              Als je je toelegt op het maken van een uitstekende voeding
              voor zieke honden, om die zich beter te laten voelen,
              waarom maak je dan niet een voeding om uw huisdieren
              gezond te laten blijven.
              Dat heeft Hill’s uiteindelijk gedaan. Zo is de <span>VET ESSENTIALS
              LIJN&copy;</span> ontstaan. Zowel voor de hond als voor de kat.
              Zo krijgen ze het beste van het beste.
              Mocht uw hond of kat een ander merk dieetvoeding gebruiken en uw bent tevreden over
              het gebruik van deze voeding, dan kunnen wij deze voeding ook voor u verzorgen.
            </p>

          </div>

        </div>

        <div class="container-image">
            <img src="../assets/voerzak-kat.png" alt="voerzak-kat">
            <img src="../assets/voerzak-hond.png" alt="voerzak-hond">
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

.container-hills {
  display: flex;
  flex-direction: column;
  gap: 25px;
}

.container-hills > .text-container-1 > h1 {
  font-size: 18px;
  font-weight: 600;

  margin-bottom: 10px;
}

.container-hills > .text-container-2 > h1 {
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
  Width: 119px;
}

.container-hills > .text-container-3 > h1 {
  font-size: 18px;
  font-weight: 500;

  margin-bottom: 10px;
}

.container-hills > .text-container-4 > h1 {
  font-size: 18px;
  font-weight: 500;

  margin-bottom: 10px;
}

.container-hills > p {
  display: flex;
  flex-direction: column;
  margin-bottom: 20px;

  font-size: 16px;
  font-weight: 400;
}

span {
  font-weight: 500;
}

.container-image {
  display: flex;
  flex-direction: row;
  justify-content: center;
  gap: 20px;
}

.container-image > img {
  width: 140px;
  height: 140px;
}

@media (min-width: 560px) {
  .container-hills > .download-app-container {
    display: flex;
    justify-content: start;

    padding-left: 25px;

    gap: 45px;
  }
        
  .container-hills > .download-app-container > a > img {
    display: flex;
    justify-content: center;
    text-decoration: none;
    gap: 35px;

    height: 100%;
    width: 100%;
  }

  .container-image > img {
    width: 180px;
    height: 180px;
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
        
  .container-hills {
    display: flex;
    flex-direction: column;
    gap: 25px;
  }

  .container-hills > .download-app-container {
    display: none;
  }
        
  .container-hills > .download-app-container > a > img {
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
        
  .container-image > img {
    width: 240px;
    height: 240px;
  }
}

@media (min-width: 1400px) { 
  .container-hills {
    display: flex;
    flex-direction: column;
    gap: 35px;
  }

  .container-hills > .text-container-1 > h1 {
    font-size: 20px;
    font-weight: 600;
        
    margin-bottom: 15px;
  }
        
  .container-hills > .text-container-2 > h1 {
    font-size: 18px;
    font-weight: 500;
        
    margin-bottom: 15px;
  }
            
  .container-hills > .text-container-3 > h1 {
    font-size: 18px;
    font-weight: 500;
        
    margin-bottom: 15px;
  }
        
  .container-hills > .text-container-4 > h1 {
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
    gap: 200px;

    margin-right: 150px;
  }
        
  .container-image > img {
    width: 250px;
    height: 250px;
  }
}
</style>