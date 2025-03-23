<template>
  <div class="services">
    <h1>Our services</h1>
    <p>
      Createx Construction Bureau is a construction giant with a full range of
      construction services.
    </p>
    <div class="services-wrapper">
      <div class="service-inner-1">
        <img src="/construction.svg" alt="" />
        <h2>Construction</h2>
      </div>
      <div class="service-inner-2">
        <img src="/plan.svg" alt="" />
        <h2>Project Development</h2>
      </div>
      <div class="service-inner-3">
        <img src="/plan.svg" alt="" />
        <h2>Interior Design</h2>
      </div>
      <div class="service-inner-4">
        <img src="/painting.svg" alt="" />
        <h2>Repairs</h2>
      </div>
    </div>
    <span>
      <h2>Learn more about our services</h2>
      <button>View services</button>
    </span>
  </div>
</template>
<style>
.services {
  margin-top: 120px;
  text-align: center;
}
.services span {
  display: flex;
  gap: 40px;
  justify-content: center;
  align-items: center;
  margin-top: 85px;
  margin-bottom: 200px;
}
.services span h2 {
  font-size: 28px;
  font-weight: 700;
  line-height: 42px;
}
.services span button {
  width: 207px;
  height: 52px;
  background: #ff5a30;
  border: none;
  color: white;
  font-size: 16px;
  font-weight: 700;
  line-height: 52px;
}
.services h1 {
  color: #1e212c;
  font-size: 46px;
  font-weight: 700;
  line-height: 59.8px;
  margin-bottom: 25px;
}
.services p {
  font-size: 18px;
  font-weight: 400;
  line-height: 27px;
  color: #787a80;
  margin-bottom: 60px;
}
.services-wrapper {
  display: grid;
  width: 65%;
  margin: 0 auto;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  gap: 30px;
}
.services-wrapper div {
  height: 230px;
  box-shadow: 2px 2px 2px 2px rgba(41, 41, 41, 0.1);
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.services-wrapper h2 {
  color: #1e212c;
  font-size: 20px;
  font-weight: 700;
  margin-top: 25px;
  line-height: 30px;
}

@media (max-width: 1000px) {
  .services-wrapper {
    grid-template-columns: 1fr 1fr;
  }
}
@media (max-width: 800px) {
  .services p {
    font-size: 14px;
    line-height: 20px;
  }
  .services h1 {
    font-size: 40px;
    line-height: 52px;
  }
  .services span {
    gap: 20px;
  }
  .services span h2 {
    font-size: 22px;
    line-height: 36px;
  }
  .services span button {
    width: 177px;
    font-size: 14px;
  }
  .services h1 {
    font-size: 40px;
    line-height: 54px;
  }
}

@media (max-width: 500px) {
  .services-wrapper {
    grid-template-columns: 1fr;
  }
  .services span {
    display: block;
  }
  .services span button {
    margin-top: 20px;
  }
  .services span {
    margin-top: 85px;
    margin-bottom: 100px;
  }
  .services p {
    font-size: 13px;
  }
}
@media (max-width: 350px) {
  .services span h2 {
    font-size: 18px;
    line-height: 32px;
  }
}
</style>
