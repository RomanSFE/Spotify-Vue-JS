<template>
    <div class="right-part">
        <div class="container">
            <div class="main-header-menu">
                <div id="nav">
                    <router-link to="/featured">FEATURED</router-link>
                    <router-link to="/podcasts">PODCASTS</router-link>
                    <router-link to="/chart">CHARTS</router-link>
                    <router-link to="/genres">GENRES & MOODS</router-link>
                    <router-link to="/release">NEW RELEASES</router-link>
                    <router-link to="/discover">DISCOVER</router-link>
                    <router-link to="/playlist">PLAYLIST</router-link>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Menu',
}
</script>
