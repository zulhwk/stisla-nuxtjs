<template>
  <b-col md="4">
    <div class="d-flex mb-4">
      <div class="left_placement">
        <span class="text_trending">{{ number }}</span>
      </div>
      <div>
        <div class="d-flex mb-2">
          <div class="d-flex align-items-center">
            <a href="#">
              <img class="b-50" :src="require(`~/assets/stisla/img/avatar/${image}`)" alt="" width="20" height="20">
            </a>
          </div>
          <div class="ml-2 d-flex align-items-center">
            <a href="">
              <span class="f-sm">{{ author }}</span>
            </a>
          </div>
        </div>
        <div>
          <a href="#">
            <h4 class="f_title">{{ title }}</h4>
          </a>
        </div>
        <div>
          <span class="t_sm">{{ date }}</span>
        </div>
      </div>
    </div>
  </b-col>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: 'Title'
    },
    author: {
      type: String,
      default: 'Author'
    },
    date: {
      type: String,
      default: Date.now
    },
    number: {
      type: String,
      default: '01'
    },
    image: {
      type: String,
      default: 'avatar-1.png'
    }
  }
}
</script>

<style>
.left_placement {
  width: 40px;
  margin-right: 16px;
}
.text_trending {
  font-weight: bold;
  color: rgba(230, 230, 230, 1);
  letter-spacing: 0;
  line-height: 36px;
  font-size: 30px;
}
.b-50 {
  border-radius: 50%;
}

.f-sm {
  font-size: 13px;
}
.f_title {
  font-weight: bold;
  line-height: 20px;
  font-size: 16px;
  color: rgba(41, 41, 41, 1);
}
.t_sm {
  font-size: 13px;
  color: rgba(117, 117, 117, 1);
}
</style>
