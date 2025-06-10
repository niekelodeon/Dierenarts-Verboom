<template>
  <div class="container-root">

  <!-- Meta Tags -->
  <Head>
    <Title>Dierenarts Verboom - Bijsluiters</Title>

    <Link rel="canonical" href="https://www.dierenartsverboom.nl/bijsluiters"/>
  </Head>

  <HeaderComponent />

  <main>

    <div class="container-main">

      <h1>Bijsluiters</h1>

        <div class="container-above">

          <div class="animal">
            <NuxtLink to="/bijsluiters/hond" exact class="nav-link">
              <img src="../../assets/hond.png">
              <h2>Hond</h2>
            </NuxtLink>
          </div>
                        
          <div class="animal">
            <router-link to="/bijsluiters/kat" exact class="nav-link">
              <img src="../../assets/kat.png">
              <h2>Kat</h2>
            </router-link>
          </div>

        </div>

        <div class="container-below">

          <div class="animal">
            <router-link to="/bijsluiters/konijn" exact class="nav-link">
              <img src="../../assets/konijn.png">
              <h2>Konijn</h2>
            </router-link>

          </div>

          <div class="animal">
            <router-link to="/bijsluiters/duif" exact class="nav-link">
              <img src="../../assets/duif.png">
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
    title: 'Dierenarts Verboom'
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