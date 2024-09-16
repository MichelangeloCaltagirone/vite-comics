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
  <header>

      <img src="../assets/img/dc-logo.png" alt="logo DC">
      
      <nav>
        
        <a v-for="link in headerLinks" href="http://#">{{ link.toUpperCase() }}</a>

      </nav>


  </header>
</template>

<style scoped>

header {
  display: flex;
  justify-content: space-between;

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

  &:hover {
    color: aqua;
    border-bottom: 2px solid aqua;
  }
}

</style>
