<script>
 export default {
        data() {
            return {
                footerComicLinks: [
                    'Characters',
                    'Comics',
                    'Movies',
                    'TV',
                    'Games',
                    'Videos',
                    'News'
                    ],
                footerShopLinks: [
                    'Shop DC',
                    'Shop DC Collectibles'
                ],
                footerDCLinks: [
                    'Terms of use',
                    'Terms of use',
                    'Terms of use',
                    'Terms of use',
                    'Terms of use',
                    'Terms of use',
                    'Terms of use',
                    'Terms of use',
                    'Terms of use',
                    'Terms of use',
                    'Terms of use'
                ],
                footerSites: [
                    'DC',
                    'Mad Magazine',
                    'DC Kid',
                    'DC Universe',
                    'DC Power Visa'
                ]                
            }
        }
    }
</script>

<template>
     <footer>
        <div class="container">

            <div class="footerLinkLists">
                <div>
                    <span>DC COMICS</span>
                    <ul>
                        <li v-for="link in footerComicLinks"><a href="#">{{ link }}</a></li>
                    </ul>

                    <span>SHOP</span>
                    <ul>
                        <li v-for="link in footerShopLinks"><a href="#">{{ link }}</a></li>
                    </ul>
                </div>

                <div>
                    <span>DC</span>
                    <ul>
                        <li v-for="link in footerDCLinks"><a href="#">{{ link }}</a></li>
                    </ul>
                </div>

                <div>
                    <span>SITES</span>
                    <ul>
                        <li v-for="link in footerSites"><a href="#">{{ link }}</a></li>
                    </ul>
                </div>
            </div>
            <img id="footerDCLogo" src="../assets/img/dc-logo-bg.png" alt="DC logo">       
        </div>
    </footer>
</template>

<style scoped>

.container {
    max-width: 1200px;
    margin: 0 auto;
    position: relative;
}
ul {
    list-style-type: none;
    margin-top: 15px;
    margin-bottom: 15px;
}
a {
    text-decoration: none;
    color: #595B55;
    font-size: 12px;
    &:hover {
        opacity: 0.5;
    }
}
footer {
    background-image: url(../assets/img/footer-bg.jpg);
    color: white;
    padding: 2rem 0;
}
.footerLinkLists {
    display: flex;
    gap: 1.5rem;
}
#footerDCLogo {
    width: 450px;
    position: absolute;
    right: 120px;
    top: -100px
}

</style>
