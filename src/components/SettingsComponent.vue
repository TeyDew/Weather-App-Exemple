<template>
  <div>
    <div class="header">
      <div class="left-side side">
        <img src="../assets/img/back-arrow.png">
      </div>
      <div class="middle-side side">
      </div>
      <div class="right-side side">
        <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path fill-rule="evenodd" clip-rule="evenodd" d="M12.5573 13.3341H8.77599C8.22115 13.3294 7.68721 13.5454 7.29162 13.9345C6.89604 14.3236 6.67123 14.8539 6.66666 15.4087V23.2607C6.67692 24.4156 7.62111 25.3437 8.77599 25.3341H12.5573C13.1122 25.3387 13.6461 25.1227 14.0417 24.7336C14.4373 24.3445 14.6621 23.8142 14.6667 23.2594V15.4087C14.6621 14.8539 14.4373 14.3236 14.0417 13.9345C13.6461 13.5454 13.1122 13.3294 12.5573 13.3341Z" stroke="#36424D" stroke-width="1.2" stroke-linecap="round" stroke-linejoin="round"/>
          <path fill-rule="evenodd" clip-rule="evenodd" d="M12.5573 5.33415H8.77599C7.64433 5.30276 6.70077 6.19324 6.66666 7.32482V8.67681C6.70077 9.80839 7.64433 10.6989 8.77599 10.6675H12.5573C13.689 10.6989 14.6325 9.80839 14.6667 8.67681V7.32482C14.6325 6.19324 13.689 5.30276 12.5573 5.33415Z" stroke="#36424D" stroke-width="1.2" stroke-linecap="round" stroke-linejoin="round"/>
          <path fill-rule="evenodd" clip-rule="evenodd" d="M19.4427 17.3342H23.2227C23.7777 17.3392 24.312 17.1234 24.7079 16.7343C25.1038 16.3451 25.3288 15.8146 25.3333 15.2596V7.40891C25.3288 6.85407 25.1039 6.32377 24.7084 5.93469C24.3128 5.54562 23.7788 5.32962 23.224 5.33424H19.4427C18.8878 5.32962 18.3539 5.54562 17.9583 5.93469C17.5627 6.32377 17.3379 6.85407 17.3333 7.40891V15.2596C17.3379 15.8144 17.5627 16.3447 17.9583 16.7338C18.3539 17.1229 18.8878 17.3389 19.4427 17.3342Z" stroke="#36424D" stroke-width="1.2" stroke-linecap="round" stroke-linejoin="round"/>
          <path fill-rule="evenodd" clip-rule="evenodd" d="M19.4427 25.3341H23.2227C24.3548 25.3663 25.2992 24.4756 25.3333 23.3435V21.9915C25.2992 20.8599 24.3557 19.9694 23.224 20.0008H19.4427C18.311 19.9694 17.3674 20.8599 17.3333 21.9915V23.3421C17.3667 24.4742 18.3105 25.3655 19.4427 25.3341Z" stroke="#36424D" stroke-width="1.2" stroke-linecap="round" stroke-linejoin="round"/>
        </svg>
      </div>
    </div>
    <div class="settings">
      <h2>General Settings</h2>
      <div class="settings-item">
        <div class="icon-side">
          <img src="../assets/img/icons/user-icon.png">
        </div>
        <span>Account</span>
        <div class="right-side"></div>
      </div>
      <div class="settings-item">
        <div class="icon-side">
          <img src="../assets/img/icons/location-icon.png">
        </div>
        <span>Location</span>
        <div class="right-side"></div>
      </div>
      <div class="settings-item">
        <div class="icon-side">
          <img src="../assets/img/icons/alerte-icon.png">
        </div>
        <span>Notifications</span>
        <div class="right-side">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" @click="changeNotif()" :class="{'silence': NotifMode}">
            <g id="Xnix/Line/Notification_Slient">
              <g id="Vector">
                <path id="Vector_2" d="M10.392 4.75C9.97779 4.75 9.642 5.08579 9.642 5.5C9.642 5.91421 9.97779 6.25 10.392 6.25V4.75ZM13.749 6.25C14.1632 6.25 14.499 5.91421 14.499 5.5C14.499 5.08579 14.1632 4.75 13.749 4.75V6.25ZM14.049 16.629C13.6348 16.629 13.299 16.9648 13.299 17.379C13.299 17.7932 13.6348 18.129 14.049 18.129V16.629ZM16.433 17.379V18.1291L16.4426 18.1289L16.433 17.379ZM17.838 16.56L18.4858 16.9379C18.5021 16.91 18.5165 16.8811 18.5291 16.8514L17.838 16.56ZM17.608 14.667L16.8934 14.8947C16.9187 14.974 16.957 15.0486 17.0068 15.1154L17.608 14.667ZM17.008 11.695L17.755 11.6276C17.7531 11.6065 17.7503 11.5854 17.7466 11.5645L17.008 11.695ZM16.1574 8.37146C15.8754 8.06803 15.4009 8.05063 15.0975 8.33259C14.794 8.61455 14.7766 9.08911 15.0586 9.39254L16.1574 8.37146ZM14.04 18.132C14.4542 18.132 14.79 17.7962 14.79 17.382C14.79 16.9678 14.4542 16.632 14.04 16.632V18.132ZM10.09 16.632C9.67579 16.632 9.34 16.9678 9.34 17.382C9.34 17.7962 9.67579 18.132 10.09 18.132V16.632ZM14.8 17.382C14.8 16.9678 14.4642 16.632 14.05 16.632C13.6358 16.632 13.3 16.9678 13.3 17.382H14.8ZM10.84 17.382C10.84 16.9678 10.5042 16.632 10.09 16.632C9.67579 16.632 9.34 16.9678 9.34 17.382H10.84ZM10.09 18.132C10.5042 18.132 10.84 17.7962 10.84 17.382C10.84 16.9678 10.5042 16.632 10.09 16.632V18.132ZM7.706 17.382L7.70437 18.132H7.706V17.382ZM7.44678 16.5887C7.0545 16.4557 6.62868 16.6659 6.4957 17.0582C6.36272 17.4505 6.57293 17.8763 6.96522 18.0093L7.44678 16.5887ZM19.5303 6.03033C19.8232 5.73744 19.8232 5.26256 19.5303 4.96967C19.2374 4.67678 18.7626 4.67678 18.4697 4.96967L19.5303 6.03033ZM15.0877 8.35167C14.7948 8.64456 14.7948 9.11944 15.0877 9.41233C15.3806 9.70522 15.8554 9.70522 16.1483 9.41233L15.0877 8.35167ZM4.46967 18.9697C4.17678 19.2626 4.17678 19.7374 4.46967 20.0303C4.76256 20.3232 5.23744 20.3232 5.53033 20.0303L4.46967 18.9697ZM7.73033 17.8303C8.02322 17.5374 8.02322 17.0626 7.73033 16.7697C7.43744 16.4768 6.96256 16.4768 6.66967 16.7697L7.73033 17.8303ZM16.1453 9.41533C16.4382 9.12244 16.4382 8.64756 16.1453 8.35467C15.8524 8.06178 15.3776 8.06178 15.0847 8.35467L16.1453 9.41533ZM6.66967 16.7697C6.37678 17.0626 6.37678 17.5374 6.66967 17.8303C6.96256 18.1232 7.43744 18.1232 7.73033 17.8303L6.66967 16.7697ZM13.6175 8.37159C13.9989 8.53316 14.439 8.35495 14.6006 7.97354C14.7622 7.59214 14.5839 7.15198 14.2025 6.99041L13.6175 8.37159ZM12.07 7.308L12.0695 6.558C12.0623 6.55801 12.0552 6.55811 12.048 6.55832L12.07 7.308ZM7.126 11.7L6.38414 11.5898C6.38203 11.604 6.38033 11.6183 6.37904 11.6326L7.126 11.7ZM6.526 14.672L7.17677 15.0448C7.20312 14.9988 7.22452 14.9502 7.24061 14.8997L6.526 14.672ZM5.49136 15.1828C5.36919 15.5786 5.591 15.9985 5.98679 16.1206C6.38258 16.2428 6.80246 16.021 6.92464 15.6252L5.49136 15.1828ZM10.392 6.25H13.749V4.75H10.392V6.25ZM14.049 18.129H16.433V16.629H14.049V18.129ZM16.4426 18.1289C17.2855 18.1182 18.0611 17.6661 18.4858 16.9379L17.1902 16.1821C17.0308 16.4554 16.7397 16.625 16.4234 16.6291L16.4426 18.1289ZM18.5291 16.8514C18.8969 15.9792 18.7752 14.9774 18.2092 14.2186L17.0068 15.1154C17.2547 15.4478 17.308 15.8865 17.1469 16.2686L18.5291 16.8514ZM18.3226 14.4393C18.0315 13.5256 17.8412 12.5827 17.755 11.6276L16.261 11.7624C16.3571 12.8264 16.5691 13.8767 16.8934 14.8947L18.3226 14.4393ZM17.7466 11.5645C17.5354 10.3693 16.9836 9.26055 16.1574 8.37146L15.0586 9.39254C15.6881 10.07 16.1086 10.9148 16.2694 11.8255L17.7466 11.5645ZM14.04 16.632H10.09V18.132H14.04V16.632ZM13.3 17.382C13.3 17.8214 13.0656 18.2275 12.685 18.4472L13.435 19.7462C14.2797 19.2586 14.8 18.3573 14.8 17.382H13.3ZM12.685 18.4472C12.3044 18.6669 11.8356 18.6669 11.455 18.4472L10.705 19.7462C11.5497 20.2339 12.5903 20.2339 13.435 19.7462L12.685 18.4472ZM11.455 18.4472C11.0744 18.2275 10.84 17.8214 10.84 17.382H9.34C9.34 18.3573 9.86034 19.2586 10.705 19.7462L11.455 18.4472ZM10.09 16.632H7.706V18.132H10.09V16.632ZM7.70763 16.632C7.61891 16.6318 7.53081 16.6172 7.44678 16.5887L6.96522 18.0093C7.20332 18.09 7.45296 18.1315 7.70437 18.132L7.70763 16.632ZM18.4697 4.96967L15.0877 8.35167L16.1483 9.41233L19.5303 6.03033L18.4697 4.96967ZM5.53033 20.0303L7.73033 17.8303L6.66967 16.7697L4.46967 18.9697L5.53033 20.0303ZM15.0847 8.35467L6.66967 16.7697L7.73033 17.8303L16.1453 9.41533L15.0847 8.35467ZM14.2025 6.99041C13.5278 6.70456 12.8023 6.5575 12.0695 6.558L12.0705 8.058C12.602 8.05764 13.1281 8.16429 13.6175 8.37159L14.2025 6.99041ZM12.048 6.55832C9.19054 6.64218 6.80414 8.76215 6.38414 11.5898L7.86786 11.8102C8.1811 9.7013 9.96089 8.12022 12.092 8.05768L12.048 6.55832ZM6.37904 11.6326C6.29284 12.5877 6.1025 13.5306 5.81139 14.4443L7.24061 14.8997C7.5649 13.8817 7.77695 12.8314 7.87296 11.7674L6.37904 11.6326ZM5.87523 14.2992C5.71511 14.5787 5.58637 14.875 5.49136 15.1828L6.92464 15.6252C6.98704 15.423 7.0716 15.2284 7.17677 15.0448L5.87523 14.2992Z"/>
              </g>
            </g>
          </svg>
        </div>
      </div>
      <h2>Temperature</h2>
      <div class="settings-item">
        <label for="celsius">Celsius</label>
        <div class="right-side">
          <input type="checkbox" class="checkbox" id="celsius" name="Celsius" checked>
          <label for="celsius"></label>
        </div>
      </div>
      <div class="settings-item">
        <label for="fahrenheit">Fahrenheit</label>
        <div class="right-side">
          <input type="checkbox" class="checkbox" id="fahrenheit" name="Fahrenheit">
          <label for="fahrenheit"></label>
        </div>
      </div>
      <br>
      <div class="settings-item">
        <div class="icon-side">
          <img src="../assets/img/icons/terms-icon.png">
        </div>
        <span class="link">Terms and services</span>
        <div class="right-side"></div>
      </div>
      <div class="settings-item">
        <div class="icon-side">
          <img src="../assets/img/icons/about-icon.png">
        </div>
        <span class="link">About</span>
        <div class="right-side"></div>
      </div>
      <div class="settings-item">
        <div class="icon-side">
          <img src="../assets/img/icons/bug-icon.png">
        </div>
        <span class="link">Report bug</span>
        <div class="right-side"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SettingsComponent',
  data() {
    return {
      NotifMode: 0,
      navActive: 'home',
    };
  },
  methods: {
    changeNotif(){
      if (this.NotifMode) {
        this.NotifMode = 0;
      } else {
        this.NotifMode = 1;
      }
    },
    selectTab(tab) {
      this.$emit('tab-selected', tab);
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
div {
  .header {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 20px;
    height: 90px;
    .side {
      display: flex;
      align-items: center;
      &.left-side {
        width: 40px;
        height: 100%;
      }
      &.middle-side {
        width: calc(100% - 100px);
      }
      &.right-side {
        width: 40px;
        height: 100%;
      }
    }
  }
  .settings {
    padding: 40px;
    h2 {
      color: #000;
      font-size: 15px;
      font-family: 'Poppins-Bold';
      font-weight: 500;
      line-height: 110.5%;
      margin-bottom: 25px;
      margin-top: 25px;
      &:first-child {
        margin-top: 0;
      }
    }
    .settings-item {
      display: flex;
      padding: 5px 0px;
      width: 100%;
      justify-content: space-between;
      .icon-side {
        width: 10%;
      }
      span {
        width: 70%;
        &.link {
          cursor: pointer;
        }
      }
      .right-side {
        width: 10%;
        position: relative;
        svg {
          cursor: pointer;
          g {
            g {
              path {
                fill: #E13D6E;
              }
            }
          }
          &.silence {
            g {
              g {
                path {
                  fill: #D9D9D9;
                }
              }
            }
          }
        }
        .checkbox {
          visibility: hidden;
          &:checked + label {
            background-color: #3EB98D;
            &::after {
              opacity: 1;
              border: 2px solid #fff;
              border-top: none;
              border-right: none;
            }
          }
        }
        label {
          background-color: #D9D9D9;
          border-radius: 50%;
          cursor: pointer;
          height: 24px;
          left: 0;
          position: absolute;
          top: 0;
          width: 24px;
          &::after {
            border: 2px solid #E3E3E3;
            border-top: none;
            border-right: none;
            content: "";
            height: 5px;
            left: 6px;
            position: absolute;
            top: 7px;
            transform: rotate(-45deg);
            width: 10px;
          }
        }
      }
    }
  }
}
</style>