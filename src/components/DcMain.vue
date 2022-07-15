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
        display: flex;
        align-items: center;
        height: 110px;
        color: white;
        font-size: 25px;

    }

}

div.ms_bottom-main-bar ul{
    list-style: none;

        li{
            @include hor-list-setup;
            margin: 0 14px;
        }

}


</style>