<template>
    <main>

        <section class="container-fluid ms_main-sect">

            <div class="container ms_main-contents">
                > Content goes here --
            </div>

        </section>

        <section class="container-fluid ms_bottom-main">
            <div class="container ms_bottom-main-bar"
                v-for="(product, index) in products"
                :key="index"
            >
                <ul>
                    <li>
                    <img :src="require(`..assets/img/buy-${product.img}`)" :alt="product.text"> {{product.text}}</li>
                </ul>
            </div>
        </section>

    </main>
</template>

<script>
export default {
    data: function(){
        return {
            products: [
                {
                    text: 'digital comics',
                    img: 'comics-digital-comics.png',
                },{
                    text: 'dc merchandise',
                    img: 'comics-merchandise.png',
                },{
                    text: 'subscription',
                    img: 'comics-subscriptions.png',
                },{
                    text: 'comic shop locator',
                    img: 'comics-shop-locator.png',
                },{
                    text: 'dc power visa',
                    img: 'dc-power-visa.svg',
                },
            ],
        };
    },
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
            margin: 0;
            padding: 0;

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