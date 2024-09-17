<script>
</script>

<template>
    <div class="bg">
        <div class="container">

            <div>
                <button id="btnSingUpNow"><a href="#">SIGN-UP NOW!</a></button>
                <div class="footerMediaGroup">
                    <a id="linkFollowUs" href="#">FOLLOW US</a>
                    <span>ciao</span>
                    <span>ciao</span>
                    <span>ciao</span>
                    <span>ciao</span>
                    <span>ciao</span>
                    <span>ciao</span>
                </div>
            </div>

        </div>
    </div>    
</template>

<style scoped>
a {
    text-decoration: none;
}
.bg {
    background-color: #303030;
    position: relative;
    z-index: 1;
}
.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 1rem 0;
    
    & div:first-child {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
}
.footerMediaGroup {
    display: flex;
    gap: 10px;
}
#btnSingUpNow {
    padding: 10px 15px;
    background-color: transparent;
    border: 1px solid aqua;
    a {
        color: white;
    }
}
#linkFollowUs {
    color: aqua;
    font-weight: bold;
}

</style>