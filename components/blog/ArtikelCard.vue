<template>
  <b-row class="mb_wrap">
    <b-col>
      <div>
        <div class="d-flex pb-3">
          <div class="mr-2">
            <a href="#">
              <img src="@/assets/stisla/img/avatar/avatar-1.png" alt="avatar" width="20" height="20">
            </a>
          </div>
          <div>
            <a href="#">
              <span>Yanuardi</span>
            </a>
          </div>
        </div>
        <div>
          <a href="#">
            <h2 class="main_article_title">This is Whats Happen when i Sleep in the Room?</h2>
          </a>
        </div>
        <div>
          <a href="#">
            <h3 class="prev_articles">Lorem ipsum dolor sit amet consectetur adipisicing elit. Corporis quia ratione ipsam quam maiores, cum veniam autem ducimus delectus rerum? Officia labore dicta accusamus, tempora pariatur maiores ut modi inventore! Lorem ipsum dolor sit amet consectetur adipisicing elit. Hic officia rerum quas deleniti aspernatur, quae accusamus voluptates suscipit, repellendus optio illo delectus sed necessitatibus voluptas, magni architecto tenetur. In, iusto?</h3>
          </a>
        </div>
        <div>
          <span>Oct 12</span>
        </div>
      </div>
    </b-col>
    <b-col md="4">
      <img src="@/assets/stisla/img/news/img01.jpg" alt="" class="w-100">
    </b-col>
  </b-row>
</template>

<style>
  .mb_wrap {
    margin-bottom: 48px;
  }
  .main_article_title {
    max-height: 56px;
    -webkit-line-clamp: 2;
    text-overflow: ellipsis;
    overflow: hidden;
    font-size: 16px;
    line-height: 20px;
    font-weight: 700;
  }
  .prev_articles {
    max-height: 40px;
    -webkit-line-clamp: 2;
    text-overflow: ellipsis;
    overflow: hidden;
    color: rgba(117, 117, 117, 1);
    font-size: 16px;
    line-height: 20px;
    font-weight: 400;
  }
</style>
