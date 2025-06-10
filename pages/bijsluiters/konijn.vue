<template>
  <div class="container-root">

    <!-- Meta Tags -->
    <Head>
      <Title>Dierenarts Verboom - Bijsluiters Konijn</Title>
    </Head>
    
    <HeaderComponent />
    
    <main>
      <KonijnComponent />
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