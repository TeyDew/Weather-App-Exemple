<template>
  <div>
    <headerComponent></headerComponent>
    <h1>Feels Like A good<br>time to ride a bike
      <img src="../assets/img/icons-8-cycling-mountain-bike-1.png">
    </h1>
    <div class="temp-container">
      <div class="temp-circle">
        <p>Today's Like</p>
        <span>25°</span>
        <img src="../assets/img/clouds/cloudy-day-icon-by-devoart.png" id="cloud1">
        <img src="../assets/img/clouds/rain-icon-by-devoart.png" id="cloud2">
        <img src="../assets/img/clouds/untitled-101.png" id="cloud3">
        <img src="../assets/img/clouds/windy-icon-by-devoart.png" id="cloud4">
        <img src="../assets/img/clouds/clear-night-icon-by-devoart.png" id="cloud5">
        <img src="../assets/img/clouds/thundersrtom-icon-by-devoart.png" id="cloud6">
      </div>
    </div>
    <table class="weather-mood">
      <tr>
        <td>Today's Mood</td>
        <td>Tomorrow's Mood</td>
      </tr>
      <tr>
        <td>Very Good</td>
        <td>Excellent</td>
      </tr>
    </table>
  </div>
</template>

<script>
import headerComponent from'@/components/headerComponent.vue'

export default {
  name: 'HomeComponent',
  components: {
    headerComponent
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
div {
  h1 {
    margin-top: 30px;
    font-size: 24px;
    line-height: 110.5%;
    font-family: 'Poppins-Medium';
    img {
      margin-left: 10px;
    }
  }
  .temp-container {
    height: 380px;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    .temp-circle {
      border-radius: 50%;
      background-color: #0C1823;
      height: 265px;
      width: 265px;
      display: flex;
      justify-content: center;
      align-items: center;
      color: white;
      flex-direction: column;
      position: relative;
      p {
        margin-left: -40px;
        margin-top: -40px;
      }
      span {
        margin-left: -40px;
        font-size: 44px;
        line-height: 100%;
      }
      img {
        position: absolute;
        &#cloud1 {
          top: 20px;
          left: 0;
        }
        &#cloud2 {
          top: 20px;
          right: 0;
        }
        &#cloud3 {
          top: 115px;
          left: 115px;
        }
        &#cloud4 {
          top: 150px;
          left: -10px;
        }
        &#cloud5 {
          top: 140px;
          right: -25px;
        }
        &#cloud6 {
          bottom: -25px;
          left: 50%;
          transform: translateX(-50%);
        }
      }
    }
  }
  .weather-mood {
    margin-top: 30px;
    tr {
      &:first-child {
        td {
          color: #36424D;
          font-size: 14.02px;
          &:first-child {
            padding-right: 50px;
          }
        }
      }
      &:last-child {
        td {
          color: #0C1823;
          font-size: 12px;
          font-family: 'Poppins-Bold';
        }
      }
    }
  }
}
</style>
