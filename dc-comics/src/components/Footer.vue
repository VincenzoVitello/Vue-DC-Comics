<template>
  <div>
    <div class="blueFooterContainer">
    <div class="container">
      <ul>
        <li v-for="(element, index) in links" :key="index"><a href="#"><img :src="element.imag" alt=""></a>{{element.text}}</li>
      </ul>
    </div>
   
    
  </div>
   <div class="footerBackGround">
     <div class="container">
       <div class="leftSection">
         <div class="footerOne">
              <h2>DC Comics</h2>
                  <ul>
                    <li>Characters</li>
                    <li>Comics</li>
                    <li>Movies</li>
                    <li>TV</li>
                    <li>Games</li>
                    <li>Videos</li>
                    <li>News</li>
                  </ul>
            <h2>Shop</h2>
                <ul>
                  <li>Show DC</li>
                  <li>Shop DC Collectibles</li>
                </ul>
         </div>
         <div class="footerTwo">
           <h2>DC</h2>
         <ul>
           <li>Terms of use</li>
           <li>Privacy Policy</li>
           <li>Ad Choises</li>
           <li>Advertising</li>
           <li>Jobs</li>
           <li>Subscriptions</li>
           <li>Talent Workshops</li>
           <li>CPSC Certificates</li>
           <li>Ratings</li>
           <li>Shop Help</li>
           <li>Contact Us</li>
         </ul>
         </div>
         <div class="footerTre">
           <h2>Sites</h2>
         <ul>
           <li>DC</li>
           <li>Mad Magazine</li>
           <li>DC Kids</li>
           <li>DC Universe</li>
           <li>DC Power Visa</li>
         </ul>
         </div>
       </div>
       <div class="rightSection">
         <img src="../assets/img/dc-logo-bg.png" alt="">
       </div>
     </div>
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
  justify-content: space-between;
}
.footerBackGround{
  background-image: url("../assets/img/footer-bg.jpg");
  height: 600px;
  transform: translate(-150px -100px);
  background-repeat: repeat-x;
  object-fit: cover;
}
</style>