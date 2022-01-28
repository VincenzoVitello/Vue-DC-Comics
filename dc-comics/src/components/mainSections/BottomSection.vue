<template>
  <div class="container_bottom_section">
    <div class="current_series">
          <p>current series</p>
        </div>
      <div class="thumbs-container">
        <div 
          v-for="(comic, index) in ElencoFumetti" :key="index" class="thumbnail">
            <img :src="comic.thumb" :alt="comic.series">
            <p>{{comic.series}}</p>
        </div>
        <button>Load More</button>
      </div>
  </div>
</template>

<script>
import ElencoFumettiPassato from '../../../dc-comics.json'
export default {
  
 name: "BottomSection",
 data(){
    return{
        ElencoFumetti: ElencoFumettiPassato
    }//chiusura return
  }//chiusura data
}//chiusura default
</script>

<style lang="scss" scoped >
@import '../../assets/style/bottomSection.scss';
</style>