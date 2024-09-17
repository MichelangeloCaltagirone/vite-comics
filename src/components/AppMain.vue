<script>
import ComicsCard from '../components/ComicsCard.vue';
 export default {
        data() {
            return {

            }
        },
        components: {
            ComicsCard
        }
    }

</script>

<template>
    <main>

        <div class="container">
            <h1>--> Contents Goes Here <--</h1>
            <ComicsCard />
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
    }

</style>
