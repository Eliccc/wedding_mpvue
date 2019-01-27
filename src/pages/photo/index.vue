<template>
    <div @click="playMusic()">
        <div v-if="isPlayingMusic">
            <div class="background_music">
                <image src="/images/music_icon.png" class="musicImg music_icon"/>
                <image src="/images/music_play.png" class="music_play pauseImg"/>
            </div>
        </div>
        <div v-else>
            <div class="background_music">
                <image src="/images/music_icon.png" class="musicImg"/>
                <image src="/images/music_play.png" class="music_play playImg"/>
            </div>
        </div>

    </div>

</template>
<script>
export default {
    data(){
        return{
            isPlayingMusic: true
        }
    },
    methods:{
        playMusic(){
            console.log(123)
            this.isPlayingMusic = !this.isPlayingMusic;
        }
    }
}
</script>

<style scoped lang=scss>
/* pages/invitation/index.wxss */
@import 'index.scss';
</style>