<script>

export default {
    data() {
        return {
            bigData: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false,
                },
            ]
        }
    },
    methods: {
        getActive(element) {
            if (element.current) {
                return "active"
            } else {
                return "notActive"
            }
        },
        makeActive(element) {
            for (let x = 0; x < this.bigData.length; x++) {
                if (this.bigData[x].current) {
                    this.bigData[x].current = false;
                }
            }
            element.current = true;
        }
    },
    name: "main header"
}



</script>

<template>
    <section>

        <div class="container">
            <img src="img/dc-logo.png" alt="">

            <ul>
                <li v-for="i in bigData" :class="getActive(i)" :key="i.text" v-on:click="makeActive(i)">
                    <a :class="getActive(i)" :href="i.url">{{ i.text }}</a>
                </li>

            </ul>

        </div>
    </section>
</template>

<style lang="scss" scoped>
@use "../assets/scss/variables" as *;
@use "../assets/scss/partials" as *;

.container {
    @include contenitore;
    @include display-flex-just-sp-bt;
    height: 90px;
    background-color: white;

    ul {
        @include display-flex-just-sp-bt;
        width: 66%;
    }
}

li {
    @include display-flex-full-center;
    list-style-type: none;
    height: 100%;
    text-align: center;
    border-bottom: 5px solid white;



}

a {
    text-decoration: none;
    color: black;
    cursor: pointer;
    font-size: 20px;
}

.active {
    border-color: #0C7CEC;
    color: #0C7CEC;

}
</style>