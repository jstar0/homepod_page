<template>
  <div id="about">
    <div class="item" id="readme" @click="go(profile.README.link)">
      <div class="item-content text-wrapper">
        <h3>关于我</h3>
        <p>
          {{ profile.README.content }}
        </p>
      </div>
    </div>
    <div class="item" id="meta">
      <div class="sub-item" :style="'color:#fff; background: '+profile.characteristic[0].color">
        <h3>
          <i :class="'fa '+profile.characteristic[0].icon" aria-hidden="true"
             style="margin-right: 5px;"></i>{{ profile.characteristic[0].title }}
          <br/>一个很酷的MC服务器项目
        </h3>
      </div>
      <div class="sub-item" :style="'color:#fff; background: '+profile.characteristic[1].color">
        <h3>
          <i :class="'fa '+profile.characteristic[1].icon" aria-hidden="true"
             style="margin-right: 5px;"></i>{{ profile.characteristic[1].title }}
          <br/>不忘初心，砥砺前行
        </h3>
      </div>
      <div class="sub-item" :style="'color:#fff; background: '+profile.characteristic[2].color">
        <h3>
          <i :class="'fa '+profile.characteristic[2].icon" aria-hidden="true"
             style="margin-right: 5px;"></i>{{ profile.characteristic[2].title }}
          <br/>内心要只有一个声音
        </h3>
      </div>
    </div>
    <div class="item" id="video">
      <video loop="true" muted="true" autoplay="true" :src="profile.video"
             :poster="profile.img" style="height: 240px;"></video>
    </div>
    <div class="item" id="links">
      <div class="sub-item" @click="go(profile.links[0].url)" :id="profile.links[0].title"
           :style="'background: '+profile.links[0].color">
        <div>
            <svg version="1.1" id="Capa_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
               viewBox="0 0 279.199 279.199" style="enable-background:new 0 0 279.199 279.199;" xml:space="preserve">
            <path style="fill:#ffffff;" d="M275.639,64.92c-0.01-0.077-0.023-0.153-0.035-0.229c-0.045-0.283-0.104-0.561-0.18-0.833
              c-0.011-0.042-0.02-0.083-0.032-0.125c-0.094-0.314-0.208-0.62-0.341-0.916c-0.022-0.05-0.048-0.098-0.071-0.148
              c-0.121-0.256-0.256-0.504-0.404-0.743c-0.029-0.048-0.057-0.097-0.087-0.144c-0.173-0.266-0.362-0.52-0.567-0.761
              c-0.04-0.047-0.083-0.091-0.125-0.138c-0.18-0.201-0.37-0.392-0.57-0.573c-0.051-0.046-0.1-0.094-0.152-0.138
              c-0.243-0.208-0.499-0.401-0.767-0.577c-0.042-0.027-0.085-0.051-0.127-0.077c-0.255-0.16-0.52-0.304-0.794-0.433
              c-0.028-0.013-0.053-0.031-0.081-0.044L142.699,0.671c-1.969-0.895-4.23-0.895-6.199,0L47.638,41.004
              c-3.772,1.712-5.441,6.157-3.729,9.929c1.711,3.772,6.158,5.446,9.929,3.729L139.6,15.736l110.217,50.025L139.6,114.198
              L14.011,59.006c-0.009-0.004-0.018-0.006-0.027-0.01c-0.184-0.08-0.374-0.149-0.565-0.215c-0.048-0.017-0.096-0.037-0.144-0.053
              c-0.157-0.05-0.319-0.089-0.48-0.129c-0.085-0.021-0.17-0.047-0.256-0.065c-0.103-0.022-0.209-0.034-0.314-0.052
              c-0.146-0.024-0.292-0.051-0.438-0.067c-0.068-0.007-0.139-0.008-0.208-0.013c-0.183-0.014-0.365-0.026-0.547-0.027
              c-0.013,0-0.025-0.002-0.038-0.002c-0.071,0-0.14,0.009-0.21,0.011c-0.162,0.004-0.324,0.009-0.484,0.024
              c-0.125,0.011-0.247,0.031-0.37,0.049c-0.113,0.017-0.227,0.03-0.338,0.052c-0.153,0.029-0.302,0.067-0.452,0.104
              c-0.081,0.021-0.162,0.039-0.242,0.063c-0.162,0.047-0.32,0.103-0.477,0.16c-0.068,0.024-0.136,0.047-0.203,0.074
              c-0.155,0.062-0.306,0.131-0.456,0.203c-0.069,0.034-0.14,0.065-0.208,0.101c-0.136,0.07-0.269,0.147-0.4,0.226
              c-0.081,0.048-0.162,0.095-0.24,0.146c-0.113,0.073-0.222,0.152-0.331,0.231c-0.091,0.066-0.182,0.132-0.27,0.202
              c-0.092,0.074-0.181,0.152-0.269,0.23c-0.096,0.084-0.191,0.167-0.282,0.256c-0.079,0.077-0.154,0.159-0.229,0.239
              c-0.09,0.096-0.18,0.191-0.266,0.292c-0.076,0.09-0.147,0.186-0.22,0.28c-0.074,0.096-0.148,0.19-0.218,0.291
              c-0.083,0.12-0.158,0.245-0.234,0.37c-0.049,0.081-0.101,0.16-0.148,0.243c-0.09,0.162-0.17,0.329-0.249,0.497
              c-0.022,0.048-0.049,0.091-0.07,0.14c-0.004,0.009-0.006,0.019-0.01,0.027c-0.08,0.184-0.149,0.373-0.214,0.563
              c-0.017,0.049-0.038,0.097-0.054,0.146c-0.049,0.155-0.088,0.315-0.127,0.474c-0.022,0.088-0.049,0.175-0.068,0.264
              c-0.021,0.098-0.032,0.198-0.049,0.297c-0.026,0.152-0.054,0.304-0.07,0.457c-0.006,0.06-0.006,0.12-0.011,0.18
              c-0.016,0.192-0.028,0.385-0.029,0.577c0,0.011-0.001,0.021-0.001,0.033v146.427c0,2.925,1.7,5.583,4.355,6.809l128.606,59.398
              c0,0,0.018,0.006,0.026,0.011c0.055,0.024,0.111,0.042,0.166,0.065c0.25,0.107,0.501,0.201,0.756,0.279
              c0.089,0.027,0.179,0.05,0.27,0.074c0.243,0.065,0.486,0.117,0.73,0.157c0.075,0.012,0.15,0.027,0.226,0.037
              c0.322,0.042,0.645,0.07,0.966,0.07c0.032,0,0.063-0.006,0.095-0.007c0.283-0.003,0.566-0.024,0.848-0.06
              c0.104-0.013,0.206-0.033,0.308-0.05c0.219-0.037,0.437-0.083,0.653-0.14c0.101-0.026,0.2-0.052,0.299-0.083
              c0.239-0.073,0.473-0.16,0.706-0.258c0.065-0.027,0.131-0.049,0.195-0.078c0.015-0.007,0.031-0.011,0.045-0.018l128.606-59.398
              c2.655-1.226,4.355-3.884,4.355-6.809V65.872C275.706,65.549,275.679,65.232,275.639,64.92z M147.1,259.972V159.266
              c0-4.143-3.357-7.5-7.5-7.5s-7.5,3.357-7.5,7.5v100.707l-113.606-52.47V77.36l118.089,51.896c0.962,0.423,1.989,0.634,3.018,0.634
              s2.056-0.211,3.018-0.634L260.706,77.36v130.142L147.1,259.972z"/>
            </svg>
          <h3>{{ profile.links[0].title }}</h3>
        </div>
      </div>
      <div class="sub-item" @click="go(profile.links[1].url)" :id="profile.links[1].title"
           :style="'background: '+profile.links[1].color">
        <div>
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 512"><path fill="#ffffff" d="M537.6 226.6c4.1-10.7 6.4-22.4 6.4-34.6 0-53-43-96-96-96-19.7 0-38.1 6-53.3 16.2C367 64.2 315.3 32 256 32c-88.4 0-160 71.6-160 160 0 2.7.1 5.4.2 8.1C40.2 219.8 0 273.2 0 336c0 79.5 64.5 144 144 144h368c70.7 0 128-57.3 128-128 0-61.9-44-113.6-102.4-125.4z"/></svg>
          <h3>{{ profile.links[1].title }}</h3>
        </div>
      </div>
      <div class="sub-item" @click="go(profile.links[2].url)" :id="profile.links[2].title"
           :style="'background: '+profile.links[2].color">
        <div>
            <svg version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" viewBox="0 0 1000 1000" enable-background="new 0 0 1000 1000" xml:space="preserve">
                <path fill="#ffffff" d="M882.6,575.2c-10.2-24.7-22.5-47.1-35.9-67.1c0.7-0.4,1.4-0.8,2-1.1c7.9-6.2-0.7-33-9-57.8c-7.9-22.8-25.4-45.5-26-44.8c-1.6,1.4-3.5,2.8-5.3,4.5c8.3-28,12.9-57.2,12.9-87.8C821.4,149.5,681,10,508.1,10C335,10,194.9,149.5,194.9,321c0,21.2,2.1,41.9,6.2,62c-1.6-1.6-3.4-3.3-5-4.6c-5.3,0-15.1,29.7-19.4,53.8c-6.1,34.6-10,49.1-10,49.1s-0.7,6.6,1.7,8.5c0.2,0.2,0.5,0.4,0.8,0.7c-15.4,18.9-30.2,40.9-42.6,65.7C82.2,644.9,88.9,734.4,116.1,749c14,7.5,50.7-16.6,86.7-60.3c5.6,49.9,28.6,95.7,64,132.8c-59.7,18.5-99,53.4-93.8,89.4c0.3,2.7,1.9,5.3,2.8,7.9c0.2,0.4-0.1,0.8-0.1,1.3c6.9,45.6,84.7,75.4,173.9,65.7c68.4-7.5,123.4-35.7,142.4-69.1c3.9,0.2,7.7,0.5,11.5,0.5c6.5,0,12.9-0.5,19.4-0.9c19.1,33.8,72.6,62.8,138.8,71.2c86.6,11.1,161.5-17.3,167.4-63.2c0-0.1,0-0.2,0-0.5c1.3-3.5,2.9-6.9,3.4-10.7c4.6-35.8-34.5-71.6-93-90.9c34.1-35.7,56.9-79.2,63.6-127c32.1,43.8,64.7,72.2,81.9,68.6C905.2,759.5,919.6,665.4,882.6,575.2z"/>
            </svg>
          <h3>{{ profile.links[2].title }}</h3>
        </div>
      </div>
      <div class="sub-item" @click="go(profile.links[3].url)" :id="profile.links[3].title"
           :style="'background: '+profile.links[3].color">
        <div>
            <svg version="1.0" xmlns="http://www.w3.org/2000/svg"
             width="980.000000pt" height="966.000000pt" viewBox="0 0 980.000000 966.000000"
             preserveAspectRatio="xMidYMid meet">

            <g transform="translate(0.000000,966.000000) scale(0.100000,-0.100000)"
            fill="#ffffff" stroke="none">
            <path d="M3565 9636 c-81 -37 -101 -89 -175 -451 -230 -1128 -420 -1644 -743
            -2015 -335 -385 -894 -631 -1932 -850 -486 -102 -611 -132 -635 -149 -32 -23
            -70 -97 -77 -150 -8 -62 14 -127 55 -161 50 -41 155 -71 502 -144 516 -109
            671 -146 933 -226 637 -191 1023 -443 1287 -836 252 -377 395 -809 615 -1854
            68 -324 92 -390 157 -429 48 -30 100 -35 158 -16 57 19 104 54 124 94 16 29
            46 160 106 456 268 1318 537 1874 1078 2232 355 234 869 404 1772 588 96 19
            233 49 303 66 112 27 133 35 162 65 80 80 70 231 -21 300 -47 36 -111 54 -404
            114 -1212 247 -1729 454 -2106 841 -359 370 -563 904 -808 2112 -60 299 -77
            344 -144 392 -36 24 -54 30 -110 32 -42 2 -78 -2 -97 -11z m184 -1543 c156
            -507 295 -806 506 -1089 137 -183 396 -415 606 -542 261 -157 491 -250 1012
            -407 86 -26 157 -52 157 -56 0 -5 -19 -13 -42 -19 -188 -47 -648 -206 -842
            -292 -320 -141 -614 -354 -815 -592 -272 -322 -480 -779 -661 -1456 l-12 -45
            -54 185 c-203 690 -409 1096 -719 1418 -174 182 -336 298 -590 425 -257 128
            -651 275 -932 348 -51 13 -93 26 -93 29 0 3 55 20 123 39 426 119 827 282
            1080 439 351 216 628 524 820 908 102 203 206 479 287 755 55 191 65 219 78
            219 5 0 46 -120 91 -267z"/>
            <path d="M7335 4796 c-45 -20 -123 -103 -138 -150 -8 -22 -31 -129 -52 -236
            -86 -444 -199 -816 -303 -1000 -146 -255 -328 -408 -632 -529 -165 -66 -335
            -115 -680 -195 -420 -98 -457 -111 -507 -185 -44 -66 -17 -205 51 -258 27 -22
            157 -56 431 -113 440 -93 776 -207 982 -336 98 -61 217 -174 276 -262 148
            -222 245 -498 357 -1017 71 -332 92 -404 125 -444 58 -68 188 -81 268 -25 65
            45 89 107 137 344 53 266 109 486 175 686 210 640 498 846 1475 1054 259 55
            376 86 416 111 41 25 84 109 84 164 0 57 -43 140 -89 170 -25 17 -94 37 -221
            65 -544 119 -710 164 -909 242 -318 127 -531 322 -665 610 -103 220 -166 445
            -287 1032 -21 99 -41 171 -54 190 -25 37 -135 96 -178 96 -18 -1 -45 -7 -62
            -14z m160 -1396 c47 -111 115 -241 169 -325 178 -274 449 -471 850 -621 97
            -36 124 -50 110 -55 -10 -5 -89 -36 -175 -69 -264 -103 -440 -213 -603 -375
            -156 -154 -287 -365 -380 -612 -44 -115 -66 -158 -75 -147 -4 5 -27 59 -50
            119 -217 557 -467 808 -1029 1030 -67 27 -121 53 -119 58 1 5 79 42 172 82
            285 122 385 186 564 360 191 186 290 339 400 620 29 72 56 141 62 155 10 23
            13 19 43 -65 18 -49 45 -119 61 -155z"/>
            </g>
            </svg>
          <h3>{{ profile.links[3].title }}</h3>
        </div>
      </div>
    </div>
    <div class="item" id="recent" @click="showPopup">
      <div class="item-content">
        <h3>
          心纪元近期博文<br/>
          <span>Recent Posts</span>
        </h3>
      </div>
    </div>
    <div class="item" id="skills">
      <div class="item-content">
        <h3>技术力</h3>
        <li v-for="item in profile.skill" :key="item.title"><i :class="'fa '+ item.icon" aria-hidden="true"></i>
          {{ item.title }} <span class="right">{{ item.percent }}%</span></li>
      </div>
    </div>
    <div class="item" @click="go(profile.github[1])" id="github-status"
         :style="'background-image: url('+profile.github[0]+');'"></div>

    <router-link to="/" class="back">
      <svg t="1628300153041" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg"
           p-id="1988" width="200" height="200">
        <path
            d="M932.04 483.875H163.745l350.591-311.627c11.009-9.785 12-26.643 2.216-37.652-9.787-11.005-26.64-11.999-37.653-2.214L74.242 492.065a26.672 26.672 0 0 0 0 39.868L478.9 891.618a26.567 26.567 0 0 0 17.708 6.735c7.353 0 14.676-3.022 19.945-8.95 9.785-11.01 8.793-27.866-2.216-37.653L160.473 537.214H932.04c14.729 0 26.669-11.94 26.669-26.67 0-14.729-11.94-26.669-26.67-26.669z"
            p-id="1989"></path>
      </svg>
    </router-link>
    <router-link to="/system" class="next">
      <svg t="1628300153041" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg"
           p-id="1988" width="200" height="200">
        <path
            d="M932.04 483.875H163.745l350.591-311.627c11.009-9.785 12-26.643 2.216-37.652-9.787-11.005-26.64-11.999-37.653-2.214L74.242 492.065a26.672 26.672 0 0 0 0 39.868L478.9 891.618a26.567 26.567 0 0 0 17.708 6.735c7.353 0 14.676-3.022 19.945-8.95 9.785-11.01 8.793-27.866-2.216-37.653L160.473 537.214H932.04c14.729 0 26.669-11.94 26.669-26.67 0-14.729-11.94-26.669-26.67-26.669z"
            p-id="1989"></path>
      </svg>
    </router-link>
    <van-popup
        v-model:show="show"
        round>
      <div id="recent-posts">
        <h3 class="recent-posts-title">已有博文</h3>
        <div class="article-item" v-for="article in posts" v-bind:key="article">
          <a :href="article.link" target="_blank"><h3>{{ article.title }}</h3></a>
        </div>
        <h5>{{ msg }}</h5>
      </div>
    </van-popup>
  </div>
</template>

<script>
export default {
  name: "about",
  data() {
    return {
      show: false,
      gotPosts: false,
      msg: 'loading',
      posts: [],
      profile: {}
    }
  },
  methods: {
    go(url) {
      console.log(url);
      window.open(url);
    },
    showPopup() {
      this.show = true;
      if (this.gotPosts === false) {
        this.getArticles()
        this.gotPosts = true
      }
    },
    getArticles() {
      let that = this;
      that.posts = that.$store.state.articles;
      if (that.posts === undefined || that.posts.length === 0) {
        console.log('yo');
        that.$http.get(this.$store.state.api + '/X/getBlogRSS?url=https://www.mcxin.top/feed&type=force').then((response) => {
          that.posts = response.data
          that.$store.commit('storeArts', response.data);
          that.msg = '到此为止'
        })
      }
    }
  },
  created() {
    if (Object.keys(this.$store.state.OriginData).length !== 0) {
      this.profile = this.$store.state.OriginData.about;
    } else {
      console.log('jump');
      window.location = '/';
    }
  }
}
</script>

<!--suppress CssInvalidFunction -->
<style scoped>
a:link, a:visited {
  color: unset;
  text-decoration: none;
}

.back, .next {
  position: fixed;
  top: 50px;
}

.back svg, .next svg {
  width: 40px;
  height: 40px;
}

.back {
  left: 50px;
}

.next {
  transform: rotate(180deg);
  right: 50px;
}

#readme, #telegram, #github-status, #bili, #blog, #country, #language, #animate, #video, #sztu, #recent, #skills, .sub-item {
  cursor: pointer;
}

#readme:hover, #telegram:hover, #github-status:hover, #bili:hover, #blog:hover, #country:hover, #language:hover, #animate:hover, #video:hover, #sztu:hover, #recent:hover, #skills:hover, .sub-item:hover {
  transform: scale(0.99);
}

#about {
  display: flex;
  width: 100%;
  height: 100%;
  justify-content: space-around;
  align-items: center;
  flex-wrap: wrap;
  position: relative;
}

.item {
  height: 240px;
  width: 240px;
  margin: 1px;
  border-radius: 20px;
  box-shadow: -5px -5px 10px rgb(32 32 32 / 10%), 5px 5px 10px rgb(32 32 32 / 10%);
  -webkit-transition: .4s ease all;
  -moz-transition: .4s ease all;
  -o-transition: .4s ease all;
  transition: .4s ease all;
}

.item-content {
  margin: 20px;
}

.sub-item {
  height: 70px;
  width: 240px;
  margin: 0;
  border-radius: 20px;
  box-shadow: -5px -5px 10px rgb(32 32 32 / 10%), 5px 5px 10px rgb(32 32 32 / 10%);
  -webkit-transition: .4s ease all;
  -moz-transition: .4s ease all;
  -o-transition: .4s ease all;
  transition: .4s ease all;
}

#readme {
  display: flex;
  justify-content: center;
  align-items: center;
  color: #fff;
  background: #06beb6; /* fallback for old browsers */
  background: -webkit-linear-gradient(to left, #48b1bf, #06beb6); /* Chrome 10-25, Safari 5.1-6 */
  background: linear-gradient(to left, #48b1bf, #06beb6); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
}

#readme h3 {
  font-size: 22px;
  text-align: center;
  font-weight: 400;
  margin: 0 0 10px;
}

#readme p {
  font-size: 18px;
  line-height: 1.7;
  margin: 0;
}

#meta {
  display: flex;
  justify-content: space-evenly;
  align-content: space-between;
  flex-wrap: wrap;
  text-align: center;
  box-shadow: none;
}

#meta .sub-item {
  display: flex;
  justify-content: space-evenly;
  align-content: space-between;
  align-items: flex-start;
  overflow: hidden;
  line-height: 70px;
  -webkit-transition: .2s ease all;
  -moz-transition: .2s ease all;
  -o-transition: .2s ease all;
  transition: .2s ease all;
}

#meta .sub-item:hover {
  line-height: 35px;
}

#meta .sub-item h3 {
  margin: 0;
  font-weight: 400;
}

#meta #country {
  background: #dd001b;
  color: #fff;
}

#meta #language {
  background: RGB(100, 147, 175);
  color: #fff;
}

#meta #animate {
  background: RGB(197, 105, 120);
  color: #fff;
}

#video {
  overflow: hidden;
}

#github-status {
  position: relative;
  width: 560px;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  background-repeat: no-repeat;
  background-size: cover;
  -webkit-background-size: cover;
  -o-background-size: cover;
}

#links {
  display: flex;
  justify-content: space-evenly;
  align-content: space-between;
  flex-wrap: wrap;
  text-align: center;
  box-shadow: none;
}

#links .sub-item {
  width: 100px;
  height: 115px;
  display: flex;
  justify-content: center;
  align-items: center;
  cursor: pointer;
}

#links .sub-item div svg {
  height: 35px;
  width: 35px;
}

#links .sub-item div h3 {
  font-family: 'Poppins', 'Noto Sans SC', sans-serif, 微软雅黑, Georgia, serif;
  margin: 8px 0 0;
  font-weight: 400;
  color: #fff;
  font-size: 14px;
}

#recent {
  display: flex;
  justify-content: center;
  align-items: center;
  color: #fff;
  background: RGB(37, 120, 181);
}

#recent h3 {
  font-size: 22px;
  text-align: center;
  font-weight: 400;
  margin: 0 0 10px;
  line-height: 1.4;
}

#recent-posts {
  height: 400px;
  width: 300px;
  padding: 40px;
  overflow: auto;
  scrollbar-width: none; /* Firefox */
}

#recent-posts::-webkit-scrollbar {
  display: none; /* Chrome Safari */
}

.recent-posts-title {
  font-size: 20px;
  margin-top: 0;
  font-weight: 400;
  color: #999;
  text-align: center;
  margin-bottom: 40px;
}

.article-item h3 {
  font-weight: 400;
  -webkit-transition: .2s ease all;
  -moz-transition: .2s ease all;
  -o-transition: .2s ease all;
  transition: .2s ease all;
}

.article-item h3:hover {
  transform: translateX(5px);
}

#recent-posts h5 {
  font-size: 20px;
  font-weight: 400;
  color: #999;
  text-align: center;
  margin-top: 50px;
}

#skills {
  display: flex;
  align-items: center;
  color: #fff;
  background: #6190E8; /* fallback for old browsers */
  background: -webkit-linear-gradient(to right, #A7BFE8, #6190E8); /* Chrome 10-25, Safari 5.1-6 */
  background: linear-gradient(to right, #A7BFE8, #6190E8); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
}

#skills h3 {
  font-size: 22px;
  text-align: center;
  font-weight: 400;
  margin: 0 0 10px;
  line-height: 1.4;
}

#skills li {
  list-style-type: none;
  font-size: 18px;
  line-height: 1.7;
  width: 200px;
}
</style>
