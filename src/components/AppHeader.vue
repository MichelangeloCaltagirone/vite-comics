<script>
    export default {
        data() {
            return {
              headerLinks: ['characters',
                            'comics',
                            'movies',
                            'TV',
                            'Games',
                            'Collectibles',
                            'Videos',
                            'Fans',
                            'News',
                            'Shop'
                            ]
            }
        }
    }
</script>

<template>
   <div class="container">
    <header>   

      <img src="../assets/img/dc-logo.png" alt="logo DC">
      
      <nav>
        
        <a v-for="link in headerLinks" href="http://#">{{ link.toUpperCase() }}</a>

      </nav>
    
    </header>
  </div>
</template>

<style scoped>

header {
  padding: 1rem 0;
  display: flex;
  justify-content: space-between;

  img {
    width: 80px;
    height: 80px;
  }

  nav {
    display: flex;
    align-items: center;
  }
}

a {
  color: black;
  text-decoration: none;
  margin: 0 10px;
  font-size: 12px;
  font-weight: bold;

  &:hover {
    color: aqua;
    border-bottom: 2px solid aqua;
  }
}
.container {
    max-width: 1200px;
    margin: 0 auto;
  }

</style>
