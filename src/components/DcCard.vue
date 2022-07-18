<template>

    <div class="ms_dc-card">
        <div class="ms_card-img">
            <img :src="singleCard.thumb" :alt="singleCard.type">
        </div>
        <h5>{{ singleCard.series }}</h5>
    </div>

</template>

<script>

export default {
    props: ['singleCard'],
}

</script>

<style lang="scss">

div.ms_card-img{
   
    img{
        height: 200px;
        width: 100%;
        object-fit: cover;
        object-position: top;
        padding: 12px;
    }
}

div.ms_dc-card {
    width: calc(100% / 6);
    

    h5{
        color: white;
        text-transform: uppercase;
        margin-top: 20px;
        font-size: 0.9rem;
        width: 80%;

    }
}


</style>