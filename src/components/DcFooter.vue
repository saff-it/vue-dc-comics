<template>
  <footer>
    <section class="container-fluid ms_top-footer">
        <div class="container">
            <div class="ms_footer-list-menu">

                <div class="left-list">
                    <h4>Dc Comics</h4>

                    <ul>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                    </ul>

                    <h4>Shop</h4>

                    <ul>
                        <li>Characters</li>
                        <li>Characters</li>
                    </ul>

                </div>

                <div class="middle-list">
                    <h4>Dc</h4>

                    <ul>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                    </ul>
                </div>

                <div class="right-list">
                    <h4>Sites</h4>

                    <ul>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>
                        <li>Characters</li>

                    </ul>
                </div>

            </div>

            <div class="footer-logo">
                <img src="../assets/img/dc-logo-bg.png" alt="dc logo big">
            </div>

        </div>
    </section>

    <section class="container-fluid ms_bottom-footer">
        <div class="container">

        </div>
    </section>

  </footer>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import "../styles/variables.scss";
@import "../styles/mixins.scss";

section.ms_top-footer{
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;

    div.container{
        @include flex-hor-center;
        justify-content: space-between;
    }
}

div.ms_footer-list-menu{
    display: flex;
    width: 40%;

    div{
        width: calc(100% / 3);
    }

}


h4{
    color: white;  
}

ul{
    list-style: none;
    color: rgb(114, 111, 111);
    margin: 15px 0;
    padding: 0;

    li{
        margin-top: 4px;
    }
}

section.ms_bottom-footer{
    height: 100px;
    background-color: $footerColor;
}

</style>