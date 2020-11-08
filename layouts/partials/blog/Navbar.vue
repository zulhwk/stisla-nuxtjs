<template>
  <div>
    <div class="jgz">
      <div class="container">
        <div class="d-flex justify-content-between" style="padding:25px 0;">
          <div>
            <a href="#">
              <h2>Zulhwk</h2>
            </a>
          </div>
          <div>
            <a href="#">
              <b-button variant="outline-dark">
                TULIS ARTIKEL
              </b-button>
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<style>
 .jgz {
   border-bottom: 1px solid rgba(41, 41, 41, 1);
 }
 .large_jumbotron_text {
   font-size: 70px;
   line-height: 74px;
   color: rgba(8, 8, 8, 1);
 }
 .small_jumbotron_text {
   line-height: 24px;
   font-size: 18px;
   font-weight: 400;
 }
 .wrap_jumbotron {
   padding-top: 33px;
   padding-bottom: 51px;
 }
 .mb {
   flex: 1;
 }
</style>
