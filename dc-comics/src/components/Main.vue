<template>
    <div class="container">
        <div class="content">
            -->Content goes here!
        </div>
    </div>
</template>

<script>
export default {
    name: 'Main'
}
</script>

<style lang="scss" scoped>
    @import '../assets/style/variables.scss';
    .content{
        width: 1000px;
        height: 100px;
        color: white;
        font-size: 25px;
        display: flex;
        align-items: center;
    }
    .container{
        background: $secondaryColor;
        justify-content: center;
    }
</style>