<template>
    <div class="row">
        <div class="col-md-4">
            <div class="playlist-contenn-box">
                <a href="#">
                <div class="single-playlist-box">
                    <img :src="single_image" alt="spotify dl"/>
                    <div class="single-playlist-hover">
                        <i class="fa fa-play"></i>
                    </div>
                </div>
                </a>
                <div class="single-playlist-text">
                    <h4>{{ music_name }}</h4>
                    <p>{{ music_listenar }} <br> {{ album_name }}</p>
                    <a href="" class="play-btnn">PLAY</a>
                </div>
            </div>		
        </div>
    </div>
</template>

<script>
export default {
    name: 'Playbox',
    props: [
        'single_image',
        'music_name',
        'music_listenar',
        'album_name' 
        ]
}
</script>

<style lang="css">
    .playlist-contenn-box h5 {
    font-size: 14px;
    font-family: 'Montserrat', sans-serif;
    color: #fff;
    font-weight: 700;
    margin-top: 15px;
}
.playlist-contenn-box {
    width: 245px;
}
.single-playlist-box {
    height: 244px;
    width: 244px;
    margin-top: 20px;
}
.single-playlist-box:hover{
    background-color: #333;
    opacity: 0.7;
    z-index: 1;
}
.single-playlist-box img {
    height: 244px;
    width: 244px;
}
.single-playlist-hover i {
    opacity: 0;
    height: 180px;
    width: 244px;
    margin-top: 45%;
    font-size: 55px;
}
.single-playlist-hover i:hover {
    opacity: 1;
    z-index: 10;
    color: #fff;
}
.single-playlist-hover {
    margin-top: -250px;
}
.single-playlist-box:hover i {
    opacity: 1;
    color: #fff;
}
a.play-btnn {
    background-color: #1ED760;
    color: #fff;
    padding: 10px 45px 10px 45px;
    border-radius: 50px;
    margin-top: 25px;
    display: block;
    width: 140px;
    text-align: center;
    margin-left: 52px;
}
.single-playlist-text {
    text-align: center;
    margin-top: 17px;
}
.single-playlist-text p {
    font-size: 14px;
    color: #afadad;
    font-weight: 600;
}
.single-playlist-text h4 {
    font-size: 27px;
    color: #fff;
    font-family: 'Montserrat', sans-serif;
    font-weight: 700;
}
</style>
