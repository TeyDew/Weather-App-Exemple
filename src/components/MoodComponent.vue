<template>
  <div>
    <headerComponent></headerComponent>
    <h1>How You feel Today ?</h1>
    <div class="mood-checker">
      <div class="mood-item" @click="changeActiveMood('1')" :class="{'active': moodActive === '1'}">
        <span>very good 😊</span>
      </div>
      <div class="mood-item" @click="changeActiveMood('2')" :class="{'active': moodActive === '2'}">
        <span>okish 😐</span>
      </div>
      <div class="mood-item" @click="changeActiveMood('3')" :class="{'active': moodActive === '3'}">
        <span>very bad 🙁</span>
      </div>
      <div class="mood-item" @click="changeActiveMood('4')" :class="{'active': moodActive === '4'}">
        <span>angry 😠</span>
      </div>
      <div class="mood-item" @click="changeActiveMood('5')" :class="{'active': moodActive === '5'}">
        <span>just sad for no reason 😩</span>
      </div>
      <div class="mood-item" @click="changeActiveMood('6')" :class="{'active': moodActive === '6'}">
        <span>i'm very very happy 😍</span>
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
  name: 'MoodComponent',
  components: {
    headerComponent
  },
  data () {
    return {
      moodActive: '1',
    }
  },
  methods: {
    changeActiveMood(mood) {
      this.moodActive = mood
    },
  }
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
  }
  .mood-checker {
    padding: 30px 10px 0px 10px;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    gap: 20px;
    position: relative;
    .mood-item {
      border-radius: 16px;
      border: 1px solid #36424D;
      color: #36424D;
      height: 80px;
      padding: 0px 20px;
      display: flex;
      justify-content: center;
      align-items: center;
      cursor: pointer;
      transition: all .2s ease-in;
      span {
        font-size: 15px;
        user-select: none;
      }
      &.active {
        color: white;
        background-color: #36424D;
        transition: all .2s ease-in;
      }
    }
    &::after {
      content: '';
      bottom: 0px;
      position: absolute;
      width: 100%;
      height: 50px;
      background: linear-gradient(0deg, rgba(255,255,255,.9) 0%, rgba(255,255,255,0) 100%);
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
