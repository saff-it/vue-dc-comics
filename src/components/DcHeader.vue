<template>
  <header>
    <nav class="container">
        <div class="img-cont">
            <img class="h-100" src="../assets/img/dc-logo.png" alt="Dc Logo">
        </div>

        <div class="nav-bar">

            <ul>
                <li  v-for="(link, index) in headerNavLinks" :key="index">
                    <a class="ms_nav-link" href="link.url">{{link.text}}</a>
                </li>                
            </ul>

        </div>
    </nav>


  </header>
</template>

<script>
export default {
    data: function(){
        return {
            headerNavLinks: [
                {
                    text: 'characters',
                    url: '#',
                },{
                    text: 'comics',
                    url: '#',
                },{
                    text: 'movies',
                    url: '#',
                },{
                    text: 'tv',
                    url: '#',
                },{
                    text: 'games',
                    url: '#',
                },{
                    text: 'collectibles',
                    url: '#',
                },{
                    text: 'video',
                    url: '#',
                },{
                    text: 'fans',
                    url: '#',
                },{
                    text: 'news',
                    url: '#',
                },{
                    text: 'shop',
                    url: '#',
                },
            ],
        };
    },
    

}
</script>

<style lang="scss">
@import "../styles/mixins.scss";


nav{
    @include flex-hor-center;
    justify-content: space-between;
    

    div.img-cont{
    height: 90px;
    padding: 14px;
    }

}

div.nav-bar ul{
    list-style: none;
    margin: 0;
    

    li {
        @include hor-list-setup;
        margin: 0 14px;

        a{
            text-decoration: none;
            color: black;
        }
    }


}




</style>