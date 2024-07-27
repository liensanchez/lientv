<template>
    <nav class="custom-container">
        <router-link to="/" class="logo">
            <svg
                fill="#000000"
                height="64px"
                width="64px"
                version="1.1"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                viewBox="0 0 50 50"
                xml:space="preserve"
            >
                <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
                <g
                    id="SVGRepo_tracerCarrier"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                ></g>
                <g id="SVGRepo_iconCarrier">
                    <g id="Layer_1">
                        <path
                            d="M1,38h23v3H12v2h26v-2H26v-3h23V8H1V38z M3,10h44v26H3V10z"
                        ></path>
                    </g>
                    <g></g>
                </g>
            </svg>
            <h1>LienTv</h1>
        </router-link>
    </nav>
    <router-view />
</template>

<style lang="scss">
@import "@/assets/global.scss";
nav {
    display: flex;

    .logo {
        display: flex;
        align-items: center;
        gap: 5px;
    }
}
</style>
