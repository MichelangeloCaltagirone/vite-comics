<script>
import ComicsCard from '../components/ComicsCard.vue';
 export default {
        data() {
            return {
                comicsBooks: [
            {
                "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                "price": "$19.99",
                "series": "Action Comics",
                "type": "comic book"
            },
            {
                "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                "price": "$3.99",
                "series": "American Vampire 1976",
                "type": "comic book"
            },
            {
                "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                "price": "$16.99",
                "series": "Aquaman",
                "type": "graphic novel"
            },
            {
                "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                "price": "$2.99",
                "series": "Batgirl",
                "type": "comic book"
            },
            {
                "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                "price": "$3.99",
                "series": "Batman",
                "type": "comic book"
            },
            {
                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                "price": "$2.99",
                "series": "Batman Beyond",
                "type": "comic book"
            },
            {
                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                "price": "$3.99",
                "series": "Batman/Superman",
                "type": "comic book"
            },
            {
                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                "price": "$4.99",
                "series": "Batman/Superman Annual",
                "type": "comic book"
            },
            {
                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                "price": "$5.99",
                "series": "Batman: The Joker War Zone",
                "type": "comic book"
            },
            {
                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                "price": "$6.99",
                "series": "Batman: Three Jokers",
                "type": "comic book"
            },
            {
                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                "price": "$4.99",
                "series": "Batman: White Knight Presents: Harley Quinn",
                "type": "comic book"
            },
            {
                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                "price": "$16.99",
                "series": "Catwoman",
                "type": "graphic novel"
            }]
            }
        },
        components: {
            ComicsCard
        }
    }

</script>

<template>
    <section id="mainJumbotron"></section>
    <main>

        <div class="container">
            
            <section class="comicsBookList">
                <ComicsCard v-for="(comic, index) in comicsBooks" :key="index"
                :picUrl="comic.thumb"
                :price="comic.price"
                :title="comic.series"
                :bookType="comic.type" />
            </section>
            <span>CURRENT SERIES</span>
            <button id="btnLoadBookList">LOAD MORE</button>
            
        </div>   

    </main>
</template>

<style scoped>

    main {
        background-color: black;
        color: pink;
        padding: 3rem;
        font-size: 20px;
        
    }    
    .container {
    max-width: 1200px;
    margin: 0 auto;
    position: relative;
    }
    .comicsBookList {
        display: flex;
        flex-wrap: wrap;
    }
    #mainJumbotron {
        background-image: url(../assets/img/jumbotron.jpg);
        background-size: cover;
        height: 250px;
    }
    span {
        background-color: #0282F9;
        color: white;
        padding: 10px 25px;
        font-size: 20px;
        font-weight: bold;
        position: absolute;
        top: -3rem;
        left: 0;
        translate: 0 -50%;
    }
    #btnLoadBookList {
        padding: 10px 40px;
        background-color: #0282F9;
        color: white;
        font-size: 12px;
        font-weight: 500;
        display: block;
        margin: 2rem auto 0 auto;
    }

</style>
