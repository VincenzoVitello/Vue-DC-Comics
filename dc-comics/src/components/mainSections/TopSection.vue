<template>
<div class="container_top_section">

  <div class="jumbo_container"></div>

</div>
</template>

<script>

export default {
    name: "TopSection",
}
</script>

<style lang="scss" scoped>
   @import '../../assets/style/global.scss';
   @import '../../assets/style/variables.scss';
   .container_top_section{
     display: flex;
     flex-direction: column;
     height: 500px;
   }
   .jumbo_container{
     background-image: url('../../assets/img/jumbotron.jpg');
     background-size: cover;
     height: 100%;
     width: 100%;
   }
   .current_series{
     background-color: $mainColor;
     width: 100vw;
     text-align: center;
     text-transform: uppercase;
     padding: 5px;
   }
</style>