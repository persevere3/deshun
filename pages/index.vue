<style lang="scss">
*,
:after,
:before {
  box-sizing: border-box;
  font-family: HelveticaNeue;
  list-style: none;
  margin: 0;
  padding: 0;
  vertical-align: middle
}

a {
  text-decoration: none
}

img {
  width: 100%
}

header {
  align-items: center;
  background-color: #171a1e;
  display: flex;
  position: relative
}

header .toggle_nav {
  cursor: pointer;
  display: none;
  left: 5.1282vw;
  position: absolute;
  top: 5.1282vw;
  width: 5.1282vw
}

header .logo {
  cursor: pointer;
  margin-left: 1.015625vw;
  margin-right: auto;
  width: 24.453125vw;
  z-index: 2
}

header .logo a {
  display: block;
  height: 100%;
  width: 100%
}

header .logo_decoration {
  left: 0;
  position: absolute;
  top: 9.5vw;
  width: 52.851562vw;
  z-index: 1
}

header nav {
  margin-right: 7.8125vw
}

header nav ul {
  display: flex
}

header nav ul li {
  cursor: pointer;
  font-size: 16px;
  margin-right: 3.984375vw
}

header nav ul li:last-child {
  margin-right: 0
}

header nav ul li a {
  align-items: center;
  color: #fff;
  display: flex;
  flex-direction: column;
  justify-content: center
}

header nav ul li a:hover {
  color: #d19e42
}

header nav ul li a div:first-child {
  margin-bottom: 3px
}

@media (max-width: 767px) {
  header .toggle_nav {
    display: block
  }

  header .logo {
    margin: 0 auto;
    width: 32.820512vw
  }

  header .logo_decoration {
    left: 50%;
    top: 15vw;
    transform: translate(-50%);
    width: 60.897435vw
  }

  header nav {
    background: rgba(23, 26, 30, .6);
    height: 100vh;
    margin-right: 0;
    position: fixed;
    right: -200px;
    top: 0;
    transform: translate(0);
    transition: .3s;
    width: 200px;
    z-index: 100
  }

  header nav.active {
    transform: translate(-200px)
  }

  header nav ul {
    flex-direction: column;
    padding-top: 100px
  }

  header nav ul li {
    font-size: 12px;
    margin-bottom: 15px;
    margin-right: 0
  }
}

.banner {
  background-color: #171a1e;
  position: relative
}

.banner .img {
  margin: 0 auto;
  width: 84.375vw
}

.banner .text {
  bottom: 2.65625vw;
  color: #fff;
  font-size: 28px;
  left: 50%;
  position: absolute;
  transform: translate(-50%)
}

@media (max-width: 767px) {
  .banner {
    padding-bottom: 7.692307vw
  }

  .banner .img {
    width: 88.974358vw
  }

  .banner .text {
    bottom: 0;
    font-size: 16px;
    height: 7.692307vw;
    line-height: 7.692307vw;
    text-align: center;
    width: 100%
  }
}

.about {
  line-height: 1.5;
  margin-top: 1.875vw
}

.about .text {
  color: #707070;
  font-size: 16px;
  text-align: center
}

.about .text:first-child {
  padding: 0 6.461538vw
}

.about .text:nth-child(2) {
  margin-top: 2.734375vw;
  padding: 0 8.461538vw
}

.about .text:nth-child(2) .img {
  margin: 0 auto 4.0625vw;
  width: 68.476562vw
}

.about .text:nth-child(2) .img.m {
  display: none
}

@media (max-width: 767px) {
  .about {
    margin-top: 4.102564vw
  }

  .about .text {
    font-size: 12px
  }

  .about .text:nth-child(2) {
    align-items: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
    margin-top: 4.871794vw;
    position: relative
  }

  .about .text:nth-child(2):before {
    border: 1px solid #707070;
    bottom: 0;
    content: "";
    height: 70%;
    left: 50%;
    position: absolute;
    transform: translate(-50%);
    width: 82.564102vw;
    z-index: -1
  }

  .about .text:nth-child(2) .img {
    display: none;
    margin: 0
  }

  .about .text:nth-child(2) .img.m {
    display: block
  }

  .about .text:nth-child(2) .text_content {
    padding: 4.102564vw;
    width: 82.564102vw
  }
}

.project {
  align-items: center;
  color: #0f1233;
  display: flex;
  flex-direction: column;
  margin: 5.390625vw auto 0;
  width: 84.375vw
}

.project .project_title {
  border-bottom: 3px solid #0f1233;
  font-size: 28px;
  padding-bottom: 1.015625vw;
  width: 100%
}

.project .img_text {
  align-items: center;
  display: flex;
  flex-direction: column;
  margin: 4.615384vw 0;
  position: relative
}

.project .img_text:before {
  background-color: #0f1233;
  bottom: 0;
  content: "";
  height: 2px;
  left: 50%;
  position: absolute;
  transform: translate(-50%, 4.615384vw);
  width: 71.282051vw
}

.project .img_text:last-child {
  margin-bottom: 0
}

.project .img_text:last-child:before {
  display: none
}

.project .img_text .img .rendered {
  cursor: pointer;
  position: relative
}

.project .img_text .img .rendered:after,
.project .img_text .img .rendered:before {
  align-items: center;
  background: hsla(0, 0%, 100%, .6);
  border-radius: 5px;
  display: flex;
  height: 40px;
  justify-content: center;
  opacity: 0;
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  transition: .3s;
  width: 80px;
  z-index: 1
}

.project .img_text .img .rendered:before {
  content: "Before";
  left: 2%
}

.project .img_text .img .rendered:after {
  content: "After";
  right: 2%
}

.project .img_text .img .rendered:hover:after,
.project .img_text .img .rendered:hover:before {
  opacity: 1
}

.project .img_text .text {
  border: 1px solid #707070;
  font-size: 16px;
  margin-top: 6.1538461vw;
  padding: 2.109375vw 1.171875vw;
  width: 80%
}

.project .img_text .text .row {
  display: flex;
  margin-bottom: 2.109375vw
}

.project .img_text .text .row:last-child {
  margin: 0
}

.project .img_text .text .row .row_title {
  white-space: nowrap
}

.slider-customization {
  --divider-width: 3px;
  --default-handle-width: 50px
}

.slider-customization:focus {
  outline: none
}

@media (max-width: 767px) {
  .project .project_title {
    font-size: 16px;
    padding-left: 2.179487vw
  }

  .project .img_text {
    width: 64.358974vw
  }

  .project .img_text .img .rendered:after,
  .project .img_text .img .rendered:before {
    font-size: 12px;
    height: 25px;
    opacity: 1;
    width: 50px
  }

  .project .img_text .text {
    font-size: 12px;
    width: 100%
  }
}

footer {
  background-color: #0f1233;
  color: #d3d3d3;
  font-size: 12px;
  line-height: 1.5;
  margin-top: 8.671875vw;
  position: relative
}

footer .contact,
footer .copyright {
  border: 1px solid #707070
}

footer .contact {
  justify-content: center;
  padding: 1.171875vw 22.65625vw
}

footer .contact .row {
  display: flex
}

footer .contact .row.company {
  font-size: 14px;
  margin-bottom: 10px
}

footer .contact .row .column:first-child {
  flex-shrink: 0;
  width: 14vw
}

footer .copyright {
  padding: .585937vw 22.65625vw
}

@media (max-width: 767px) {
  footer .contact {
    padding: 1.171875vw 7vw
  }

  footer .contact .row .column:first-child {
    width: 30vw
  }

  footer .copyright {
    padding: .585937vw 7vw
  }
}

.line {
  bottom: 220px;
  right: 15px;
  width: 50px
}

.line,
.up {
  cursor: pointer;
  position: fixed
}

.up {
  bottom: 120px;
  right: 0;
  width: 80px
}

@media (max-width: 767px) {
  .line {
    bottom: 180px;
    right: 5px;
    width: 40px
  }

  .up {
    bottom: 120px;
    right: 0;
    width: 50px
  }
}
</style>

<template>
  <header id="home">
    <div class="toggle_nav" tabindex="0" @click="is_nav_active = !is_nav_active" @blur="is_nav_active = false">
      <img
        src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADwAAAA5BAMAAACYH1XyAAAAElBMVEVHcEzbq0jcqkfcqUbcqkfcqkeZqCvTAAAABXRSTlMAQL+i5kIlfocAAAA7SURBVDjLYwjFBwIYhq30SAW4wyR4WEsL4gbDOr6VsAED/MnBYRhIY41pgeGfv5VwAAH82X/IS+PP3AAjYg0ZLyaXlgAAAABJRU5ErkJggg=="
        alt="">
    </div>
    <div class="logo"><a href=""><img src="@/images/logo.png" alt=""></a></div>
    <div class="logo_decoration"><img src="@/images/logo_decoration.png" alt=""></div>
    <nav :class="{ active: is_nav_active }">
      <ul>
        <li><a aria-current="page" href="/#home" class="router-link-active router-link-exact-active">
            <div>首頁</div>
            <div>HOME</div>
          </a></li>
        <li><a aria-current="page" href="/#about" class="router-link-active router-link-exact-active">
            <div>關於德舜</div>
            <div>ABOUT</div>
          </a></li>
        <li><a aria-current="page" href="/#project" class="router-link-active router-link-exact-active">
            <div>實績案例</div>
            <div>PROJECT</div>
          </a></li>
        <li><a aria-current="page" href="/#contact" class="router-link-active router-link-exact-active">
            <div>聯絡我們</div>
            <div>CONTACT</div>
          </a></li>
      </ul>
    </nav>
  </header>
  <div class="banner">
    <div class="img"><img src="@/images/banner.png" alt=""></div>
    <div class="text"> 建築夢想，實現無限 </div>
  </div>
  <div class="about" id="about">
    <div class="text"> 我們致力於提供卓越建築與工程解決方案的專業公司。<br> 憑藉多年的經驗和優秀的團隊，創造令人驚嘆的建築作品。<br> 透過創新設計，不斷超越客戶期望，成為您可靠的合作夥伴。<br>
    </div>
    <div class="text">
      <div class="img"><img src="@/images/about1.png" alt=""></div>
      <div class="img m"><img src="@/images/about1_m.png" alt=""></div>
      <div class="text_content"> 德舜營造公司提供全面的建築與工程服務，包括建築設計、工程施工、室內裝修、土木工程等。<br>
        我們的專業團隊擁有深厚的專業知識和技術能力，能夠迅速響應客戶需求並提供度身訂造的解決方案。<br> 以高品質施工、精細工藝和專業管理為核心價值，確保每個項目都達到卓越水平。<br></div>
    </div>
  </div>
  <div class="project" id="project">
    <div class="project_title"> 案例實績 </div>
    <div class="img_text">
      <ClientOnly>
        <div class="img">
          <img-comparison-slider class="slider-customization rendered" tabindex="0">
            <img slot="first" src="@/images/before1.jpg">
            <img slot="second" src="@/images/after1.jpg">
          </img-comparison-slider>
        </div>
      </ClientOnly>
      <div class="text">
        <div class="row">
          <div class="row_title"> 案場名稱： </div>
          <div class="row_contemt">中興大樓外牆整修工程案</div>
        </div>
        <div class="row">
          <div class="row_title"> 施作項目： </div>
          <div class="row_contemt">假設及拆除工程、東向與南向磁磚面工程、西南向及北向帷幕面工程、騎樓整修工程</div>
        </div>
      </div>
    </div>
  </div>
  <footer>
    <div class="contact" id="contact">
      <div class="row company"> 德舜營造股份有限公司 </div>
      <div class="row">
        <div class="column"> 電話：04-24714109 </div>
        <div class="column"> 信箱：deshun202201@gmail.com </div>
      </div>
      <div class="row">
        <div class="column"> 傳真：04-24714139 </div>
        <div class="column"> 地址：台中市南屯區大墩二街120號1樓 </div>
      </div>
    </div>
    <div class="copyright"> Copyright © 2023 - All Rights Eeserved - DESHUN . </div>
    <div class="line"><a href="https://line.me/ti/p/KVl18VQqbm"><img
          src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACkAAAApCAMAAACfvvDEAAAAyVBMVEVHcEwj2TML1RgA0AwA3hch3DIXySAr3j4A2QoS1x0A4BsA1RApwS0A2hMAwggAzwoN3yQWzSEAwQYZzST///8A3xoA4RsA2RUA3BcApAAA1hAA3hgA1hYApgEA0RAAzBIAyA8BvAsAxA4AuAgAtAYi4jgX3i4AwQwAqgIArwQtty9AzkjA7sLQ89KA6IkuwDPA9MSw67Pw/PAP2SE/3U4Z0ioUxx5g4Wug6KRAv0GQ5JVv5Hkwzzrg9uEQrBBP0VYQ3ybg+uJQ3VyZCFHdAAAAFHRSTlMAvz7wnHKb+hAfz8/tMNvA3S5XzrGAVkkAAAJTSURBVDjLldVrd6IwEAbgWGvR7m7b3Y0FMSCIiiwXBRGol2r3//+onUkiF8UP+3qOH9LnDOmQjIRgBr2OMm+N0ukNSJUnVUSDjCFDzHuZx750/W+6rjfpuEmffwiJUFpNay/7zKs+ZZCJqdd2cGsfAf40RvAxRiPPsfSbHZT0AUqOqiwd67rq+7As+r2CBsTbplEU7dPzuGnfCPlThx9FQmXC/blBaxLckTZSnMVer6TxGdPrJGnV2lIanyFtSV5SKY07sEaFhHbG7ZAmc0m5xH+a3kssu4US24glkwC/YhpCC44BjaNojXQu3hhIhJ+4FHiw12JG/SyhuR+6rrXB5Ui8MCGXH0JC0dihvn2iJz9wA/l48XJRLpdSzuBvAcjMLiI/mObRDpfXbTIU0s+zA8itteVSnBmQAJerqqYNMjlM/cBay6fXpefhwQiclb/nkoaZv7YO6V+Ue3EQufQ8r4Cl48n398cTjaBlxS7J0zRHuRF3ASVAb3W384VeSoSz2e4O/NrIy0jIisOZfeeEKEzeWy4BOk47zVldcujY9q4VqmIa6CAv0LYPwdWJUwCqak0K6Lru9LCr7SFcMJVBK03zIis4nVpWlkocMawIPWcX2YSTySTl3UkZSjwcG14UJkMFLYBA8R1GG75FgEONyy4hHbsOIWZE18rlyRrci4UJgWnzcA3NrcIEVDkUEiYYealDEyRj7FKS31+Ur3zGNysKx7QSouyK+f2rBicmM8uKYzFn5mZXTm8yeLmpKAvy2bV47Vc/Hr3fW5nFTd565D/zDz/CrHERWMUAAAAAAElFTkSuQmCC"
          alt=""></a></div>
    <div class="up">
      <a href="#home">
        <img
          src="data:image/png;base64,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"
          alt="">
      </a>
    </div>
  </footer>
</template>

<script setup>
import { ImgComparisonSlider } from '@img-comparison-slider/vue';

useHead({
  title: '德舜營造 - DESHUN',
  link: [
    {
      rel: 'icon',
      type: 'image/x-icon',
      href: './images/favicon.ico'
    },
  ]
})
const is_nav_active = ref(false)

</script>
