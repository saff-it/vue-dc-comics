<template>
    <main>

        <section class="container-fluid ms_main-sect">

            <div class="container ms_main-contents">
                > Content goes here --
            </div>

        </section>

        <section class="container-fluid ms_bottom-main">
            <div class="container ms_bottom-main-bar">
                <ul>
                    <li> <img src="../assets/img/buy-comics-digital-comics.png" alt="digital comics icon"> Digital Comics</li>
                    <li> <img src="../assets/img/buy-comics-merchandise.png" alt="digital comics icon"> Dc Merchandise</li>
                    <li> <img src="../assets/img/buy-comics-subscriptions.png" alt="digital comics icon"> Subscription</li>
                    <li> <img src="../assets/img/buy-comics-shop-locator.png" alt="digital comics icon"> Comic Shop Locator</li>
                    <li> <img src="../assets/img/buy-dc-power-visa.svg" alt="digital comics icon"> Dc power Visa</li>
                </ul>
            </div>
        </section>

    </main>
</template>

<script>
export default {

}
</script>

<style lang="scss">
@import "../styles/variables.scss";
@import "../styles/mixins.scss";


section.ms_main-sect {
    background-color: $bgColor;

    div.ms_main-contents {
        @include flex-hor-center;
        height: 110px;
        color: white;
        font-size: 25px;

    }

}

section.ms_bottom-main{
    background-color: $brandColor;
    
    div.ms_bottom-main-bar {
        height: 120px;
        @include flex-hor-center;

        ul{
            list-style: none;
            width: 100%;

            li{
                @include hor-list-setup;
                width: calc(100% / 5 - 30px);
                margin: 0 15px;
                color: white;
                text-align: center;

                img{
                    height: 40px;
                    margin-right: 10px;

                }
            }
        }
    }
}

</style>