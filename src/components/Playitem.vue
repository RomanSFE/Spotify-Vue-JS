<template>
    <div class="col-md-8">
        <div class="list-sections">
            <div class="ui middle aligned selection list">
                <div class="item">
                    <div class="content">
                        <div class="list-textt">
                            <div class="list-main-tt">
                                <h6><span><i class="fa fa-music"></i></span>{{ item_rel }}</h6>
                            <p><a v-bind:href="item_rel_link">{{ item_rel_name }}</a> . <a href="#">{{ item_rel_time }}</a></p>
                            </div>
                            <div class="download-itm">
                                <a v-bind:href=" item_down_link " class="download-btnn">{{ item_down }}</a>
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
    name: 'Playitem',
    props: [
        'item_rel',
        'item_rel_link',
        'item_rel_name',
        'item_rel_time',
        'item_down_link',
        'item_down'
    ]

}
</script>

<style lang="css">
.list-sections {
    margin-top: 15px;
}
.list-textt h6 {
    font-size: 15px;
    color: #ece8e8;
    margin-bottom: 3px;
}
.list-textt h6 span {
    margin-right: 15px;
}
.ui.selection.list .list>.item, .ui.selection.list>.item {
    border-radius: 0px;
    height: 62px;
}
.ui.selection.list.list>.item:hover, .ui.selection.list>.item:hover {
    background: rgba(0, 20, 20, 0.10);
    color: rgba(0,0,0,.7);
}
.list-textt {
    margin-top: -8px;
    position: relative;
}
.list-textt p a {
    color: #afadad;
    font-size: 12px;
    font-weight: 600;
    font-family: 'Montserrat', sans-serif;
}
.list-textt p a:hover {
    color: #afadad;
    font-size: 12px;
    font-weight: 600;
    font-family: 'Montserrat', sans-serif;
    text-decoration: underline
}
.download-itm a {
    position: absolute;
    right: 28px;
    top: 6px;
}
a.download-btnn{
	background-color: #1ED760;
    color: #fff;
    padding: 10px 45px 10px 41px;
    border-radius: 50px;
    margin-top: 3px;
    display: block;
    width: 140px;
    text-align: center;
}
.download-itm{
	opacity: 0;
}
.ui.selection.list.list>.item:hover, .ui.selection.list>.item:hover .download-itm {
    opacity: 1;
}
</style>
