<template>
  <div class="construction">
    <div class="construction-wrapper">
      <h1>
        CREATE<span>X</span>
        <br />
        CONSTRUCTION
      </h1>
      <p>
        Cras ultrices leo vitae non
        <br class="br-hidden" />
        viverra. Fringilla nisi quisque
        <br />
        consequat, dignissim vitae
        <br class="br-hidden" />
        proin ipsum sed. Pellentesque nec
        <br />
        turpis purus eget pellentesque
        <br class="br-hidden" />
        integer ipsum elementum felis.
      </p>
      <div class="construction-links">
        <a href="" class="learn">Learn more about us</a>
        <a href="#submit" class="submit">SUBMIT REQUEST</a>
      </div>
    </div>
  </div>
</template>
<style scoped>
.construction {
  background-image: url(/bg-image.jpg);
  width: 100%;
  height: 775px;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  margin-top: 25px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.learn {
  border: 1px solid #ffffff;
  background: none;
  width: 278px;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 52px;
  color: white;
  font-size: 16px;
  font-weight: 700;
  line-height: 52px;
}
.construction-wrapper {
  width: 65%;
  margin: 0 auto;
}
.construction-wrapper h1 {
  font-size: 72px;
  font-weight: 700;
  color: white;
  line-height: 93.6px;
}
.construction-wrapper span {
  color: #ff5a30;
}
.construction-wrapper p {
  font-size: 20px;
  font-weight: 400;
  line-height: 30px;
  color: white;
  margin-top: 20px;
  margin-bottom: 60px;
}
.submit {
  background: #ff5a30;
  width: 224px;
  height: 53.6px;
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  font-size: 16px;
  font-weight: 700;
  line-height: 52px;
}
.br-hidden {
  display: none;
}
.construction-links {
  display: flex;
  gap: 25px;
}
@media (max-width: 1300px) {
  .construction {
    background-size: contain;
  }
}
@media (max-width: 1000px) {
  .construction-wrapper h1 {
    font-size: 62px;
    line-height: 83.6px;
  }
  .construction-wrapper p {
    font-size: 16px;
  }
}
@media (max-width: 800px) {
  .construction-wrapper h1 {
    font-size: 50px;
    line-height: 63.6px;
  }
  .construction-wrapper p {
    font-size: 14px;
  }
  .submit {
    width: 154px;
    height: 53.6px;
    font-size: 14px;
    line-height: 45px;
  }
  .construction-wrapper p {
    font-size: 12px;
    margin-top: 10px;
    margin-bottom: 20px;
  }
  .construction-wrapper {
    width: 80%;
  }
}
@media (max-width: 650px) {
  .construction-wrapper h1 {
    font-size: 32px;
    line-height: 43.6px;
  }
}
@media (max-width: 500px) {
  .construction-links {
    flex-direction: column;
    gap: 15px;
  }
  .br-hidden {
    display: block;
  }
  .construction {
    background-size: 120% 65%;
  }
}
@media (max-width: 400px) {
  .construction-wrapper h1 {
    font-size: 28px;
    line-height: 40px;
  }
  .learn {
    width: 230px;
    font-size: 13px;
    white-space: nowrap;
  }
}
</style>
