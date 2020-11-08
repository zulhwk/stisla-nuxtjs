<template>
  <div>
    <div class="blog_wrapper mt-5">
      <div class="container-small">
        <div class="container_blogs">
          <div>
            <div class="title_content">
              <h1>5 Deeply Disturbing Facts About The Chris Watts Murders</h1>
            </div>
            <div class="d-flex">
              <div class="d-flex" style="align-items: center;">
                <div>
                  <img class="ava_content" src="@/assets/stisla/img/avatar/avatar-1.png" alt="" width="50" height="50">
                </div>
                <div>
                  <div>
                    <span class="author_text_content">Yanuardi</span>
                  </div>
                  <div>
                    <span class="date_text_content">Ockt 10</span>
                  </div>
                </div>
              </div>
            </div>
            <div class="content__">
              <p>
                <img src="@/assets/stisla/img/unsplash/eberhard-grossgasteiger-1207565-unsplash.jpg" alt="">
              </p>
              <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Cupiditate, facilis. Cupiditate accusamus quisquam reiciendis ex non ab. Repudiandae eum error, reiciendis neque, ex saepe distinctio aperiam, minima ab adipisci ipsam. Lorem ipsum, dolor sit amet consectetur adipisicing elit. Porro explicabo assumenda natus vero eligendi beatae mollitia maxime ea nihil ratione id nemo fugiat velit tempore quos, expedita sint facere. Tempore!</p>
              <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Cupiditate, facilis. Cupiditate accusamus quisquam reiciendis ex non ab. Repudiandae eum error, reiciendis neque, ex saepe distinctio aperiam, minima ab adipisci ipsam. Lorem ipsum, dolor sit amet consectetur adipisicing elit. Porro explicabo assumenda natus vero eligendi beatae mollitia maxime ea nihil ratione id nemo fugiat velit tempore quos, expedita sint facere. Tempore!</p>
              <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Cupiditate, facilis. Cupiditate accusamus quisquam reiciendis ex non ab. Repudiandae eum error, reiciendis neque, ex saepe distinctio aperiam, minima ab adipisci ipsam. Lorem ipsum, dolor sit amet consectetur adipisicing elit. Porro explicabo assumenda natus vero eligendi beatae mollitia maxime ea nihil ratione id nemo fugiat velit tempore quos, expedita sint facere. Tempore!</p>
              <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Cupiditate, facilis. Cupiditate accusamus quisquam reiciendis ex non ab. Repudiandae eum error, reiciendis neque, ex saepe distinctio aperiam, minima ab adipisci ipsam. Lorem ipsum, dolor sit amet consectetur adipisicing elit. Porro explicabo assumenda natus vero eligendi beatae mollitia maxime ea nihil ratione id nemo fugiat velit tempore quos, expedita sint facere. Tempore!</p>
              <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Cupiditate, facilis. Cupiditate accusamus quisquam reiciendis ex non ab. Repudiandae eum error, reiciendis neque, ex saepe distinctio aperiam, minima ab adipisci ipsam. Lorem ipsum, dolor sit amet consectetur adipisicing elit. Porro explicabo assumenda natus vero eligendi beatae mollitia maxime ea nihil ratione id nemo fugiat velit tempore quos, expedita sint facere. Tempore!</p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import Footer from '@/layouts/partials/blog/Footer.vue'
export default {
  layout: 'blog',
  components: {
    Footer
  }
}
</script>

<style>
  .ava_content {
    border-radius: 50%;
    margin-right: 20px;
  }
  .author_text_content {
    font-size: 14px;
    font-weight: 400;
    color: black;
  }
  .date_text_content {
    font-size: 14px;
    font-weight: 400;
    color: rgba(117, 117, 117, 1);
  }
  .content__ p {
    letter-spacing: -0.003em;
    margin-top: 2em;
    font-size: 21px;
    line-height: 32px;
    font-weight: 400;
    color: rgba(41, 41, 41, 1);
  }
  .content__ p img {
    width: 100%;
  }
</style>
