<!-- inserimento HTML -->
<template>
  <div class="container header_container">
      <div class="header_left">
         <a href=""><img src="../assets/img/dc-logo.png" alt=""></a>
      </div>
      <div class="header_right_list">
          <nav>
            <ul>
              <li v-for="(element, index) in links" :key="index" ><a href="">{{element.text}}</a></li>
            </ul>
          </nav>
      </div>
  </div>
</template>
<!-- inserimento script -->
<script>
export default {
    name: 'Header',

    data(){
     return {
         links: [
             {
                 text: "Characters",
                 url: "#",
                 current: false,
             },
             {
                 text: "Comics",
                 url: "#",
                 current: false,
             },
             {
                 text: "Movies",
                 url: "#",
                 current: false,
             },
             {
                 text: "TV",
                 url: "#",
                 current: false,
             },
             {
                 text: "Games",
                 url: "#",
                 current: false,
             },
             {
                 text: "Collectibles",
                 url: "#",
                 current: false,
             },
             {
                 text: "Videos",
                 url: "#",
                 current: false,
             },
             {
                 text: "Fans",
                 url: "#",
                 current: false,
             },
             {
                 text: "News",
                 url: "#",
                 current: false,
             },
             {
                 text: "Shop",
                 url: "#",
                 current: false,
             },
             
         ]
     } //chiusura return
  } //chiusura data()
} //chiusura default 
</script>

<!-- inserimento stile CSS -->
<style lang="scss" scoped>
 @import '../assets/style/Header_style.scss';
</style>