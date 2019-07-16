<template>
    <div class="left-part">
        <div class="left-menu-img">
            <router-link to="/"><img src="../assets/spotify.png"/></router-link>
        </div>
        <div class="left-main-menu">
        <ul>
            <li><a href="#"><span><i class="fa fa-home"></i></span> Home</a></li>
            <li><a href="#"><span><i class="fa fa-search"></i></span> Search</a></li>
            <li><a href="#"><span><i class="fa fa-list-ul"></i></span> Your Library</a></li>
        </ul>
        </div>
        <div class="after-left-menu">
        <h6>Recently Played</h6>
        <ul>
            <li><a href="#"><span>Daily Mix 3</span> Daily Mix</a></li>
            <li><a href="#"><span>2009 Hits</span> Playlist</a></li>
            <li><a href="#"><span>Beast Mode</span> Playlist</a></li>
        </ul>
        </div>
      </div>
</template>

<script>
export default {
  name: 'Sidemenu'
}
</script>

<style lang="css">
.left-part {
    width: 17%;
    height: 89%;
    position: fixed;
    background-color: #000;
}
.left-partt {
    width: 17%;
    height: 89%;
    position: fixed;
    background-color: #000;
}
.left-menu-img img {
    width: 126px;
    height: 40px;
    margin: 30px 10px 10px -25px;
}
.left-menu-imgg img {
    width: 126px;
    height: 40px;
    margin: 44px 10px 10px 23px;
}
.left-main-menu {
    margin-top: 15px;
    text-align: left;
}
.left-main-menu ul {
    list-style: none;
}
.left-main-menu ul li {
    display: block;
    padding: 10px 5px 5px 5px;
}
.left-main-menu ul li a {
    font-size: 15px;
    color: #b3b1b1;
    font-weight: 500;
}
.after-left-menu ul {
    list-style: none;
}
.after-left-menu li {
    display: block;
    padding: 3px 5px 5px 3px;
}
.after-left-menu li a {
    color: #b7b5b5;
    font-weight: 500;
    font-size: 14px;
    line-height: 14px;
}
.after-left-menu ul li a span {
    display: block;
}
.after-left-menu h6 {
    color: #bbbaba;
    font-size: 14px;
    text-transform: uppercase;
    font-weight: 500;
    margin-left: 43px;
}
.after-left-menu {
    text-align: left;
}
.install-app {
    border-bottom: 1px solid #aba7a7;
    margin-bottom: 10px;
    margin-left: 40px;
    margin-right: 28px;
}
.after-left-menu h6 {
    margin-top: 30px;
    margin-bottom: 30px;
}
.install-app a {
    color: #afadad;
    font-size: 14px;
    font-weight: 700;
    margin-bottom: 5px;
    display: block;
}
.user-profile-left img {
    margin-right: 10px;
    width: 35px;
    height: 35px;
    border-radius: 50%;
}
.user-profile-left a {
    color: #fff;
    font-weight: 700;
    font-size: 14px;
}
.user-profile-left {
    margin-left: 38px;
}
.install-profile {
    margin-top: 68px;
}
</style>