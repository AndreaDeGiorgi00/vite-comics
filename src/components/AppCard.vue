<script>
export default {
    name: "cards",
    props: { store: Array },

}
</script>


<template>

    <div v-for="i in store" class="card">
        <div class="img-container">

            <img :src="i.thumb" alt="copertina">
        </div>
        <h4>{{ i.series }}</h4>
    </div>
</template>



<style scoped lang="scss">
@use "../assets/scss/variables" as *;
@use "../assets/scss/partials" as *;


.card {
    width: calc(100% / 6 - 20px);
    height: 200px;
    margin: 20px 0;

}

.img-container {
    height: 168px;
    width: 100%;
    overflow: hidden;
}

h4 {
    margin: 10px 0;
    color: white;

}
</style>