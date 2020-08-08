<template>
    <div class="container-header">
        <div class="content">
            <div class="logo">
                <a href="http://remoteroofing.com">
                    <img src="https://uploads-ssl.webflow.com/5f127ac8860f158e650f06b5/5f12985a91b23596370f7a81_logo-72-dc-7-f-0-f%402x.png" height="50" >
                </a>
            </div>

            <div class="contact">
                <img src="https://uploads-ssl.webflow.com/5f127ac8860f158e650f06b5/5f1297d1c3fecf36271c10a2_483947%403x.png">
                <a href="tel:2148658818">
                    214-865-8818
                </a>
            </div>
        </div>

    </div>
</template>

<script>
    export default {
        name: 'Header'
    }
</script>
<style scoped>
    /*Need to check min height*/
    .container-header {
        background-image: url("https://uploads-ssl.webflow.com/5f127ac8860f158e650f06b5/5f127dcece36df2cd5e4f713_Screen%20Shot%202020-07-17%20at%209.41.58%20PM.png");
        min-height: 500px;
        padding-top: 20px;
    }

    .container-header .content {
        margin: auto;
        max-width: 964px;
    }

    .container-header .content .logo {
        display: inline-block;
        float: left;
    }
    .container-header .content .contact {
        float: right;
        display: flex;
    }
</style>
