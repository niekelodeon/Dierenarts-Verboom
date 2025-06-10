<template>
  <div class="container-root">

    <!-- Meta Tags -->
    <Head>
      <Title>Dierenarts Verboom - Over</Title>

      <Link rel="canonical" href="https://www.dierenartsverboom.nl/over"/>
    </Head>

    <HeaderComponent />

    <main>
      <div class="container-main-over">
        <div class="container-about">
          <div class="text-container-1">

            <h1>Over ons</h1>

            <p>
              In 1987 is deze praktijk van start gegaan aan de Alexanderstraat in Kapelle.
              Daarna is de praktijk verhuisd naar de Karmijnstraat 19 in Kapelle.
              Nadat ruim een jaar de praktijk gesloten is geweest, hebben we besloten om per 1 december 2022 de praktijk te heropenen.
              We wilden graag de menselijke maat binnen de diergeneeskundige zorg behouden, en verder gaan als zelfstandige praktijk voor gezelschapsdieren.
              Door de vele jaren ervaring wil ik samen met Carin de best mogelijk zorg voor uw huisdier realiseren.
            </p>

          </div>

          <div class="text-container-2">

            <h1>Wim Verboom, Dierenarts</h1>

            <p>
              Geboren en opgegroeid in Yerseke, na de lagere school heb ik 10 jaar landbouwonderwijs gevolgd.
              Na de lagere, middelbare en hogere landbouwschool, ben ik aan de studie diergeneeskunde in Utrecht begonnen.
              In 1985 afgestudeerd en vervolgens met veel plezier begonnen als praktiserende dierenarts in een gemengde praktijk in Oost-Brabant/Limburg en in
              1987 begonnen in een gemengde praktijk op Zuid-Beveland met standplaats Kapelle.
              In Kapelle zijn we begonnen op de hoek Bruellisstraat/Alexanderstraat en in 1997 verhuisd naar een ruimere praktijkruimte aan de Karmijnstraat.
            </p>
          </div>

          <div class="text-container-3">

            <h1>Carin de Kok, Dierenarts assistent</h1>

            <p>
              Geboren en opgegroeid in Kapelle. Na de lagere school, ben ik via vmbo, mbo en hbo begonnen in Antwerpen/Gent aan de studie diergeneeskunde.
              Sinds mijn veertiende jaar kom ik al bij de dierenartspraktijk eerst als stagiaire en later als dierenartsassistent.
              Op het gebied van dieetvoeding voor zowel hond en kat heb ik diverse cursussen gevolgd. Over een jaar hoop ik af te studeren als dierenarts.
            </p>

          </div>
        </div>

        <div class="container-image-over">
          <img src="../assets/over-desktop.png">
        </div>
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
    title: 'Dierenarts Verboom'
  })
</script>

<style>
/* Font Import */

@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&display=swap');

/* Main Section */

main > .container-main-over {    
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

.container-about > p {
  display: flex;
  flex-direction: column;
  margin-bottom: 20px;

  font-size: 16px;
  font-weight: 400;
}

.container-image-over {
  display: flex;
  flex-direction: row;
  justify-content: center;
  gap: 20px;
}

.container-image-over > img {
  width: 200px;
  height: 260px;
}

@media (min-width: 560px) {
  .container-image-over > img {
    width: 302px;
    height: 393px;
  }
}

@media (min-width: 940px) {
  main > .container-main-over {
    display: flex;
    flex-direction: row;
    gap: 70px;
        
    margin-top: 45px;
    margin-left: 75px;
    margin-right: 45px;
        
    padding-bottom: 100px;
  }
        
  .container-image-over {
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
        
  .container-image-over {
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
        
  main > .container-main-over {
    display: flex;
    flex-direction: row;
    gap: 500px;
        
    margin-top: 65px;
    margin-left: 150px;
    margin-right: 45px;
        
    padding-bottom: 100px;
  }
        
  .container-image-over {
    display: flex;
    flex-direction: column;
    justify-content: center;

    margin-right: 150px;
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