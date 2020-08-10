<template>
    <div class="row menu-row menu w-100">
        <div class="menu-item" v-for="(value, name) in items" :key="value" >
            <div>
                <a :href="value">{{ name }}</a>
            </div>
            <div v-if="page === name" class="menu-underline">
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Menu",
        props: {
          page: String
        },
        data() {
            return {
                items: {
                    Home: "https://www.remoteroofing.com/",
                    FAQ: "https://www.remoteroofing.com/faq",
                    Services: "https://www.remoteroofing.com/#services",
                }
            }
        },

    }
</script>

<style scoped>
    @font-face {
        font-family: 'AirbnbCerealLight';
        src: url('https://uploads-ssl.webflow.com/5f127ac8860f158e650f06b5/5f129663d13f49d2bead206e_AirbnbCerealLight.woff') format('woff');
        font-weight: 300;
        font-style: normal;
    }

    .menu {
        padding-top: 20px;
    }

    .menu-item {
        margin-right: 5%;
    }

    .menu-item a{
        font-family: AirbnbCerealLight, sans-serif;
        color: #ffffff;
        font-size: 18px;
        font-weight: 400;
    }

    .menu-underline {
        width: 50px;
        margin-top: 9px;
        border-style: solid;
        border-width: 1px;
        border-color: #fff;
        border-radius: 1px;
        background-color: #fff;
        color: #fff;
        line-height: 20px;
    }

    a:hover{
        text-decoration: none;
    }

    .menu-row {
        margin: 0;
        padding-top: 20px;
    }
</style>
