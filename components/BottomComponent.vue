<template>
  <div class="container-root">

    <footer>
      <div class="bottom-container">
      
        <div class="line-above"></div>
          <div class="socials">
      
            <div class="facebook">
              <img src="../assets/facebook.png" alt="fb">
              <a href="https://m.facebook.com/profile.php?id=100084778803917">Dierenarts Verboom</a>
            </div>
      
            <div class="instagram">
              <img src="../assets/instagram.png" alt="ig">
              <a href="https://instagram.com/dierenartspraktijkverboom/">dierenartspraktijkverboom</a>
            </div>
      
          </div>
      
          <p id="copyright" class="copyright">&copy; {{ currentYear }} Dierenarts Verboom</p>
      
        </div>
    </footer>
  </div>
</template>
  
<script>
export default {
  name: 'BottomComponent',
  
  data() {
    return {
      isActive: false,
      currentYear: new Date().getFullYear(),
    };
  },
}
</script>
  
<style>
/* Font Import */
    
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap');
    
/* Footer */
  
footer {
  width: 100%;
  
  animation: fadeIn 0.35s;
}
  
.line-above {
  height: 6px;
  width: 100%;
  
  background-color: var(--main-green);
}
  
/* Facebook & Instagram */
  
.socials {
  display: flex;
  flex-direction: column;
  gap: 10px;
  
  padding: 15px 0 15px 25px;
}
  
.facebook, .instagram {
  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 7.5px;
}
  
.facebook > img {
  height: 20px;
  width: 20px;
}
  
.instagram > img {
  height: 20px;
  width: 20px;
}
  
.facebook > a {
  color: var(--text-black);
  font-size: 14px;
  font-weight: 600;
  
  text-decoration: none;
}
  
.instagram > a {
  color: var(--text-black);
  font-size: 14px;
  font-weight: 600;
  
  text-decoration: none;
}
  
@media (min-width: 560px) {
  .socials {
    padding: 25px 0 5px 35px;
  }
  
  .facebook, .instagram {
    gap: 12.5px;
  }
  
  .facebook > img {
    height: 30px;
    width: 30px;
  }
  
  .instagram > img {
    height: 30px;
    width: 30px;
  }
  
  .facebook > a {
    font-size: 16px;
  }
  
  .facebook > a:hover {
    font-size: 16px;
  
    color: var(--main-green);
    transition: 0.3s;
  }
          
  .instagram > a:hover {
    font-size: 16px;
  
    color: var(--main-green);
    transition: 0.3s;
  }
          
  .instagram > a {
    font-size: 16px;
  }
}
  
/* Copyright */
  
.copyright {
  display: none;
}
  
@media (min-width: 560px) { 
  .copyright {
    display: flex;
    justify-content: flex-end;
              
    margin: 0 30px 15px;
  }
}
</style>