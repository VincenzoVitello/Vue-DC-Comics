<template>
    <div class="main_container">
        <div class="content">
            <TopSection />
            <BottomSection/>
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
    .main_container{
        width: 100vw;
    }
    .content{
        height: 100%;
        width: 100%;
        color: white;
        font-size: 25px;
        align-items: center;
    }
</style>