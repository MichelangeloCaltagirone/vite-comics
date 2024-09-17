<script>
    export default {
        data() {
            return {
            }
        },
        props: {
            picUrl: {
                type: String,
                required: true
            },
            price: {
                type: String,
                required: false
            },
            title: {
                type: String,
                required: true
            },
            bookType: {
                type: String,
                required: false
            }
        },
        metspands: { 
            getImageUrl(picPath) {
                return new URL(`../assets/img/${picPath}`, import.meta.url).href
            }
        }

    }
</script>

<template>
    <article>
        <div>
            <img :src="picUrl" :alt="title">
        </div>
        
        <span>{{ title.toUpperCase() }}</span>
    </article>
   
</template>

<style scoped>
article {
    flex-basis: calc(100% / 6);
    padding: 0 10px;
    div {
        height: 150px;
        margin: 1rem 0 1.5rem 0;
    }
    img {
        width: 100%; 
        max-height: 100%;
    }
    span {
        font-size: 16px;
        color: #FEFEFE;
    }
    }
</style>