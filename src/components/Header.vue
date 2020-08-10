<template>
  <div>
    <div class="container-header container-fluid">
      <div class="content">
        <div class="row header-row justify-content-between" >
          <div class="">
            <a href="http://remoteroofing.com">
              <img class="logo-img" src="https://uploads-ssl.webflow.com/5f127ac8860f158e650f06b5/5f12985a91b23596370f7a81_logo-72-dc-7-f-0-f%402x.png" height="50" >
            </a>
          </div>

          <div class="contact v-align">
            <img src="https://uploads-ssl.webflow.com/5f127ac8860f158e650f06b5/5f1297d1c3fecf36271c10a2_483947%403x.png">
            <a href="tel:2148658818">
              <strong>214-865-8818</strong>
            </a>
          </div>
        </div>
        <div class="row header-row pb-0">
          <Menu page="Home"/>
        </div>
        <div class="row header-row justify-content-start text-left">
          <h1>Roof inspections made remote and easy</h1>
          <span class="sub-head ">Get your roof inspected remotely and connect with our trusted roofers</span>
        </div>
        <div class="row header-row">
          <PlaceSearch/>
        </div>

      </div>
    </div>
    <div class="row header-row justify-content-center banner hidden-sm-down">
      <div class="banner-content row justify-content-between w-100">
        <div class="banner-content-item justify-content-center position-relative" v-for="(image, name) in benefits" v-bind:key="name">
          <div class="banner-content-item-img v-align d-flex"><img :src="image[0]" :width="image[1]" ></div>
          <div class="v-align text-left">{{name}}</div>
        </div>
      </div>
    </div>

  </div>
</template>


<script>
import Menu from "@/components/Menu";
import PlaceSearch from "@/components/PlaceSearch";

export default {
  name: 'Header',
  components: {
    Menu,
    PlaceSearch
  },
  data() {
    return {
      benefits: {
        "Free Inspection":["https://uploads-ssl.webflow.com/5f127ac8860f158e650f06b5/5f1290e8860f155c380f1c02_3039041%403x.png", "80"],
        "File a Claim":["https://uploads-ssl.webflow.com/5f127ac8860f158e650f06b5/5f1293b423e1bd4b2b89c278_2921571%403x.png", "81"],
        "Replace or Repair a Roof":["https://uploads-ssl.webflow.com/5f127ac8860f158e650f06b5/5f12939072c6226dbd635684_69886%403x.png","130"],
      }
    }
  }

}
</script>
<style scoped>
@font-face {
  font-family: 'AirbnbCerealLight';
  src: url('https://uploads-ssl.webflow.com/5f127ac8860f158e650f06b5/5f129663d13f49d2bead206e_AirbnbCerealLight.woff') format('woff');
  font-weight: 300;
  font-style: normal;
}
@font-face {
  font-family: 'AirbnbCerealBold';
  src: url('https://uploads-ssl.webflow.com/5f127ac8860f158e650f06b5/5f129663911bc70025b78db3_AirbnbCerealBold.woff') format('woff');
  font-weight: 700;
  font-style: normal;
}
h1 {
  font-family: AirbnbCerealBold, sans-serif;
  color: #fff;
  font-weight: 700;
  font-size: 38px;
  margin: 40px 0px 10px;
}

.sub-head {
  font-family: AirbnbCerealLight, sans-serif;
  color: #fff;
  font-size: 18px;
  line-height: 1.5em;
  font-weight: 700;
}

/*Need to check min height*/
.container-header {
  background-image: url("https://uploads-ssl.webflow.com/5f127ac8860f158e650f06b5/5f127dcece36df2cd5e4f713_Screen%20Shot%202020-07-17%20at%209.41.58%20PM.png");
  background-position: 0 0;
  background-size: cover;
  background-color: #f5f6f9;
}


.logo-img {
  width: 82px;
  height: 30px;
  max-height: none;
  max-width: none;
}
.container-header .content .contact a {
  font-family: AirbnbCerealBold, sans-serif;
  border-style: solid;
  border-width: 0;
  border-color: hsla(0, 0%, 100%, 0);
  color: #fff;
  font-weight: bold;
  font-size: 14px;
  line-height: 20px;
  margin-right: 40px;
}

.container-header .content .contact img {
  max-width: 15px;
  margin-right: 10px;
}

a:hover{
  text-decoration: none;
}
.header-row {
  margin: 0;
  padding-top: 20px;
}

@media screen and (min-width: 1023px) {
  .content {
    margin: auto;
    max-width: 940px;
    padding-left: 10px;
    padding-bottom: 140px;
  }

  .banner {
    margin: auto;
    max-width: 940px;
    align-items: center;
    padding: 0;
  }

  .banner-content {
    margin-top: -60px;
    height: 154px;
    background-color: #0059bf;
    box-shadow: 2px 2px 7px 0 rgba(10, 10, 10, 0.5);
    border-radius: 11px;
    padding-right: 40px;
    padding-left: 40px;
  }

  .banner-content-item {
    display: flex;
    width: 30%;
    padding-right: 20px;
    padding-left: 20px;
  }

  .banner-content-item img {
    max-width: 100%;
    margin-right: 0;
    padding-right: 20px;
    max-height: 60px;
  }

  .banner-content-item div {
    font-family: AirbnbCerealBook, sans-serif;
    color: #fff;
    font-size: 18px;
    font-weight: 400;
    padding-right: 10px;
  }
}

@media screen and (min-width: 768px) and (max-width: 1023px) {

  .content {
    margin: auto;
    max-width: 728px;
    padding-left: 10px;
    padding-bottom: 140px;
  }


  .banner {
    margin: auto;
    max-width: 728px;
    align-items: center;
    padding: 0;
  }

  .banner-content {
    margin-top: -60px;
    height: 154px;
    background-color: #0059bf;
    box-shadow: 2px 2px 7px 0 rgba(10, 10, 10, 0.5);
    border-radius: 11px;
    padding-right: 40px;
    padding-left: 40px;
  }

  .banner-content-item {
    display: flex;
    width: 30%;
    padding-right: 20px;
    padding-left: 20px;
  }

  .banner-content-item-img {
    width: 100px;
  }
  .banner-content-item-img img{
    max-width: 100%;
    margin-right: 0;
    padding-right: 20px;
    max-height: 60px;
  }

  .banner-content-item div {
    font-family: AirbnbCerealBook, sans-serif;
    color: #fff;
    font-size: 18px;
    font-weight: 400;
    padding-right: 10px;
  }
}

@media screen and (max-width: 768px) {

  .content {
    margin: auto;
    max-width: 728px;
    padding-left: 10px;
    padding-bottom: 140px;
  }
}

.v-align {
  margin-top: auto;
  margin-bottom: auto;
}

</style>
