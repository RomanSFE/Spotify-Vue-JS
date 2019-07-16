<template>
  <div class="player-main-section">
	<div class="ui container-fluid">
		<div class="ui grid">
			<div class="row">
			    <div class="col-md-3">
					<div class="music-image-text">
						<a href="#"><img src="../assets/chart1.jpg" alt=""></a>
						<div class="music-title align-right">
							<h4>Lorem ipsum dolor sit amet,</h4>
							<p>Lorem ipsum dolor</p>
						</div>
						<div class="music-iconn">
							<span><i class="fa fa-heart" title="Save to your Favourite Songs"></i> <i class="fa fa-file" title="Hello something"></i></span>
						</div>
					</div>
				</div>

				<div class="col-md-6">
					<div class="play-button-sec">
						<div class="player-music-icon">
                          <div class="item">
                          	<i class="fa fa-random" title="Enable shuffle"></i>
                          </div>
                          <div class="item">
                          	<i class="fa fa-step-backward" title="Previous"></i>
                          </div>
                          <div class="item ex-play">
                          	<i class="fa fa-play" title="Pause"></i>
                          </div>
                          <div class="item">
                          	<i class="fa fa-step-forward" title="Next"></i>
                          </div>
                          <div class="item">
                          	<i class="fa fa-retweet" title="Enable repeat one"></i>
                          </div>
                        </div>
					</div>
					<div class="play-button-progress">
						<div class="ui tiny progress">
						  <div class="bar"></div>
						</div>
					</div>
				</div>

				<div class="col-md-3">
					<div class="volume-button-sec">
						<div class="player-music-icon">
	                          <div class="item">
	                          	<i class="fa fa-list-alt" title="Queue"></i>
	                          </div>
	                          <div class="item">
	                          	<i class="fa fa-music" title="Hello I am a popup"></i>
	                          </div>
	                          <div class="item">
	                          	<i class="fa fa-volume-up" title="Sound system"></i>
	                          </div>
	                          <div class="item">
	                          	<div class="volume-boxx">
	                          		<div class="ui tiny progress">
									  <div class="bar"></div>
									</div>
	                          	</div>
	                          </div>
                          </div>
                        </div>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
    name: 'Musicplayer',
    props: [
        
    ]
}
</script>

<style lang="css">
.player-main-section {
    height: 170px;
    width: 100%;
    position: fixed;
    background-color: #000;
}
.music-image-text a img {
    width: 75px;
    height: 80px;
    padding: 15px 10px 10px 10px;
    position: relative;
    margin-left: -245px;
}
.music-title.align-right {
    position: absolute;
    left: 89px;
    top: 24px;
}
.music-title.align-right p {
    margin-top: -8px;
    text-align: left;
}
.music-title.align-right h4{
	position: relative;
}
.music-title.align-right h4 {
    color: #fff;
    font-size: 15px;
    font-weight: 500;
    font-family: 'Cuprum', sans-serif;
}
.music-title.align-right p {
    color: #9c9797;
    font-size: 13px;
}
.player-music-icon i.fa {
    color: #948c8c;
    padding: 5px 0px 0px 0px;
}
.player-music-icon i.fa:hover{
    color: #fff;
}
.music-iconn i.fa {
    margin-left: 7px;
    color: #948c8c;
}
.music-iconn {
    position: absolute;
    left: 292px;
    top: 27px;
    display: inline-block;
}
.ui.horizontal.list {
    display: inline-block;
    font-size: 0;
    margin-left: 37%;
    color: #989393;
    margin-top: 18px;
    margin-bottom: 10px;
}
.ui.horizontal.list .item:hover {
    color: #fff;
    transition: .1s;
}
.item.ex-play:hover i {
    color: #fff;
}
.item.ex-play {
    color: #a2a0a0;
    height: 35px;
    width: 35px;
    border: 1px solid #8c8989;
    border-radius: 50%;
}
.item.ex-play:hover{
	border-color: #fff;
	transform: scale(1.07);
	transition: .3s;
}
.ui.horizontal.list .item {
    padding: 8px 0px 0px 12px;
}
.music-iconn i:hover {
    color: #fff;
    transition: .1s;
}
.volume-boxx .ui.tiny.progress {
    margin: 0 auto;
    margin-left: -15px;
    width: 45px;
    background-color: #948c8c;
    height: 6px;
}
.play-button-progress .ui.tiny.progress {
    margin: 0 auto;
    margin-left: 72px;
    width: 71px;
    height: 6px;
    background-color: #948c8c;
}
.player-music-icon .item {
    display: inline-block;
    padding: 4px 17px 13px 12px;
}
.play-button-sec {
    margin-top: 15px;
}
.volume-button-sec {
    margin-top: 15px;
}
</style>
