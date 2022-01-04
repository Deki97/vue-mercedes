<template>
    <header>
        <div class="container">
            <div class="logo-left">
                <img src="https://car-brand-names.com/wp-content/uploads/2015/05/Mercedes-symbol-720x640.jpg" alt="Mercedes Logo">
            </div>

            <div class="logo-right">
                <img src="https://www.mercedes-benzcaribbean.com/assets/themes/mb-caribbean/media/stock_images/word-logo2b.png" alt="Mercedes Motto">
            </div>
        </div>
    </header>
</template>


<script>
export default {
    name: 'Header'
}
</script>


<style lang="scss" scoped>
@import '../style/variables.scss';

header {
    background-color: $page-primary-color;
    border-bottom: 1px solid lighten($page-primary-color, 30%);
    height: 95px;
    
    .container {
        display: flex;
        align-items: center;
        height: 100%;
    
        .logo-left {
            width: 100px;
        }

        .logo-right {
            width: 200px;
            margin-left: 40px;
        }
    }
}
</style>