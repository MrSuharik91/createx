<template>
  <div class="bureau">
    <h1>We are Createx Construction Bureau</h1>
    <h2>
      We are rightfully considered to be the best construction company in the
      USA.
    </h2>
    <img src="/indian-work.png" alt="" />
  </div>
</template>
<style>
.bureau {
  margin-top: 120px;
  text-align: center;
}
.bureau img {
  width: 65%;
  margin-top: 60px;
}
.bureau h1 {
  font-size: 46px;
  font-weight: 700;
  line-height: 59.8px;
  margin-bottom: 25px;
}
.bureau h2 {
  font-size: 18px;
  font-weight: 400;
  line-height: 27px;
  color: #787a80;
}

@media (max-width: 700px) {
  .bureau img {
    width: 75%;
  }
}

@media (max-width: 700px) {
  .bureau h1 {
    font-size: 40px;
    line-height: 52px;
  }
  .bureau h2 {
    font-size: 16px;
  }
}

@media (max-width: 500px) {
  .bureau img {
    width: 85%;
  }
  .bureau h1 {
    font-size: 34px;
  }
  .bureau {
    margin-top: 80px;
    text-align: center;
  }
}

@media (max-width: 400px) {
  .bureau h1 {
    font-size: 32px;
    line-height: 42px;
  }
  .bureau img {
    width: 95%;
  }
}
</style>
