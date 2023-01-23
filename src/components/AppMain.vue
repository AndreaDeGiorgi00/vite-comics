<script>

export default {


    name: "main",


}
</script>

<template>
    <section>
        <div class="contenitore">
            <div class="text">content Here</div>
        </div>
        <div class="contenitore blue">

        </div>
    </section>
</template>

<style lang="scss" scoped>
@use "../assets/scss/variables" as *;
@use "../assets/scss/partials" as *;

.contenitore {
    @include contenitore;
    height: 200px;
    display: flex;
    align-items: center;

    &.blue {
        height: 150px;

    }
}


.blue {
    background-color: #0282F9;
}

.text {
    width: 100%;
    background-color: black;
    color: white;
    padding-left: 30px;

}

section {
    background-color: black;
}
</style>