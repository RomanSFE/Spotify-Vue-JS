<template>
    <div class="playlistt">
        <div class="side-menuu">
            <Sidemenu/>
        </div>

        <div class="music-box-xx">
               <Playbox v-for="item in lists" :key="item.id" :single_image="item.img" :music_name="item.m_name" :music_listenar="item.m_listener" :album_name="item.a_name"/>
        </div>
        <div class="single-music-itmm">
            <Playitem v-for="item in lists2" :key="item.id" :item_rel="item.item_r" :item_rel_link="item.item_r_lnk" :item_rel_name="item.item_r_name" :item_rel_time="item.item_r_time" :item_down_link="item.item_d_lnk" :item_down="item.item_dwn"/>
        </div>

        <!-- <Playbox v-for="item in lists" :key="item.id" :single_image="item.img" :music_name="item.m_name" :music_listenar="item.m_listener" :album_name="item.a_name"/>

        <Playitem v-for="item in lists2" :key="item.id" :item_rel="item.item_r" :item_rel_link="item.item_r_lnk" :item_rel_name="item.item_r_name" :item_rel_time="item.item_r_time" :item_down_link="item.item_d_lnk" :item_down="item.item_dwn"/> -->
 
    <div class="music-player-playlist">
        <Musicplayer/>
    </div>

    </div>
</template>

<script>
import Sidemenu from '@/components/Sidemenu.vue'
import Playbox from '@/components/Playbox.vue'
import Playitem from '@/components/Playitem.vue'
import Musicplayer from '@/components/Musicplayer.vue'

export default {
    name: 'playlistt',
    components: {
        Sidemenu,
        Playbox,
        Playitem,
        Musicplayer
    },
    data: () => ({
        lists: [
            {id: 0, m_name: "Daily Mix 5", img: require("../assets/chart1.jpg"), m_listener: "Model for Lotus Kazi by Spotify.", a_name: "Endlexx Mix"},
        ],
        lists2: [
            {id: 0, item_r: "New", item_r_lnk: "https://google.com", item_r_name: "daya", item_r_time: "New", item_d_lnk: "https://google.com", item_dwn: "Download"},
            {id: 1, item_r: "New", item_r_lnk: "https://google.com", item_r_name: "daya", item_r_time: "New", item_d_lnk: "https://google.com", item_dwn: "Download"},
            {id: 2, item_r: "New", item_r_lnk: "https://google.com", item_r_name: "daya", item_r_time: "New", item_d_lnk: "https://google.com", item_dwn: "Download"},
            {id: 3, item_r: "New", item_r_lnk: "https://google.com", item_r_name: "daya", item_r_time: "New", item_d_lnk: "https://google.com", item_dwn: "Download"},
            {id: 4, item_r: "New", item_r_lnk: "https://google.com", item_r_name: "daya", item_r_time: "New", item_d_lnk: "https://google.com", item_dwn: "Download"},
            {id: 5, item_r: "New", item_r_lnk: "https://google.com", item_r_name: "daya", item_r_time: "New", item_d_lnk: "https://google.com", item_dwn: "Download"},
            {id: 6, item_r: "New", item_r_lnk: "https://google.com", item_r_name: "daya", item_r_time: "New", item_d_lnk: "https://google.com", item_dwn: "Download"},
            {id: 7, item_r: "New", item_r_lnk: "https://google.com", item_r_name: "daya", item_r_time: "New", item_d_lnk: "https://google.com", item_dwn: "Download"},
            {id: 8, item_r: "New", item_r_lnk: "https://google.com", item_r_name: "daya", item_r_time: "New", item_d_lnk: "https://google.com", item_dwn: "Download"},
        ]
  }),

}
</script>

<style>
/* side menu */
.side-menuu {
    margin-top: -92px;
    position: relative;
}

/* music box */
.music-box-xx {
    position: absolute;
    left: 269px;
    top: 90px;
}
/* .music-box-xx{
    position: relative;
} */
/* Music item */
.single-music-itmm {
    position: absolute;
    left: 527px;
    width: 821px;
    top: 103px;
}
.list-main-tt {
    float: left;
    margin-top: 5px;
    margin-left: 5px;
}

/* Music player */
.music-player-playlist{
  margin-top: 582px;
  position: fixed;
}
</style>

