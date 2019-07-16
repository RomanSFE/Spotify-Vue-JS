<template>
  <div class="home">
    <div class="side-menu">
      <Sidemenu/>
    </div>

    <div class="feature-section">
      <div class="container">
        <div class="row">
          <div class="featured-ch-section">
            <h3>Featured Charts</h3>
          </div> 

          <div class="feature-popularr">
              <div class="row">
                <Feature v-for="item in lists" :key="item.id" :feat_popu_lnk="item.fe_popu_link" :heading="item.genre" :imagex="item.img" />
            </div>
          </div>

          <div class="popular-ch-section">
              <h3>Popular Charts</h3>
          </div>
          <div class="feature-popularr">
              <div class="row">
                <Feature v-for="item in lists2" :key="item.id" :feat_popu_lnk="item.fe_popu_link" :heading="item.genre" :imagex="item.img" />
            </div>
          </div>

        </div>
      </div>
    </div>

    <div class="music-player">
        <Musicplayer/>
    </div>


  <!-- <Feature v-for="item in lists" :key="item.id" :heading="item.genre" :imagex="item.img" /> -->
    <!-- <Feature :image="images[0].url"/> -->
  </div>
</template>

<script>
// @ is an alias to /src

import Sidemenu from '@/components/Sidemenu.vue'

import Feature from '@/components/Feature.vue'

import Musicplayer from '@/components/Musicplayer.vue'


export default {
  name: 'home',
  components: {
    Sidemenu,
    Feature,
    Musicplayer
  },
  data: () => ({
    lists: [
      {id: 0, genre: "Pop", fe_popu_link: "https://google.com", img: require("../assets/chart1.jpg")},
      {id: 1, genre: "Rock", fe_popu_link: "https://facebook.com", img: require("../assets/chart1.jpg")},
      {id: 2, genre: "Indie", fe_popu_link: "https://twitter.com", img: require("../assets/chart1.jpg")},
      {id: 3, genre: "Feature Songs", fe_popu_link: "https://linkedln.com", img: require("../assets/chart1.jpg")}
    ],
    lists2: [
      {id: 0, genre: "popular song", fe_popu_link: "https://spotify.com", img: require("../assets/chart1.jpg")},
      {id: 1, genre: "Popular", fe_popu_link: "https://google.com", img: require("../assets/chart1.jpg")},
      {id: 2, genre: "Indie", fe_popu_link: "https://vuejs.com", img: require("../assets/chart1.jpg")},
      {id: 3, genre: "Popular 2019", fe_popu_link: "https://reactjs.org/", img: require("../assets/chart1.jpg")}
    ]
  })
}
</script>

<style>
/* side menu */
.side-menu {
    margin-top: -92px;
}

/* Feature popular */
.feature-popularr{
  margin-left: 176px;
}

/* Music player */
.music-player{
  margin-top: -130px;

  /* margin-top: -320px; */
}
</style>

