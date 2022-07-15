<template>
  <footer>
    <section class="container-fluid ms_top-footer">
        <div class="container">


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

<style lang="scss">
@import "../styles/variables.scss";
@import "../styles/mixins.scss";

section.ms_top-footer{
    height: 350px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
}


section.ms_bottom-footer{
    height: 100px;
    background-color: $footerColor;
}
</style>