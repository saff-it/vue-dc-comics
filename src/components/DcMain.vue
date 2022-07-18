<template>
    <main>

        <section class="container-fluid ms_main-sect">

            <div class="container ms_main-contents">
                > Content goes here --
            </div>

        </section>

        <section class="container-fluid ms_bottom-main">
            
            <div class="container">
                <div class="ms_bottom-main-bar"
                    v-for="(product, index) in products"
                    :key="index"
                >
                    <div>
                        <img :src="require(`../assets/img/buy-${product.img}`)" :alt="product.text">
                        
                    </div>
                    <h3> {{product.text}} </h3>
                                
                </div>
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
    
    
    div.container{
        display: flex;


       div.ms_bottom-main-bar {
            height: 120px;
            display: flex;
            align-items: center;
            justify-content: center;
            width: calc(100% / 5);
            
            

            div{
                color: white;
                text-align: center;
                margin: 0 15px;

                img{
                    height: 45px;
                    margin-right: 10px;
                }
            }

            h3{
                color: white;
                font-size: 14px;
                text-transform: uppercase;
            }
            
        } 
    }
        
}

</style>