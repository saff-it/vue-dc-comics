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

<style>

div.ms_dc-card {
    width: calc(100% / 6);


}


</style>