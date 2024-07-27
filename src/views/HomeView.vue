<script>
import videoPlayer from "@/components/videoPlayer.vue";
export default {
    data() {
        return {
            channel: "",
        };
    },
    components: {
        videoPlayer,
    },
    methods: {
        setChannel(channel) {
            this.channel = channel;
        },
    },
};
</script>

<template>
    <div class="tv custom-container">
        <videoPlayer v-if="channel !== ''" :tvChannel="channel" />
    </div>
    <div class="channels custom-container">
        <button @click="setChannel('VGVsZWZlSEQ=')">
            <img src="@/assets/channels/telefe.png" alt="" />
            Telefe
        </button>
        <button @click="setChannel('QW1lcmljYTI0')">
            <img src="@/assets/channels/america.webp" alt="" />
            America
        </button>

        <button @click="setChannel('QzVO')">
            <img src="@/assets/channels/c5n.webp" alt="" />
            C5N
        </button>
        <button @click="setChannel('QXJ0ZWFySEQ')">
            <img src="@/assets/channels/eltrece.webp" alt="" />
            El Trece
        </button>
        <button @click="setChannel('Q2FuYWw5')">
            <img src="@/assets/channels/nueve.webp" alt="" />
            Nueve
        </button>
        <button @click="setChannel('VG9kb05vdGljaWFz')">
            <img src="@/assets/channels/tn.png" alt="" />
            TN
        </button>
        <button @click="setChannel('Q2FuYWw3')">
            <img src="@/assets/channels/tvpublica.webp" alt="" />
            TV Publica
        </button>
        <button @click="setChannel('VHlDU3BvcnQ')">
            <img src="@/assets/channels/tyc.webp" alt="" />
            TyC Sports
        </button>
        <button @click="setChannel('Rm94U3BvcnRz')">
            <img src="@/assets/channels/foxsports.png" alt="" />
            Fox Sports
        </button>
        <!--         <button @click="setChannel('ZGAACWale2MAAAAJM/TcAw==')">
            <img src="@/assets/channels/tvpublica.webp" alt="" />
            DirectTv
        </button> -->
    </div>
</template>

<style scoped lang="scss">
.channels {
    display: flex;
    gap: 25px;
    flex-wrap: wrap;

    button {
        padding: 25px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-between;
        img {
            height: auto;
            width: 125px;
        }
    }
}
</style>
