<script>
export default {
    props: {
        tvChannel: {
            type: String,
            required: true
        }
    },
    computed: {
        iframeSrc() {
            return `https://a3.115tv.site/cvatt.html?get=${this.tvChannel}&start=true`;
        }
    }
};
</script>

<template>
    <div class="home custom-container">
        <iframe
            width="100%"
            height="500px"
            :src="iframeSrc"
            frameborder="0"
        ></iframe>
    </div>
</template>
