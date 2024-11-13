<script></script>
<template>
  <div class="news">
    <h1>Recent news</h1>
    <div class="news-wrapper">
      <div>
        <img src="/image-news-1.jpg" alt="" />
        <a href="">
          <h2>How to Build Climate Change-Resilient Infrastructure</h2></a
        >
        <span
          >Industry News
          <div class="line"></div>
          June 24, 2020</span
        >
        <p>
          Ipsum aliquet nisi, hendrerit rhoncus quam tortor,
          <br class="br-hide-news" />
          maecenas faucibus. Tincidunt aliquet sit
          <br />
          vel, venenatis nulla. Integer bibendum turpis convallis enim, nibh
          convallis...
        </p>
      </div>
      <div>
        <div>
          <img src="/image-news-2.jpg" alt="" />
          <a href=""><h2>How Construction Can Help Itself</h2></a>
          <span
            >Innovation
            <div class="line"></div>
            June 12, 2020</span
          >
        </div>
        <div>
          <img src="/image-news-3.jpg" alt="" />
          <a href=""><h2>How Construction Can Help Itself</h2></a>
          <span
            >Company News
            <div class="line"></div>
            December 1, 2019</span
          >
        </div>
      </div>
    </div>
    <div class="posts">
      <b>Explore all our news posts </b><button>View all news</button>
    </div>
  </div>
</template>
<style scoped>
.news h1 {
  font-size: 46px;
  font-weight: 700;
  line-height: 59.8px;
  text-align: center;
  margin-top: 120px;
  margin-bottom: 60px;
}
.news button {
  background: #ff5a30;
  width: 212px;
  height: 52px;
  border: none;
  color: #ffffff;
  font-size: 16px;
  font-weight: 700;
  line-height: 52px;
}
.posts {
  margin-top: 80px;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 40px;
  margin-bottom: 120px;
}
.news b {
  color: #1e212c;
  font-size: 28px;
  font-weight: 700;
  line-height: 42px;
}
.line {
  height: 12px;
  background: #787a80;
  width: 0.1px;
}
.news span {
  display: flex;
  gap: 12px;
  align-items: center;
  margin-top: 12px;
  margin-bottom: 16px;
}
.news-wrapper {
  display: flex;
  gap: 30px;
  justify-content: center;
  width: 65%;
  margin: 0 auto;
}
.news-wrapper img {
  width: 100%;
}
.news-wrapper h2 {
  font-size: 20px;
  font-weight: 700;
  line-height: 30px;
  color: #1e212c;
}
.news-wrapper p {
  font-size: 15px;
  font-weight: 400;
  line-height: 25.6px;
}
.br-hide-news {
  display: none;
}
@media (max-width: 1000px) {
  .news-wrapper {
    flex-direction: column;
  }
}
@media (max-width: 900px) {
  .news-wrapper p {
    font-size: 12px;
    font-weight: 400;
    line-height: 20px;
  }
}
@media (max-width: 750px) {
  .news-wrapper h2 {
    font-size: 16px;
    line-height: 22px;
  }
  .br-hide-news {
    display: block;
  }
}
@media (max-width: 600px) {
  .posts {
    flex-direction: column;
    gap: 10px;
  }
  .news-wrapper p {
    font-size: 10px;
    line-height: 16px;
  }
  .news-wrapper h2 {
    font-size: 14px;
    line-height: 20px;
  }
}
@media (max-width: 500px) {
  .news-wrapper h2 {
    font-size: 10px;
    line-height: 18px;
  }
  .news span {
    font-size: 10px;
  }
  .br-hide-news {
    display: none;
  }
  .news b {
    font-size: 20px;
    line-height: 36px;
  }
  .news button {
    width: 152px;
    font-size: 14px;
    line-height: 46px;
  }
}
</style>
