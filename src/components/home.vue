<template>
  <div id="home-container">
    <div id="home-l">
      <div>
        <img id="avatar" v-bind:src="UserMeta.avatar" :alt="UserMeta.username">
      </div>
    </div>
    <div id="home-r">
      <div>
        <h3><span @click="hi(1)" @mouseover="hi(0)" class="animate__animated animate__wobble">{{ emoji }}</span> 您好,
          我是{{ UserMeta.username }}</h3>
        <div class="text-wrapper"><p>{{ UserMeta.detail }}</p></div>
        <button id="more" @click="more">More</button>
      </div>
    </div>

    <div id="footer" v-html="UserMeta.footer"></div>
  </div>
</template>

<script>
export default {
  name: "home",
  data() {
    return {
      UserMeta: {
        avatar: 'https://sdn.geekzu.org/avatar/d42da1c33b856e2314219d0439dcdcde?s=200',
        username: '景星',
        detail: '网络加载较慢，正您展示静态版。\n⭐ 胸有大海星辰，不负青春 ⭐\n🏔 鹰隼试翼，风尘翕张 🌄\n欢迎来到景星的个人主页。',
        footer: ''
      },
      emoji: '✨'
    }
  },
  methods: {
    hi(method = 0) {
      if (method === 0)
        this.emoji = '🎇';
      else
        this.emoji = '✨';
    },
    more() {
      this.$router.push({path: 'about'});
    }
  },
  created() {
    this.$http.get(this.$store.state.api + '/X/getProfileDataMobile').then((response) => {
      this.$store.commit('updateSystemData', response.data);
      this.UserMeta = response.data.home;
    });
  }
}
</script>

<style scoped>
#wrap-content {
  position: relative;
  width: 1200px;
  height: 600px;
  border-radius: 15px;
  align-items: center;
  justify-content: center;
  text-align: center;
}

#home-container {
  display: flex;
  height: 100%;
  width: 100%;
  align-items: center;
  justify-content: center;
}

#home-l {
  height: 500px;
  margin: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
}

#avatar {
  border-radius: 10000rem;
  height: 200px;
  width: 200px;
}

#home-r {
  height: 500px;
  margin: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
}

#home-r h3 {
  font-weight: lighter;
  font-size: 2.5rem;
  margin: 10px 0 0;
}

#home-r h3 span {
  display: inline-block;
  animation-iteration-count: infinite;
  animation-duration: 2s;
  cursor: pointer;
}

#home-r p {
  font-size: 18px;
  line-height: 1.77;
}

#more {
  font-family: 'Noto Sans SC', sans-serif, Georgia, serif;
  background: rgba(0, 0, 0, 0);
  color: rgba(0, 119, 255, 0.8);
  padding: 6px 21px;
  border-radius: 10px;
  border: 2px solid #07f;
  font-weight: lighter;
  cursor: pointer;
  -webkit-transition: .2s ease all;
  -moz-transition: .2s ease all;
  -o-transition: .2s ease all;
  transition: .2s ease all;
}

#more:hover {
  background: rgba(0, 119, 255, 1);
  color: #fff;
}

#footer {
  position: fixed;
  bottom: 0;
  color: #86868b;
  line-height: 1.7;
  text-align: center;
  opacity: 0.5;
}

#footer >>> a,#footer a:link,#footer a:visited, a:-webkit-any-link{
  color: #86868b!important;
  text-decoration: none;
}

@media screen and (max-width: 768px) {
  #home-container {
    height: auto;
    width: auto;
    flex-direction: column;
  }
  #home-l, #home-r {
    height: auto;
  }
  #home-r {
    margin-top:0px;
  }

  #home-r h3{
    font-weight: normal;
    font-size: 1.5rem;
    margin: 10px 0 0;
  }
  #more {
    display: none;
  }

  #footer {
    position: relative;
  }
}
</style>
