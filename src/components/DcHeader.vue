<template>
  <header>
    <nav class="container">
        <div class="img-cont">
            <img class="h-100" src="../assets/img/dc-logo.png" alt="Dc Logo">
        </div>

        <div class="nav-bar">
            <ul>
                <li>Characters</li>
                <li>Comics</li>
                <li>Movies</li>
                <li>TV</li>
                <li>Games</li>
                <li>Collectibles</li>
                <li>Videos</li>
                <li>Fans</li>
                <li>News</li>
                <li>Shop</li>
            </ul>
        </div>
    </nav>


  </header>
</template>

<script>
export default {

}
</script>

<style lang="scss">

nav{
    display: flex;
    justify-content: space-between;
    align-items: center;

    div.img-cont{
    height: 90px;
    padding: 14px;
    }

}

div.nav-bar ul{
    list-style: none;

    li {
        display: inline-block;
        margin: 0 14px;
        font-size: 12px;
        font-weight: bold;
        text-transform: uppercase;
    }
}




</style>