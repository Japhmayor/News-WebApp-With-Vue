<template>
  <div class="container">
    <div class="row">
      <div class="col-md-3" v-for="item in list">
        <router-link :to="'/news/'+item.link">
          <div class="card border-dark mb-3 arrange">
            <img class="card-img-top" :src="item.img" alt="item.title">
            <div class="card-body">
                <h4 class="card-title">{{ item.title }}</h4>
            </div>
          </div>
        </router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      list: [
        {
          title: 'ABC News',
          link: 'abc-news-au',
          img: 'http://mobile.abc.net.au/cm/cb/4355924/News+iOS+120x120/data.png'
        },
        {
          title: 'BBC News',
          link: 'bbc-news',
          img: 'http://m.files.bbci.co.uk/modules/bbc-morph-news-waf-page-meta/1.2.0/apple-touch-icon.png'
        },
        {
          title: 'BBC Sport',
          link: 'bbc-sport',
          img: 'http://static.bbci.co.uk/onesport/2.11.204/images/web-icons/bbc-sport-180.png'
        },
        {
          title: 'Buzzfeed',
          link: 'buzzfeed',
          img: 'https://www.buzzfeed.com/static-assets/img/touch-icon-ios_120.208a0e329cd6e8d831b21ae17fb6aabb.png'
        },
        {
          title: 'CNN',
          link: 'cnn',
          img: 'https://i.cdn.cnn.com/cnn/.e/img/3.0/global/misc/apple-touch-icon.png'
        },
        {
          title: 'Daily Mail',
          link: 'daily-mail',
          img: 'http://www.dailymail.co.uk/apple-touch-icon.png'
        },
        {
          title: 'The TOI',
          link: 'the-times-of-india',
          img: 'https://icons.better-idea.org/lettericons/I-120-000000.png'
        },
        {
          title: 'Google News',
          link: 'google-news',
          img: 'https://ssl.gstatic.com/news-static/img/1703439073-news-thumb-128_w.png'
        },
        {
          title: 'ESPN',
          link: 'espn',
          img: 'http://a.espncdn.com/wireless/mw5/r1/images/bookmark-icons/espn_icon-152x152.min.png'
        },
        {
          title: 'Times',
          link: 'times',
          img: 'http://s0.wp.com/wp-content/themes/vip/time2014/img/time-touch_icon_120.png'
        },
        {
          title: 'The Next Web',
          link: 'the-next-web',
          img: 'https://cdn0.tnwcdn.com/wp-content/themes/cyberdelia/assets/icons/apple-touch-icon-120x120.png?v=1502808859'
        },
        {
          title: 'The New York Times',
          link: 'the-new-york-times',
          img: 'https://cdn1.nyt.com/mw-static/images/touch-icon-ipad-144.319373aa.png'
        },
        {
          title: 'The Hindu',
          link: 'the-hindu',
          img: 'https://icons.better-idea.org/lettericons/T-120-ffffff.png'
        },
        {
          title: 'Techradar',
          link: 'techradar',
          img: 'http://cdn0.static.techradar.futurecdn.net/20170811/apple-touch-icon.png'
        },
        {
          title: 'Reddit All',
          link: 'reddit-r-all',
          img: 'https://www.redditstatic.com/mweb2x/favicon/120x120.png'
        },
        {
          title: 'Hacker News',
          link: 'hacker-news',
          img: 'https://news.ycombinator.com/favicon.ico'
        }
      ]
    }
  },
  methods: {
    
  }
}
</script>

<style scoped>
a {
  text-decoration: none;
  color: #000;
}
</style>
