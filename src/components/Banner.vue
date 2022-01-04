<template>
    <div class="banner">
        <img src="https://wallpapersmug.com/large/a45232/black-car.jpg" alt="Mercedes Banner">
    </div>
</template>


<script>
export default {
    name: 'Banner'
}
</script>


<style lang="scss" scoped>
.banner img {
    width: 100%;
    height: calc(100vh - 95px);
    object-fit: cover;
    object-position: bottom;
}
</style>