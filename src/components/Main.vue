<template>
    <main>
        <Banner />

        <div class="container">
            <h2>Le nostre vetture</h2>
            <SingleMercedes />
        </div>

    </main>
</template>


<script>
import Banner from './Banner.vue';
import SingleMercedes from './SingleMercedes.vue';

export default {
    name: 'Main',
    components: {
        Banner,
        SingleMercedes
    }
}
</script>


<style lang="scss" scoped>
main {
    .container {
        h2 {
            font-size: 36px;
            margin: 50px 0;
        }
    }
}
</style>