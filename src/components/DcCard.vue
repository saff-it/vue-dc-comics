<template>

    <div class="ms_dc-card">
        <div class="ms_card-img">
            <img :src="card.thumb"
                alt="">
        </div>
        <h5>ACTION COMICS</h5>
    </div>

</template>

<script>

export default {
    props: ['card'],
}
</script>

<style>
</style>