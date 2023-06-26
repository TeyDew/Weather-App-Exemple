<template>
  <div class="home">
    <div class="dynamic-island"></div>
    <div class="loading" :class="{'hide': !loadingScreen, 'anim': loadingClosing}">
      <svg width="105" height="73" viewBox="0 0 105 73" fill="none" xmlns="http://www.w3.org/2000/svg">
        <g id="Group 11">
          <g id="Random Symboles 10">
            <g id="Group">
              <path id="Vector" d="M0.000732422 72.1828L24.3139 72.1828L13.1366 55.8604L0.000732422 72.1828Z" fill="white"/>
              <path id="Vector_2" d="M65.3601 72.1828L52.2272 55.8604L41.0585 72.1828L65.3601 72.1828Z" fill="white"/>
              <path id="Vector_3" d="M29.3495 41.5757L-2.79063e-06 0.507983L-1.85866e-06 24.4447L32.6873 72.1828L29.3495 41.5757Z" fill="white"/>
              <path id="Vector_4" d="M34.0557 71.6748L66.7303 23.9368L66.7303 4.85657e-05L37.3753 41.0677L34.0557 71.6748Z" fill="white"/>
            </g>
          </g>
          <g id="Random Symboles 11">
            <g id="Group_2">
              <path id="Vector_5" d="M104.004 71.6748L90.8709 55.3524L79.7021 71.6748L104.004 71.6748Z" fill="white"/>
              <path id="Vector_6" d="M67.9934 41.0676L38.6439 -5.85497e-05L38.6439 23.9367L71.3312 71.6747L67.9934 41.0676Z" fill="white"/>
              <path id="Vector_7" d="M71.3312 71.6748L104.006 23.9367L104.006 -2.62351e-05L74.6508 41.0676L71.3312 71.6748Z" fill="white"/>
            </g>
          </g>
        </g>
      </svg>
      <svg width="219" height="20" viewBox="0 0 219 20" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M20.7372 1.07036L25.4332 13.8338L30.5172 1.07036H35.668L28.2829 19.4529H22.7708L17.9678 7.09085L13.1782 19.4529H7.66608L0.267577 1.07036H5.43182L10.4087 13.5662L15.2118 1.07036H20.7372ZM59.2014 18.5431C57.6941 19.0426 56.1867 19.3994 54.6794 19.6135C53.1809 19.8364 51.6468 19.9479 50.0771 19.9479C48.0702 19.9479 46.2819 19.7339 44.7121 19.3057C43.1513 18.8687 41.8357 18.2399 40.7654 17.4193C39.6951 16.5988 38.879 15.5953 38.317 14.4091C37.7551 13.2228 37.4742 11.8805 37.4742 10.382C37.4742 8.99065 37.7551 7.70182 38.317 6.51556C38.8879 5.32038 39.6906 4.28575 40.7252 3.41166C41.7688 2.52866 43.0264 1.84188 44.4981 1.35132C45.9697 0.851844 47.6109 0.602105 49.4215 0.602105C51.0894 0.602105 52.6146 0.829545 53.9971 1.28443C55.3885 1.73039 56.5792 2.39487 57.5692 3.27788C58.5682 4.16088 59.3397 5.24903 59.8838 6.54232C60.4367 7.83561 60.7132 9.32512 60.7132 11.0109V12.2417H42.5983C42.7588 12.8215 43.0219 13.3522 43.3876 13.8338C43.7622 14.3154 44.2662 14.7257 44.8994 15.0646C45.5327 15.4036 46.3087 15.6667 47.2274 15.854C48.155 16.0413 49.2609 16.135 50.5453 16.135C51.4551 16.135 52.347 16.0814 53.2211 15.9744C54.0952 15.8585 54.9113 15.7113 55.6694 15.5329C56.4276 15.3456 57.1099 15.1405 57.7164 14.9175C58.3318 14.6945 58.8268 14.4715 59.2014 14.2485V18.5431ZM55.7764 8.60266C55.7319 8.14778 55.5936 7.67952 55.3617 7.19788C55.1387 6.70732 54.782 6.26582 54.2914 5.87337C53.8008 5.48093 53.1587 5.15983 52.3648 4.9101C51.571 4.65144 50.581 4.52211 49.3947 4.52211C48.2798 4.52211 47.3166 4.66036 46.5049 4.93685C45.6933 5.21335 45.0109 5.55674 44.4579 5.96703C43.9139 6.37731 43.4902 6.81881 43.1869 7.29153C42.8837 7.76425 42.6875 8.20129 42.5983 8.60266H55.7764ZM80.8083 19.4529V17.6468C80.175 17.9946 79.4927 18.3023 78.7613 18.5699C78.0389 18.8375 77.2852 19.0649 76.5003 19.2522C75.7154 19.4395 74.9038 19.5778 74.0653 19.667C73.2359 19.7651 72.3974 19.8141 71.5501 19.8141C70.5601 19.8141 69.6013 19.7205 68.6737 19.5332C67.755 19.3459 66.9389 19.0426 66.2253 18.6234C65.5118 18.2042 64.9365 17.6557 64.4995 16.9778C64.0713 16.3 63.8573 15.4705 63.8573 14.4894C63.8573 13.2496 64.1962 12.2194 64.8741 11.3988C65.5519 10.5694 66.5866 9.89149 67.978 9.36525C69.3694 8.83902 71.1265 8.43319 73.2492 8.14778C75.3809 7.86236 77.9006 7.63938 80.8083 7.47884V7.09085C80.8083 6.7876 80.728 6.4888 80.5675 6.19447C80.4069 5.89121 80.1126 5.62809 79.6845 5.40511C79.2653 5.17321 78.6855 4.98591 77.9452 4.8432C77.2138 4.70049 76.2773 4.62914 75.1357 4.62914C74.2348 4.62914 73.3429 4.6782 72.4599 4.77631C71.5858 4.8655 70.7385 4.99037 69.9179 5.15092C69.1062 5.31146 68.3347 5.49877 67.6034 5.71283C66.872 5.92689 66.2075 6.14987 65.6099 6.38177V1.96675C66.2343 1.8062 66.9344 1.65012 67.7104 1.49849C68.4864 1.34686 69.2936 1.21753 70.132 1.1105C70.9704 0.994551 71.8177 0.905359 72.6739 0.842924C73.5302 0.77157 74.3508 0.735893 75.1357 0.735893C76.6787 0.735893 78.1013 0.865222 79.4035 1.12388C80.7057 1.37362 81.8251 1.76607 82.7616 2.30122C83.707 2.83637 84.4429 3.51424 84.9691 4.33481C85.5043 5.15538 85.7718 6.13203 85.7718 7.26477V19.4529H80.8083ZM80.8083 11.0644C78.8996 11.1357 77.2763 11.2383 75.9384 11.3721C74.6094 11.5059 73.5034 11.662 72.6204 11.8403C71.7374 12.0187 71.0417 12.2105 70.5333 12.4156C70.0338 12.6208 69.6592 12.8304 69.4095 13.0444C69.1598 13.2585 69.0037 13.4726 68.9412 13.6866C68.8877 13.9007 68.861 14.0969 68.861 14.2753C68.861 14.4894 68.9189 14.699 69.0349 14.9041C69.1508 15.1003 69.3515 15.2742 69.6369 15.4259C69.9313 15.5775 70.3193 15.6979 70.8009 15.7871C71.2825 15.8763 71.889 15.9209 72.6204 15.9209C73.4321 15.9209 74.2259 15.8585 75.0019 15.7336C75.7778 15.6087 76.5137 15.4393 77.2094 15.2252C77.9051 15.0022 78.5562 14.7436 79.1627 14.4492C79.7781 14.146 80.3266 13.8249 80.8083 13.4859V11.0644ZM101.612 5.07064V19.4529H96.6489V5.07064H88.849V1.07036H109.426V5.07064H101.612ZM130.31 19.4529V11.7868H117.68V19.4529H112.717V1.07036H117.68V7.75979H130.31V1.07036H135.274V19.4529H130.31ZM161.523 18.5431C160.016 19.0426 158.508 19.3994 157.001 19.6135C155.502 19.8364 153.968 19.9479 152.399 19.9479C150.392 19.9479 148.603 19.7339 147.034 19.3057C145.473 18.8687 144.157 18.2399 143.087 17.4193C142.017 16.5988 141.2 15.5953 140.639 14.4091C140.077 13.2228 139.796 11.8805 139.796 10.382C139.796 8.99065 140.077 7.70182 140.639 6.51556C141.209 5.32038 142.012 4.28575 143.047 3.41166C144.09 2.52866 145.348 1.84188 146.82 1.35132C148.291 0.851844 149.932 0.602105 151.743 0.602105C153.411 0.602105 154.936 0.829545 156.319 1.28443C157.71 1.73039 158.901 2.39487 159.891 3.27788C160.89 4.16088 161.661 5.24903 162.205 6.54232C162.758 7.83561 163.035 9.32512 163.035 11.0109V12.2417H144.92C145.08 12.8215 145.343 13.3522 145.709 13.8338C146.084 14.3154 146.588 14.7257 147.221 15.0646C147.854 15.4036 148.63 15.6667 149.549 15.854C150.476 16.0413 151.582 16.135 152.867 16.135C153.777 16.135 154.668 16.0814 155.543 15.9744C156.417 15.8585 157.233 15.7113 157.991 15.5329C158.749 15.3456 159.431 15.1405 160.038 14.9175C160.653 14.6945 161.148 14.4715 161.523 14.2485V18.5431ZM158.098 8.60266C158.053 8.14778 157.915 7.67952 157.683 7.19788C157.46 6.70732 157.103 6.26582 156.613 5.87337C156.122 5.48093 155.48 5.15983 154.686 4.9101C153.893 4.65144 152.902 4.52211 151.716 4.52211C150.601 4.52211 149.638 4.66036 148.826 4.93685C148.015 5.21335 147.332 5.55674 146.779 5.96703C146.235 6.37731 145.812 6.81881 145.508 7.29153C145.205 7.76425 145.009 8.20129 144.92 8.60266H158.098ZM184.454 5.23119C184.32 5.18659 184.124 5.12862 183.866 5.05726C183.616 4.97699 183.322 4.90118 182.983 4.82982C182.644 4.74955 182.269 4.68266 181.859 4.62914C181.457 4.57562 181.043 4.54887 180.615 4.54887C179.723 4.54887 178.889 4.66036 178.113 4.88334C177.346 5.0974 176.628 5.38728 175.959 5.75296C175.29 6.10973 174.665 6.52002 174.086 6.98382C173.515 7.4387 172.989 7.90696 172.507 8.3886V19.4529H167.543V1.07036H172.507V4.05385C173.105 3.60789 173.716 3.17976 174.34 2.76948C174.973 2.35028 175.629 1.98013 176.307 1.65903C176.993 1.33794 177.716 1.08374 178.474 0.89644C179.232 0.700217 180.035 0.602105 180.882 0.602105C181.203 0.602105 181.529 0.619943 181.859 0.65562C182.198 0.682378 182.523 0.718055 182.835 0.762651C183.157 0.807247 183.455 0.856303 183.732 0.909819C184.008 0.963334 184.249 1.01685 184.454 1.07036V5.23119ZM210.075 10.0208L218.798 19.4529H212.844L207.091 13.2585L201.365 19.4529H195.425L204.135 10.0208L195.853 1.07036H201.807L207.091 6.82327L212.403 1.07036H218.356L210.075 10.0208Z" fill="white"/>
      </svg>
    </div>
    <div class="first-page" :class="{'is-closing': isClosing, 'is-closed': isClosed}">
      <div class="img-header-container">
        <img src="../assets/img/star-1.png">
      </div>
      <h1>Let’s See<br>The <svg width="36" height="36" viewBox="0 0 36 36" fill="none" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
      <path d="M0 35.466H35.2284V0.237555H0V35.466Z" fill="url(#pattern0)"/>
      <defs>
      <pattern id="pattern0" patternContentUnits="objectBoundingBox" width="1" height="1">
      <use xlink:href="#image0_1_91" transform="scale(0.015625)"/>
      </pattern>
      <image id="image0_1_91" width="64" height="64" xlink:href="data:image/png;base64,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"/>
      </defs>
      </svg><br>Weather<br>Around you</h1>
      <button class="button" @click="hideFirstPage()">Let's Check</button>
    </div>
    <div class="content">
      <transition>
        <component :is="getContentComponent()" :key="activeTab" v-show="!isTabClosing" :class="{'is-opening': isTabOpening, 'is-closing': isTabClosing}"></component>
      </transition>
    </div>
    <navBar class="nav-bar" @tab-selected="changeTab"></navBar>
  </div>
</template>

<script>
import navBar from '@/components/navBar.vue'
import HomeComponent from'@/components/HomeComponent.vue'
import MoodComponent from'@/components/MoodComponent.vue'
import MapsComponent from'@/components/MapsComponent.vue'
import SettingsComponent from'@/components/SettingsComponent.vue'

export default {
  name: 'HomeView',
  components: {
    navBar
  },
  data() {
    return {
      isClosing: false,
      isClosed: false,
      activeTab: 'Home',
      isTabClosing: false,
      isTabOpening: false,
      loadingScreen: true,
      loadingClosing: false,
    };
  },
  methods: {
    hideLoadingScreen() {
      setTimeout(() => {
        this.loadingClosing = true;
        setTimeout(() => {
          this.loadingScreen = false;
        }, 300);
      }, 1000);
    },
    hideFirstPage(){
      this.isClosing = true;
      setTimeout(() => {
        this.isClosed = true;
      },500);
    },
    changeTab(tab) {
      this.isTabClosing = true
      setTimeout(() => {
        this.activeTab = tab;
        this.isTabClosing = false;
        this.isTabOpening = true;
        setTimeout(() => {
          this.isTabOpening = false;
        }, 500);
      }, 500);
    },
    getContentComponent() {
      switch (this.activeTab) {
        case 'Home':
          return HomeComponent;
        case 'Mood':
          return MoodComponent;
        case 'Maps':
          return MapsComponent;
        case 'Settings':
          return SettingsComponent;
        default:
          return HomeComponent;
      }
    },
  },
  mounted() {
    this.hideLoadingScreen()
  }
}
</script>

<style lang="scss" scoped>
.home {
  font-family: "Poppins-Regular";
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  color: #0C1823;
  width: 374px;
  height: 812px;
  background-color: white;
  border-radius: 50px;
  display: flex;
  flex-direction: column;
  align-items: center;
  overflow: hidden;
  .dynamic-island {
    position: absolute;
    z-index: 105;
    background-color: black;
    width: 25%;
    height: 30px;
    border-radius: 30px;
    top: 10px;
    transition: transform .1s ease-in-out;
    &:active {
      transform: scale(1.05);
      transition: transform .1s ease-in-out;
    }
  }
  .loading {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    background-color: #0C1823;
    z-index: 102;
    width: 100%;
    height: 100%;
    position: absolute;
    gap: 30px;
    &.hide {
      display: none;
    }
    &.anim {
      opacity: 0;
      transition: all .3s ease-in;
    }
  }
  .first-page {
    z-index: 99;
    position: absolute;
    background-color: white;
    width: 100%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-direction: column;
    height: 100%;
    .img-header-container {
      display: flex;
      justify-content: flex-end;
      width: 101%;
    }
    h1 {
      font-family: "Poppins-Bold";
      font-size: 42px;
      font-weight: 700;
      line-height: 110%;
    }
    .button {
      padding: 20px 89px 20px 90px;
      border-radius: 16px;
      background: #0C1823;
      color: white;
      border: none;
      margin-bottom: 77px;
      cursor: pointer;
    }
    &.is-closing {
      animation: isClosing .5s forwards ease;
    }
    @keyframes isClosing {
      from {
        transform: translateY(0);
        opacity: 1;
      }
      to {
        transform: translateY(-100%);
        opacity: 0;
      }
    }
    &.is-closed {
      display: none;
    }
  }
  .content {
    height: 88%;
    width: 100%;
    padding: 30px 30px 0px 30px;
    div {
      &.is-opening {
        animation: isTabOpening .5s forwards ease;
      }
      @keyframes isTabOpening {
        from {
          transform: translateY(5%);
          opacity: 0;
        }
        to {
          transform: translateY(0%);
          opacity: 1;
        }
      }
      &.is-closing {
        animation: isTabClosing .5s forwards ease;
      }
      @keyframes isTabClosing {
        from {
          transform: translateX(0%);
          opacity: 1;
        }
        to {
          transform: translateX(-100%);
          opacity: 0;
        }
      }
    }
  }
  .nav-bar {
    height: 12%;
    width: 100%;
  }
}
</style>
