<template>
  <div class="container-root">
    
    <header>
      <div class="header-container">

        <img class="logo-small" src="../assets/logo-small.png" alt="logo-small">
        <img class="logo-big" src="../assets/logo-big.png" alt="logo-big">

        <div class="second-container-hamburger">
          <div class="hamburger-container">
            <button class="hamburger" :class="{ 'is-active': isActive }" @click="toggleMenu">
              <div class="bar"></div>
            </button>
          </div>
        </div>

        <div class="second-container-info">

          <div class="info-container">
            <div class="phone-container">
              <img src="../assets/phone.png" alt="telefoon">
              <p class="p-phone">0113-290800</p>
            </div>

            <div class="openhours-container">
              <img src="../assets/openhours.png" alt="openingsuren">
              <div class="openhours-container-2">
                <p class="p-openhours-1">op afspraak ma - vr</p>
                <p class="p-openhours-2">08:30 - 11:00</p>
                <p class="p-openhours-3">13:15 - 14:00</p>
                <p class="p-openhours-4">19:15 - 20:00</p>
              </div>
            </div>

            <div class="location-container">
              <img src="../assets/location.png" alt="locatie">
              <div class="location-container-2">
                <p class="p-location-1">Karmijnstraat 19</p>
                <p class="p-location-2">4421 LC</p>
                <p class="p-location-3">Kapelle</p>
              </div>
            </div>
          </div>

        </div>

      </div>
    
      <div class="sub-header">

        <div class="info-container-mobile">
          <div class="phone-container-mobile">
            <img src="../assets/phone.png" alt="telefoon">
            <p class="p-phone">0113-290800</p>
          </div>
    
          <div class="openhours-container-mobile">
            <img src="../assets/openhours.png" alt="openingsuren">
    
            <div class="openhours-container-2-mobile">
              <p class="p-openhours-1-mobile">op afspraak ma - vr</p>
              <p class="p-openhours-2-mobile">08:30 - 11:00</p>
              <p class="p-openhours-3-mobile">13:15 - 14:00</p>
              <p class="p-openhours-4-mobile">19:15 - 20:00</p>
            </div>
          </div>

          <div class="location-container-mobile">
            <img src="../assets/location.png" alt="locatie">
    
            <div class="location-container-2-mobile">
              <p class="p-location-1">Karmijnstraat 19</p>
              <p class="p-location-2">4421 LC</p>
              <p class="p-location-3">Kapelle</p>
            </div>
          </div>
    
        </div>

      </div>

      <nav>
        <NuxtLink to="/" exact class="nav-link" active-class="a-active">Home</NuxtLink>
        <NuxtLink to="/over" exact class="nav-link" active-class="a-active">Over ons</NuxtLink>
        <NuxtLink to="/bijsluiters" exact-active-class="nav-link" active-class="a-active">Bijsluiters</NuxtLink>
        <NuxtLink to="/hillsvoeding" exact class="nav-link" active-class="a-active">Hill's voeding</NuxtLink>
        <NuxtLink to="/duiven" exact class="nav-link" active-class="a-active">Duiven</NuxtLink>
        <NuxtLink to="/contact" exact class="nav-link" active-class="a-active">Contact</NuxtLink>
      </nav>
      <div class="mobile-nav" :class="{ 'is-active': isActive }" :style="{ overflow: isActive ? 'hidden' : 'auto' }">
        <div class="mobile-nav-second">
          <NuxtLink to="/" exact class="nav-link" active-class="a-active" @click="closeMenu">Home</NuxtLink>
          <NuxtLink to="/over" exact class="nav-link" active-class="a-active" @click="closeMenu">Over ons</NuxtLink>
          <NuxtLink to="/bijsluiters" exact-active-class="nav-link" active-class="a-active" @click="closeMenu">Bijsluiters</NuxtLink>
          <NuxtLink to="/hillsvoeding" exact class="nav-link" active-class="a-active" @click="closeMenu">Hill's voeding</NuxtLink>
          <NuxtLink to="/duiven" exact class="nav-link" active-class="a-active" @click="closeMenu">Duiven</NuxtLink>
          <NuxtLink to="/contact" exact class="nav-link" active-class="a-active" @click="closeMenu">Contact</NuxtLink>
        </div>
        <div class="under-section">
          <p id="copyright-mb" class="copyright-mb">&copy; {{ currentYear }} Dierenarts Verboom & de Kok</p>
        </div>
      </div>
  
    </header> 
  
    </div>
  
</template>
  
<script>
export default {
  name: 'HeaderComponent',
  data() {
    return {
      isActive: false,
      currentYear: new Date().getFullYear(),
    }
  },

  mounted() {
    this.$router.afterEach(() => {
      this.closeMenu()
    })
  },
  methods: {
    toggleMenu() {
      this.isActive = !this.isActive
      document.body.style.overflow = this.isActive ? 'hidden' : 'auto'
      window.scrollTo(0, 0)
    },

    closeMenu() {
      this.isActive = false
      document.body.style.overflow = 'auto'
      window.scrollTo({ top: 0 })
    },
  },
}
</script>
 
<style>
/* Font Import */
  
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap');
  
/* Header */
  
.header-container {
  display: flex;
  flex-direction: row;
  
  margin-top: 10px;
}
  
@media (min-width: 560px) {
  .header-container {
    margin-top: 15px;
  }
}
  
/* Header logo */
  
.logo-big {
  display: none;
}
  
.second-container-hamburger {
  width: 100%;
}
  
.hamburger-container {
  height: 100%;
  
  border-bottom: 15px solid var(--main-orange);
}
  
@media (min-width: 560px) {
  .logo-small {
    display: none;
  }
  
  .logo-big {
    display: block;
  }
  
  .hamburger-container {
    height: 100%;
        
    border-bottom: 21px solid var(--main-orange);
  }
}
  
@media (min-width: 800px) {
  .second-container-hamburger {
    display: none;
  }
}
  
/* Hamburger icon */
  
.hamburger {
  position: relative;
  float: right;
  
  width: 35px;
  margin-top: 20px;
  margin-right: 30px;
  
  cursor: pointer;
  appearance: none;
  background: none;
  outline: none;
  border: none;
  
  animation: fadeIn 0.3s;
}
  
.hamburger.is-active > .bar {
  background-color: var(--main-orange);
  
  transform: translate(15px, 0); 
  transition: 0.3s all ease-in-out;
}
  
.hamburger.is-active::before {
  transform: rotate(-45deg) translate(-9px, 6px);
}
  
.hamburger.is-active::after {
  transform: rotate(45deg) translate(-9px, -7px);
}
  
.bar, .hamburger::after, .hamburger::before {
  content: '';
  display: block;
  transition: 0.2s;
    
  width: 100%;
  height: 5px;
  
  margin: 6px 0px;
        
  background-color: #545454;
}
  
.hamburger.is-active .bar {
  opacity: 0;
}
  
@media (min-width: 350px) {
  .hamburger {
    margin-right: 15px;
  }
}
  
@media (min-width: 400px) {
  .hamburger {
    margin-right: 25px;
  }
}
  
@media (min-width: 560px) {
  .hamburger {
    margin-right: 35px;
    margin-top: 40px;
  }
}
  
@media (min-width: 800px) {
  .hamburger {
    display: none;
    margin-right: 35px;
    margin-top: 50px;
  }
}
  
/* Navigation menu mobile */
  
header, .header-container, .sub-header {
  z-index: 99;
}
  
.mobile-nav {
  display: flex;
  flex-direction: column;
          
  position: fixed;
  top: 108px;
  bottom: 0;
  left: 100%;
  
  width: 100%;
  
  background-color: #fff;
  
  z-index: 1;
        
  transition: 0.3s;
  
  min-height: 100vh;
}
  
@media (min-height: 600px) {
  .mobile-nav {
    gap: 30px;
  }
}
  
@media (min-height: 650px) {
  .mobile-nav {
    gap: 60px;
  }
}
  
@media (min-height: 700px) {
  .mobile-nav {
    gap: 110px;
  }
}
  
@media (min-height: 750px) {
  .mobile-nav {
    gap: 160px;
  }
}
  
@media (min-height: 800px) {
  .mobile-nav {
    gap: 210px;
  }
}
  
@media (min-height: 850px) {
  .mobile-nav {
    gap: 260px;
  }
}
  
.mobile-nav-second {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  gap: 15px;
  padding-top: 25px;
}
  
.mobile-nav-second > a {
  text-align: center;
        
  width: 100%;
  padding: 12px 16px;
  
  color: var(--text-black);
  
  text-decoration: none;
  font-size: 18px;
  font-weight: 600;
}
  
.mobile-nav-second > a:hover {
  color: var(--main-orange-hover);
  transition: 0.2s;
}
  
.mobile-nav-second > .a-active:hover {
  color: var(--main-green);
}
  
.mobile-nav-second > .a-active {
  color: var(--main-green)
}
  
.mobile-nav.is-active {
  position: absolute;
  top: 108px; 
  left: 0;
  
  animation: fadeIn 0.4s;
}
  
.under-section {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 5px;
  
  width: 100%;
  height: 100%;
  border-top: solid 6px var(--main-green);
}
  
.copyright-mb {
  margin-top: 40px;
  
  font-size: 14px;
  font-weight: 400;
}
  
.made-by, .made-by > a {
  margin-bottom: 20px;
  
  font-weight: 400;
  font-size: 14px;
}
  
@media (min-width: 560px) {
  .mobile-nav {
    top: 152px;
  }
  
  .mobile-nav.is-active {
    top: 152px;
    left: 0;
  
    min-height: 100vh;
  } 
  
  .mobile-nav-second {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    gap: 35px;
    padding-top: 45px;
  }
  
  .mobile-nav-second > a {
    text-align: center;
            
    width: 100%;
    padding: 12px 16px;
        
    color: var(--text-black);
        
    text-decoration: none;
    font-size: 22px;
    font-weight: 600;
  }
}
  
@media (min-width: 800px) {
  .mobile-nav {
    display: none;
  }
}
  
/* Information */
  
.second-container-info {
  display: none;
}
  
@media (min-width: 800px) {
  .second-container-info {
    display: block;
    width: 100%;
  }
  
  .info-container {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    align-items: center;
  
    height: 100%;
  
    border-bottom: 21px solid var(--main-orange);        
  } 
  
  .phone-container, .openhours-container, .location-container {
    display: flex;
    align-items: center;
    text-align: center;
    gap: 10px;
  }
  
  .location-container-2 > p {
    font-weight: 500;
    font-size: 17px;
  }
  
  .phone-container > p {
    font-weight: 500;
    font-size: 17px;
  }
  
  .location-container {
    display: none;
  }
        
  .openhours-container {
    text-align: center;
  }
  
  .openhours-container-2 > p {
    font-weight: 500;
    font-size: 17px;
  }
  
  /* Aligning info */
  
  .p-openhours-1 {
    position: relative;
    right: 4px;
  }
  
  .p-openhours-2 {
    position: relative;
    right: 1px;
  }
  
  .p-openhours-3 {
    position: relative;
    left: 2px;
  }
  
  .p-openhours-4 {
    position: relative;
    left: 3px;
  }
}
  
@media (min-width: 1000px) {
  .location-container {
    display: flex;
  }
}
  
/* Sub header */
  
.info-container-mobile {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  width: 100%;
  
  padding: 12.5px 0;
        
  min-height: 90px;
  border-bottom: 4px solid var(--main-green);
}
  
.phone-container-mobile, .openhours-container-mobile, .location-container-mobile {
  display: flex;
  align-items: center;
  text-align: center;
  gap: 10px;
}
  
.p-phone {
  font-size: 16px;
  font-weight: 500;
}
  
.openhours-container-2-mobile > p {
  font-size: 16px;
  font-weight: 500;
}
  
.location-container-2-mobile > p {
  font-size: 16px;
  font-weight: 500;
}
  
.location-container-mobile {
  display: none;
}
  
/* Aligning mobile info */
  
.p-openhours-1-mobile {
  position: relative;
  right: 5px;
}
  
.p-openhours-2-mobile {
  position: relative;
  right: 2px;
}
  
.p-openhours-3-mobile {
  position: relative;
  left: 1px;
}
  
.p-openhours-4-mobile {
  position: relative;
  left: 2px;
} 
  
/* resizing icons */
  
.phone-container-mobile > img {
  width: 30px;
  height: 30px;
}
  
.openhours-container-mobile > img {
  width: 30px;
  height: 30px;
}
  
.location-container-mobile > img {
  width: 30px;
  height: 30px;
}
  
@media (min-width: 800px) {
  .info-container-mobile {
    display: none;
  }
}
  
@media (min-width: 560px) {
  .location-container-mobile {
    display: flex;
  }
}
  
/* Sub header navigation */
  
nav {
  display: none;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  
  padding: 12.5px 0;
        
  min-height: 90px;
  border-bottom: 7px solid var(--main-green);
}
  
nav > a {
  color: var(--text-black);
  
  font-size: 20px;
  font-weight: 600;
  text-decoration: none;  
}
  
nav > a:hover {
  color: var(--main-orange-hover);
  transition: 0.2s;
}
  
nav > .a-active {
  color: var(--main-green)
}
  
nav > .a-active:hover {
  color: var(--main-green)
}
  
@media (min-width: 800px) {
  nav {
    display: flex;
  }
}
</style>
  