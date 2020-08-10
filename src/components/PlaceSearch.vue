<template>
  <div class="search-container w-100">
    <form name="place-search" method="get" action="https://www.remoteroofing.com/signup-form">
      <div class="search-box d-flex flex-row align-content-center justify-content-between ">
        <div class="search-input">
          <div>
            <img class="search-img" src="https://uploads-ssl.webflow.com/5f127ac8860f158e650f06b5/5f13618db066ca1a332318d1_home%403x.png" width="30" alt="">
          </div>
          <div class="search-input-container">
            <input type="text" class="place-input" maxlength="256" name="place" placeholder="Enter Your Address" required autocomplete="off">
          </div>
        </div>
        <input type="submit" value="Get Inspection" class="submit-button">
      </div>
    </form>
  </div>
</template>

<script>
export default {
  name: "PlaceSearch"
}
</script>

<style scoped>
@font-face {
  font-family: 'AirbnbCerealLight';
  src: url('https://uploads-ssl.webflow.com/5f127ac8860f158e650f06b5/5f129663d13f49d2bead206e_AirbnbCerealLight.woff') format('woff');
  font-weight: 300;
  font-style: normal;
}
.search-container {
  margin-top: 20px;
}


.search-box {
  position: relative;
  z-index: 0;
  height: 60px;
  max-height: none;
  max-width: 500px;
  margin-bottom: 10px;
  align-items: center;
  border-radius: 50px;
  background-color: #fff;
  box-shadow: 1px 1px 3px 0 #000;
}

.search-img {
  max-width: 60%;
  margin-left: 10px;
  margin-right: 10px;
  padding-left: 5px;
}
.search-input {
  display: -webkit-box;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
  width: 100%;
  -webkit-box-pack: start;
  -webkit-justify-content: flex-start;
  -ms-flex-pack: start;
  justify-content: flex-start;
  -webkit-box-align: center;
  -webkit-align-items: center;
  -ms-flex-align: center;
  align-items: center;
}

.search-input-container {
  width: 100%;
  padding-top: 10px;
}

.place-input {
  width: 100%;
  font-family: AirbnbCerealLight, sans-serif;
  display: block;
  height: 38px;
  padding: 8px 12px;
  margin-bottom: 10px;
  font-size: 14px;
  line-height: 1.42857143;
  color: #333333;
  vertical-align: middle;
  background-color: #ffffff;
  border: 0px solid #cccccc;

}

.place-input:focus {
  border: 1px solid #3898EC;
  outline: 0;
}
.submit-button {
  font-family: AirbnbCerealBook, sans-serif;
  font-size: 16px;
  color: white;
  background-color: #017afe;
  padding: 9px 15px;
  line-height: inherit;
  height: 45px;
  min-width: 190px;
  margin-right: 10px;
  border-radius: 22px;
  display: inline-block;
  border: 0;
  text-decoration: none;
  cursor: pointer;
}
</style>
