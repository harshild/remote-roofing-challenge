<template>
    <div class="container-header container-fluid">
        <div class="content">
            <div class="row justify-content-between">
                <div class="">
                    <a href="http://remoteroofing.com">
                        <img class="logo-img" src="https://uploads-ssl.webflow.com/5f127ac8860f158e650f06b5/5f12985a91b23596370f7a81_logo-72-dc-7-f-0-f%402x.png" height="50" >
                    </a>
                </div>

                <div class="contact">
                    <img src="https://uploads-ssl.webflow.com/5f127ac8860f158e650f06b5/5f1297d1c3fecf36271c10a2_483947%403x.png">
                    <a href="tel:2148658818">
                        214-865-8818
                    </a>
                </div>
            </div>
            <div class="row">
                <Menu/>
            </div>
            <div class="row">
                <Title/>
            </div>
        </div>
    </div>
</template>


<script>
    import Menu from "@/components/Menu";
    import Title from "@/components/Title";

    export default {
        name: 'Header',
        components: {
            Menu,
            Title
        }

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
        padding-top: 20px;
        padding-bottom: 20px;
        padding-left: 10px;
    }

    .logo-img {
        width: 82px;
        height: 30px;
        max-height: none;
        max-width: none;
    }
    .container-header .content .contact a {
        border-style: solid;
        border-width: 0px;
        border-color: hsla(0, 0%, 100%, 0);
        font-family: AirbnbCerealBold, sans-serif;
        color: #fff;
        font-weight: bold;
        font-size: 14px;
        line-height: 20px;
    }

    .container-header .content .contact a:hover {
        text-decoration:none;
    }

    .container-header .content .contact img {
        max-width: 15px;
        margin-right: 10px;
    }
</style>
