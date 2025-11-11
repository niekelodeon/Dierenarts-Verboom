<template>
  <div class="container-main">
      
    <div class="container-bijsluiters">
      
      <h1>Bijsluiters Hond</h1>
    
      <div class="container-center">
    
        <div class="item" v-for="bijsluiter in bijsluiters" :key="bijsluiter.id" v-on:click="toggleActive">
          <div class="name">
            <h2>{{ bijsluiter.naam }}</h2>
            <svg width="21" height="15" viewBox="0 0 19 13" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M16.5983 2L9.29916 9L2.00005 2" stroke="#545454" stroke-width="5" />
            </svg>
          </div>
    
          <div class="content">
            <a :href="bijsluiter.link" target="_blank">Bekijk PDF</a>
          </div>
        </div>
    
      </div>
            
    </div>
      
  </div>
</template>
    
<script>
export default {
  name: 'DuifComponent',

  data() {
    return {
      bijsluiters: [],
      jsonUrl: 'https://www.dierenartsverboom.nl/data/bijsluiters-hond.json',
    }
  },

  created() {
    this.fetchData()
  },

  methods: {
    fetchData() {
      fetch(this.jsonUrl)
        .then(response => {
          if (!response.ok) {
            throw new Error('Network response was not ok')
          }
          return response.json()
        })
        .then(data => {
          console.log(data)
          this.bijsluiters = data['bijsluiters-hond']
        })
        .catch(error => {
          console.log(error)
        })
    },

    toggleActive(event) {
      const currentItem = event.currentTarget
      currentItem.classList.toggle('active')
    },
  },
}
</script>
      
<style>
/* Font Import */
    
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&display=swap');
    
.container-bijsluiters {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
        
.container-bijsluiters > h1 {
  font-size: 18px;
  font-weight: 600;
        
  margin-bottom: 20px;
}
        
.container-center {
  display: flex;
  flex-direction: column;
  gap: 15px;
}
        
.item {
  min-width: 300px;
        
  background-color: #F5F5F5;
  border: 2px solid #D7D7D7;
  cursor: pointer;
}
        
.name {
  display: flex;
  justify-content: space-between;
  align-items: center;
        
  padding: 10px;
}
        
.name > h2 {
  font-size: 16px;
  font-weight: 500;
}
        
.content {
  max-height: 0;
  overflow: hidden;
  transition: 0.3s;
}
        
.content p {
  line-height: 1.4;
  font-size: 16px;
        
  padding: 10px;
}
        
.content a {
  line-height: 1.4;
  font-size: 16px;
        
  padding-bottom: 10px;
  padding-left: 10px;
}
        
.item.active > .content {
  max-height: 300px;
  transition: 0.3s;
}
        
.item svg {
  transform: rotate(0deg);
  transition: transform 0.3s;
}
        
.item.active svg {
  transform: rotate(180deg);
  transition: transform 0.3s;
}
        
@media (min-width: 800px) { 
  .name > h2 {
    font-size: 18px;
  }
        
  .item svg {
    height: 35px;
    width: 25px;
  }
}
        
@media (min-width: 940px) {     
  main > .container-main {
    margin-top: 45px;
    margin-inline: 45px;
                
    padding-bottom: 100px;
  } 
        
  .container-center {
    gap: 25px;
  }
}
        
@media (min-width: 1400px) {       
  main > .container-main {
    margin-top: 65px;
    margin-inline: 45px;
                
    padding-bottom: 100px;
  }
        
  .container-bijsluiters > h1 {
    font-size: 20px;
    font-weight: 600;
                
    margin-bottom: 25px;
  }
}
</style>