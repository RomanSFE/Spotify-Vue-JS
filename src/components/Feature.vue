<template>
    <div class="col-md-3">
        <div class="chart-contenn-box">
            <a v-bind:href="feat_popu_lnk" target="_blank">
                <div class="single-chart-box">
                    <img :src="imagex" alt="" />
                    <div class="single-chart-hover">
                        <i class="fa fa-play"></i>
                    </div>
                </div> 
                
            </a>
                <h5> {{ heading }} </h5>
            
        </div>
    </div>              
</template>

<script>
export default {
    name: 'Feature',
    props: [
        'heading',
        'imagex',
        'feat_popu_lnk'
    ]
    // data() { 
    //     return {
    //         abc: require("../assets/chart1.jpg"),
    //         image: {
    //             id:"0",
    //             url:"../assets/chart1.jpg",
    //             title:"tt",
    //             des:"some text"
    //         }
    //     } 
    // },
    // computed: {
    //     getImage: function () {
    //         return require(this.image.url)
    //     }
    // }
}
</script>

<style lang="css">
.single-chart-box img{
    height: 165px;
    width: 165px;
}
.single-chart-box {
    height: 165px;
    width: 165px;
    margin-top: 2px;
}
.single-chart-box:hover{
    background-color: #333;
    opacity: 0.7;
    z-index: 1;
}
.single-chart-hover {
    margin-top: -165px;
    height: 165px;
    margin-bottom: 165px;
}
.single-chart-hover i {
    opacity: 0;
    height: 165px;
    width: 165px;
    margin-top: 38%;
    font-size: 45px;
}
.single-chart-hover i:hover {
    opacity: 1;
    z-index: 999;
    color: #fff;
}
.single-chart-box:hover i {
    opacity: 1;
    color: #fff;
}
.featured-ch-section {
    margin-top: 115px;
    padding: 10px 20px 20px 173px;
}
.featured-ch-section h3 {
    font-size: 35px;
    color: #fff;
    font-family: 'Montserrat', sans-serif;
    font-weight: 700;
}
.popular-ch-section {
    margin-top: 25px;
    padding: 10px 20px 20px 173px;
}
.popular-ch-section h3 {
    font-size: 35px;
    color: #fff;
    font-family: 'Montserrat', sans-serif;
    font-weight: 700;
}
.charts-section {
    margin-left: 20%;
}
.chart-contenn-box h5 {
    font-size: 14px;
    font-family: 'Montserrat', sans-serif;
    color: #fff;
    font-weight: 700;
    margin-top: 15px;
}
.chart-contenn-box {
    width: 165px;
}
</style>