<template>
  <div class="values">
    <h1>Our core values</h1>
    <h3>
      Our mission is to set the highest standards for construction sphere.
    </h3>
    <div class="values-grid">
      <div>
        <img src="/like.svg" alt="" />
        <h2>Quality</h2>
        <p>
          Culpa nostrud commodo ea consequat
          <br />
          aliquip reprehenderit. Veniam velit
          <br />
          nostrud aliquip sunt.
        </p>
      </div>
      <div class="safety">
        <img src="/safety.svg" alt="" />

        <h2>Safety</h2>
        <p>
          Anim reprehenderit sint voluptate
          <br />
          exercitation adipisicing laborum
          <br />
          adipisicing. Minim empor est ea.
        </p>
      </div>
      <div>
        <img src="/comfort.svg" alt="" />

        <h2>Comfort</h2>
        <p>
          Sit veniam aute dolore adipisicing nulla
          <br />
          sit culpa. Minim mollit voluptate
          <br />
          ullamco proident ea ad.
        </p>
      </div>
    </div>
  </div>
</template>
<style>
.values h1 {
  margin-top: 180px;
  font-size: 46px;
  font-weight: 700;
  text-align: center;
  line-height: 59.8px;
}
.values h3 {
  text-align: center;
  font-size: 18px;
  font-weight: 400;
  line-height: 27px;
  margin-top: 25px;
  color: #787a80;
  margin-bottom: 60px;
}
.values-grid {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  width: 65%;
  margin: 0 auto;
  margin-bottom: 120px;
}
.values-grid div {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  height: 188px;
}
.safety {
  border-left: 1px solid #dadbdd80;
  border-right: 1px solid #dadbdd80;
}
.values-grid div p {
  text-align: center;
  margin-bottom: 8px;
  font-size: 16px;
  font-weight: 400;
  line-height: 25.6px;
}
.values-grid h2 {
  font-size: 20px;
  font-weight: 700;
  line-height: 30px;
  margin-top: 8px;
  margin-bottom: 8px;
}
@media (max-width: 1200px) {
  .values-grid {
    width: 70%;
  }
  .values-grid div p {
    font-size: 14px;
  }
}
@media (max-width: 1000px) {
  .values-grid {
    width: 80%;
  }
}
@media (max-width: 850px) {
  .values-grid div p {
    line-height: 20px;
    font-size: 12px;
  }
}
@media (max-width: 700px) {
  .values-grid {
    grid-template-columns: 1fr;
    gap: 25px;
  }
  .values-grid div p {
    line-height: 25px;
    font-size: 15px;
  }
}
</style>
