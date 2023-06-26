<template>
  <div>
    <headerComponent></headerComponent>
    <input type="text" placeholder="Bosila, Mohammadpur Dhaka">
    <div class="maps">
      <img src="../assets/img/basemap-image.png">
      <img class="blips" src="../assets/img/blips.png">
    </div>
  </div>
</template>

<script>
import headerComponent from'@/components/headerComponent.vue'

export default {
  name: 'MapsComponent',
  components: {
    headerComponent
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
div {
  position: relative;
  height: 100%;
  input {
    margin-top: 35px;
    border-radius: 13px;
    border: 1px solid #36424D;
    padding: 20px 70px 20px 40px;
    color: #36424D;
    font-size: 14px;
    width: 100%;
    outline: none;
    background-image: url("../assets/img/xnix-line-search-5.png");
    background-position: right 10% center;
    background-repeat: no-repeat;
  }
  .maps {
    margin-top: 20px;
    border-radius: 13px;
    width: 100%;
    height: 65%;
    overflow: hidden;
    user-select: none;
    img {
      position: relative;
    }
    .blips {
      position: absolute;
      bottom: 190px;
      left: 85px;
    }
  }
}
</style>
