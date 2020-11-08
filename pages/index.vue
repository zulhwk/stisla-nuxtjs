<template>
  <div class="container">
    <!-- TRENDING ARTIKEL -->
    <div class="mb-3 mt-5">
      <div class="mb-3">
        <b-row>
          <b-col cols="auto">
            <img src="@/assets/bar-graph.svg" alt="" width="20" height="15">
          </b-col>
          <b-col>
            <span class="trend_text">TRENDING TOPIC</span>
          </b-col>
        </b-row>
      </div>
      <b-row>
        <CardTrending
          title="What Half of America Choosing Trump Again Taught Me"
          author="Yanuardi"
          date="12 Nov"
          number="01"
          image="avatar-1.png"
        />
        <CardTrending
          title="Facebook Shuts Down Massive ‘Stop the Steal’ Group"
          author="Muhammad Azhari"
          date="10 Nov"
          number="02"
          image="avatar-2.png"
        />
        <CardTrending
          title="Donald Trump Won, No Matter What Happens Next"
          author="Muhammad Rian"
          date="09 Okt"
          number="03"
          image="avatar-3.png"
        />
        <CardTrending
          title="Instalation NuxtJS in VueJS"
          author="Yanuardi"
          date="12 Nov"
          number="04"
          image="avatar-4.png"
        />
        <CardTrending
          title="Facebook Shuts Down Massive ‘Stop the Steal’ Group"
          author="Muhammad Azhari"
          date="10 Nov"
          number="05"
          image="avatar-2.png"
        />
        <CardTrending
          title="What Half of America Choosing Trump Again Taught Me"
          author="Yanuardi"
          date="12 Nov"
          number="06"
          image="avatar-1.png"
        />
      </b-row>
    </div>

    <!-- ALL ARTIKEL -->
    <div class="bg_content mt-5">
      <b-row>
        <b-col>
          <div class="content_wrap">
            <AllArticle v-for="i in 20" :key="i" />
          </div>
        </b-col>
        <b-col md="5">
          <div ref="sidebarContent" class="sidebar-right" :class="myStyle">
            <div class="sid_one">
              <p class="title_sidebar">
                DISCOVER MORE OF WHAT MATTERS TO YOU
              </p>
              <Tags name="Relationship" />
              <Tags name="Programming" />
              <Tags name="News" />
              <Tags name="Health" />
              <Tags name="Self" />
              <Tags name="Relationship" />
              <Tags name="Programming" />
              <Tags name="News" />
            </div>
          </div>
        </b-col>
      </b-row>
    </div>
  </div>
</template>

<script>
import CardTrending from '@/components/blog/TrendingCard.vue'
import AllArticle from '@/components/blog/ArtikelCard.vue'
import Tags from '@/components/blog/TagsCard.vue'
export default {
  layout: 'blog',
  components: {
    CardTrending,
    AllArticle,
    Tags
  },
  data () {
    return {
      myStyle: ''
    }
  },
  mounted () {
    window.addEventListener('scroll', this.calculateScrollY)
  },
  methods: {
    calculateScrollY () {
      if (window.scrollY >= 210) {
        this.myStyle = 'fixed-top_one'
      } else {
        this.myStyle = ''
      }
    }
  }
}
</script>

<style>
  .title_sidebar {
    text-transform: uppercase;
    letter-spacing: 0.083em;
    line-height: 16px;
    font-size: 12px;
    font-weight: 700;
  }
  .sid_one {
    border-bottom: 1px solid rgba(230, 230, 230, 1);
    padding-bottom: 24px;
  }
  .trend_text {
    text-transform: uppercase;
    letter-spacing: 0.083em;
    line-height: 16px;
    font-size: 12px;
    font-weight: 700;
    color: rgba(41, 41, 41, 1);
  }
</style>
