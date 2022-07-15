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
                    <li>Digital Comics</li>
                    <li>Dc Merchandise</li>
                    <li>Subscription</li>
                    <li>Comic Shop Locator</li>
                    <li>Dc power Visa</li>
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
            }
        }
    }
}

</style>