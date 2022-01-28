<template>
    <div class="container">
        <div class="content">
            <TopSection />
            <BottomSection />
        </div>
    </div>
</template>

<script>
import TopSection from './mainSections/TopSection.vue'
import BottomSection from './mainSections/BottomSection.vue'

export default {
    name: 'Main',
    components:{
        TopSection,
        BottomSection,
    } 
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