<script></script>
<template>
  <div class="partners">
    <h1>Supported by 12+ partners</h1>
    <div class="partners-img">
      <div>
        <img src="/client-logo.png" alt="" />
      </div>
      <div>
        <img src="/client-logo-2.png" alt="" />
      </div>
      <div>
        <img src="/client-logo-3.png" alt="" />
      </div>
      <div>
        <img src="/client-logo-4.png" alt="" />
      </div>
      <div>
        <img src="/client-logo-5.png" alt="" />
      </div>
      <div>
        <img src="/client-logo-6.png" alt="" />
      </div>
    </div>
    <div class="clients">
      <div class="clients-indian">
        <h2>What our clients are saying</h2>
        <img src="/profile-image.svg" alt="" />
        <p>
          Ipsum aute sunt aliquip aute et
          <br class="br-hide-partners" />
          occaecat. Anim minim do cillum eiusmod enim.
          <br />
          Consectetur magna cillum

          <br class="br-hide-partners" />
          consequat minim laboris cillum

          <br class="br-hide-partners" />
          laboris voluptate minim
          <br />
          proident exercitation ullamco.
        </p>
        <span>
          <b>Shawn Edwards</b>
          <br />
          <p>Position, Company name</p>
        </span>
      </div>
      <img class="builder" src="/builder.jpg" alt="" />
    </div>
  </div>
</template>
<style>
.partners {
  background: #f4f5f6;
  width: 100%;
  padding-top: 60px;
}
.partners h1 {
  font-size: 46px;
  font-weight: 700;
  line-height: 59.8px;
  text-align: center;
  margin-bottom: 60px;
}
.partners-img {
  display: flex;
  width: 65%;
  margin: 0 auto;
  justify-content: space-between;
}
.partners-img div {
  text-align: center;
}
.partners h2 {
  font-size: 46px;
  font-weight: 700;
  line-height: 59.8px;
  margin-top: 170px;
}
.clients {
  width: 65%;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.clients p {
  color: #424551;
  font-size: 16px;
  font-weight: 400;
  line-height: 25.6px;
  margin-bottom: 25px;
}
.clients-indian img {
  margin-top: 60px;
  margin-bottom: 25px;
}
.builder {
  width: 40%;
  height: 350px;
  margin-top: 170px;
}
.br-hide-partners {
  display: none;
}
@media (max-width: 1000px) {
  .partners-img {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
  }
  .clients p {
    font-size: 14px;
    line-height: 20px;
  }
  .partners h2 {
    font-size: 40px;
    line-height: 50px;
  }
  .br-hide-partners {
    display: block;
  }
}
@media (max-width: 700px) {
  .clients {
    flex-direction: column;
    text-align: center;
  }
  .builder {
    margin-top: 30px;
    height: 300px;
    margin-bottom: 30px;
  }
}
@media (max-width: 600px) {
  .partners h1 {
    font-size: 40px;
    line-height: 50px;
  }
  .builder {
    height: 250px;
    width: 70%;
  }
}
@media (max-width: 500px) {
  .partners h1 {
    font-size: 34px;
    line-height: 44px;
  }
  .partners-img {
    display: grid;
    grid-template-columns: 1fr 1fr;
    width: 85%;
  }
}
@media (max-width: 300px) {
  .partners h1 {
    font-size: 30px;
    line-height: 40px;
  }
  .partners-img {
    display: grid;
    grid-template-columns: 1fr;
  }
  .partners h1 {
    font-size: 26px;
    line-height: 40px;
  }
  .partners h2 {
    font-size: 26px;
    line-height: 36px;
  }
  .clients p {
    font-size: 11px;
    line-height: 18px;
  }
  .builder {
    width: 90%;
    height: 200px;
  }
}
</style>
