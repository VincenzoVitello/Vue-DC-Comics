<template>
  <div class="blueFooterContainer">
    <div class="container">
      <ul>
        <li v-for="(element, index) in links" :key="index"><a href="#"><img :src="element.imag" alt=""></a>{{element.text}}</li>
      </ul>
    </div>
    
  </div>
</template>

<script>
export default {
    name: 'Footer',
       data(){
     return {
         links: [
             {
                 text: "Digital Comics",
                 imag: require('../assets/img/buy-comics-digital-comics.png'),
                 current: false,
             },
             {
                 text: "DC Merchandise",
                 imag: require('../assets/img/buy-comics-merchandise.png'),
                 current: false,
             },
             {
                 text: "Subscription",
                 imag: require('../assets/img/buy-comics-subscriptions.png'),
                 current: false,
             },
             {
                 text: "Comic Shop Locator",
                 imag: require('../assets/img/buy-comics-shop-locator.png'),
                 current: false,
             },
             {
                 text: "DC Power Visa",
                 imag: require('../assets/img/buy-dc-power-visa.svg'),
                 current: false,
             },
             
         ]
     } //chiusura return
  } //chiusura data()
}
</script>

<style lang="scss" scoped>
@import '../assets/style/footer.scss';
.container{
  justify-content: center;
}
</style>