<template>
  <div class="container-root">

    <!-- Meta Tags -->
    <Head>
      <Title>Dierenarts Verboom - Contact</Title>

      <Link rel="canonical" href="https://www.dierenartsverboom.nl/contact"/>
    </Head>

    <HeaderComponent/>
        
    <main>

      <div class="container-main">
        
        <div class="container-about">

          <h1>Contact</h1>

          <div class="container-contact">

            <div class="openhours-contact-container">
              <p>Volgens afspraak op:</p>
              <p>Maandag - vrijdag</p>
              <p>08:30 - 11:00</p>
              <p>13:15 - 14:00</p>
              <p>19:15 - 20:00</p>
            </div>
        
            <div class="phone-email-container">
              <p>info@dierenartsverboom.nl</p>
              <p>0113 - 290800</p>
            </div>

            <div class="adres-container">
              <p>Karmijnstraat 19</p>
              <p>4421 LC</p>
              <p>Kapelle</p>
            </div>

          </div>
        
        </div>

        <div class="iframe-container-mobile">
          <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2484.403381040776!2d3.9506826930389574!3d51.48746472298837!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0xcaaa1f19c40cd5%3A0x160cbd6a6e4c6c77!2sDierenartsenpraktijk%20Verboom!5e0!3m2!1snl!2snl!4v1672146833551!5m2!1snl!2snl" width="220" height="220" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
        </div>
        <div class="iframe-container-tablet">
          <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2484.403381040776!2d3.9506826930389574!3d51.48746472298837!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0xcaaa1f19c40cd5%3A0x160cbd6a6e4c6c77!2sDierenartsenpraktijk%20Verboom!5e0!3m2!1snl!2snl!4v1672146833551!5m2!1snl!2snl" width="250" height="250" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
        </div>
        <div class="iframe-container-desktop">
          <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2484.403381040776!2d3.9506826930389574!3d51.48746472298837!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0xcaaa1f19c40cd5%3A0x160cbd6a6e4c6c77!2sDierenartsenpraktijk%20Verboom!5e0!3m2!1snl!2snl!4v1672146833551!5m2!1snl!2snl" width="370" height="370" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
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
    title: 'Dierenarts Verboom'
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

  padding-bottom: 100px;
}

.container-about > h1 {
  font-size: 18px;
  font-weight: 600;

  margin-bottom: 10px;
}

.container-about {
  display: flex;
  flex-direction: column;
  gap: 0px;
}

.container-contact {
  display: flex;
  flex-direction: column;
  gap: 25px;
}

.iframe-container-tablet {
  display: none;
}

.iframe-container-desktop {
  display: none;
}

@media (min-width: 560px) {
  .iframe-container-mobile {
    display: none;
  }

  .iframe-container-tablet {
    display: flex;
  }
}

@media (min-width: 940px) {   
  main > .container-main {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
        
    margin-top: 45px;
    margin-left: 75px;
    margin-right: 45px;
        
    padding-bottom: 200px;
  }
        
  .container-about {
    display: flex;
    flex-direction: column;
  }

  .iframe-container-mobile {
    display: none;
  }

  .iframe-container-tablet {
    display: none;
  }

  .iframe-container-desktop {
    display: flex;
  }
}

@media (min-width: 1200px) {
  .iframe-container-desktop {
    margin-right: 100px;
  }
}

@media (min-width: 1400px) { 

  main > .container-main {
    display: flex;
    flex-direction: row;
    gap: 500px;
        
    margin-top: 65px;
    margin-left: 150px;
    margin-right: 45px;
        
    padding-bottom: 250px;
  }

  .container-about {
    display: flex;
    flex-direction: column;
  }

  .container-about > h1 {
    font-size: 20px;
    font-weight: 600;
        
    margin-bottom: 15px;
  }
}
</style>