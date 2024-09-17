<script>
export default {
        data() {
            return {
                mainLinks: [
                    {
                        picPath: 'buy-comics-digital-comics.png',
                        text: 'Digital Comics'
                    },
                    {
                        picPath: 'buy-comics-merchandise.png',
                        text: 'Comics Merchandise'
                    },
                    {
                        picPath: 'buy-comics-subscriptions.png',
                        text: 'Subscription'
                    },
                    {
                        picPath: 'buy-comics-shop-locator.png',
                        text: 'Comic Shop Locator'
                    },
                    {
                        picPath: 'buy-dc-power-visa.svg',
                        text: 'DC Power-Visa'
                    },
                ]
            }
        },
        methods: {
            getImageUrl(picPath) {
                return new URL(`../assets/img/${picPath}`, import.meta.url).href
            }
        }
    }

</script>


<template>

<div class="bg">
    <div  class="container">

      <div v-for="link in mainLinks">
         <img :src="getImageUrl(link.picPath)" alt="{{ link.text }}">
         <a href="#">{{ link.text }}</a>
      </div>

    </div> 
</div>
    

</template>


<style scoped>

a {
    text-decoration: none;
    color: white;
    padding-left: 10px;
    &:hover {
        scale: 1.1;
    }
}
img {
    width: 40px;
}
.bg {
    background-color: #0282F9;
    padding: 2rem 0;
}
.container {
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    justify-content: space-around;
    color: white;
    position: relative;
    z-index: 1;

    div {
        display: flex;
        align-items: center;
    }
  }

</style>