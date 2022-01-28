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
     <div class="bottom_footer_container">
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
    <div class="contacts_container">
      <button>SIGN UP NOW!</button>
      <div class="socials">
        <p>FOLLOW US!</p>
        <img src="../assets/img/footer-facebook.png" alt="">
        <img src="../assets/img/footer-twitter.png" alt="">
        <img src="../assets/img/footer-youtube.png" alt="">
        <img src="../assets/img/footer-pinterest.png" alt="">
        <img src="../assets/img/footer-periscope.png" alt="">
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
@import '../assets/style/variables.scss';
.bottom_footer_container{
  display: flex;
  justify-content: space-evenly;
}
.leftSection{
  margin-top: 30px;
}
.footerBackGround{
  background-image: url("../assets/img/footer-bg.jpg");
  height: 350px;
  background-repeat: repeat-x;
  overflow: hidden;
  object-fit: cover;

  img{
    transform: translateY(-100px);
  }
}
.contacts_container{
  background-color: #303030;
  height: 100px;
  width: 100%;
  display: flex;
  justify-content: space-evenly;
  align-items: center;

  button{
    height: 30px;
    background-color: #303030;
    border: 2px solid $mainColor;
    color: white;
    padding: 5px 20px;
    &:hover{
      cursor: pointer;
    }
  }
}
.socials{
  display: flex;
  justify-content: space-around;
  align-items: center;

  img{
    margin: 0px 10px;
    &:hover{
      cursor: pointer;
    }
  }
  p{
    color: $mainColor;
    
  }
}

</style>