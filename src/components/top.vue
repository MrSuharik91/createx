<script>
import ScrollReveal from "scrollreveal";
import { onMounted } from "vue";
export default {
  data() {
    return {
      menu: window.innerWidth <= 750,
      menuHidden: false,
    };
  },
  methods: {
    menuClick() {
      this.menuHidden = true;
      this.menu = false;
    },
    exit() {
      this.menuHidden = false;
      this.menu = true;
    },
  },
  mounted() {
    ScrollReveal().reveal(".head", {
      duration: 1200,
      origin: "left",
      delay: 200,
      distance: "200px",
    });
    ScrollReveal().reveal(".construction-wrapper", {
      duration: 1200,
      origin: "left",
      delay: 800,
      distance: "200px",
    });
    ScrollReveal().reveal(".service-inner-1", {
      duration: 500,
      origin: "top",
      delay: 350,
      distance: "200px",
    });
    ScrollReveal().reveal(".service-inner-2", {
      duration: 500,
      origin: "bottom",
      delay: 350,
      distance: "200px",
    });
    ScrollReveal().reveal(".service-inner-3", {
      duration: 500,
      origin: "top",
      delay: 350,
      distance: "200px",
    });
    ScrollReveal().reveal(".service-inner-4", {
      duration: 500,
      origin: "bottom",
      delay: 350,
      distance: "200px",
    });
    ScrollReveal().reveal(".red", {
      duration: 700,
      origin: "left",
      delay: 500,
      distance: "300px",
    });
    ScrollReveal().reveal(".cub", {
      duration: 700,
      origin: "left",
      delay: 350,
      distance: "200px",
    });
    ScrollReveal().reveal(".pencil", {
      duration: 700,
      origin: "left",
      delay: 350,
      distance: "200px",
    });
  },
};
</script>
<template>
  <div class="head" id="to-top">
    <div class="links">
      <img class="logo" src="/logo.svg" alt="" />
      <a class="links-header" href="">About Us</a>
      <a class="links-header" href="">Services</a>
      <a class="links-header" href="">Work</a>
      <a class="links-header" href="">News</a>
      <a class="links-header" href="">Contacts</a>
    </div>
    <div class="info-wrapper">
      <div class="info">
        <img src="/iPhone.svg" alt="" />
        <p>
          <span>Call us</span>
          <br />
          (405) 555-0128
        </p>
      </div>
      <div class="info">
        <img src="/Chat.svg" alt="" />
        <p>
          <span>Talk to us</span>
          <br />
          hello@createx.com
        </p>
      </div>
    </div>

    <img
      @click="menuClick"
      v-if="menu"
      class="menu"
      src="/hamburger.svg"
      alt=""
    />
  </div>

  <div class="MenuHide" v-if="menuHidden">
    <img class="exit" @click="exit" src="/exit.svg" alt="" />
    <div class="hover-info">
      <a href="">About Us</a>
    </div>
    <div class="hover-info">
      <a href="">Services</a>
    </div>
    <div class="hover-info">
      <a href="">Work</a>
    </div>
    <div class="hover-info">
      <a href="">News</a>
    </div>
    <div class="hover-info">
      <a href="">Contacts</a>
    </div>
    <div class="info-wrapper-phone">
      <div>
        <img src="/iPhone.svg" alt="" />
        <p>
          <span>Call us</span>
          (405) 555-0128
        </p>
      </div>
      <img class="logo" src="/logo.svg" alt="" />
      <div>
        <img src="/Chat.svg" alt="" />
        <p>
          <span>Talk to us</span>
          hello@createx.com
        </p>
      </div>
    </div>
  </div>
</template>
<style scoped>
a {
  color: #424551;
}
.links {
  display: flex;
  align-items: center;
  gap: 30px;
}
span {
  color: #424551;
  font-size: 16px;
  font-weight: 700;
  line-height: 21px;
}
.info {
  display: flex;
  gap: 10px;
}
.info-wrapper {
  display: flex;
  align-items: center;
  gap: 35px;
}
.head {
  display: flex;
  width: 65%;
  margin: 0 auto;
  justify-content: space-between;
  align-items: center;
  margin-top: 20px;
}

.info-wrapper-phone {
  width: 80%;
  border-radius: 15px;
  height: 18%;
  background-color: rgb(255, 255, 255);
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.info-wrapper-phone div {
  text-align: center;
}
.menu {
  width: 40px;
  height: 40px;
}
.MenuHide {
  position: fixed;
  top: 0;
  left: 0;
  width: 100vw;
  height: 100vh;
  z-index: 9999;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background-color: rgb(255, 115, 0);
  gap: 25px;
  overflow: hidden;
}
.hover-info {
  cursor: pointer;
  width: 80%;
  border-radius: 15px;
  height: 7.5%;
  background-color: rgb(255, 255, 255);
  display: flex;
  justify-content: center;
  align-items: center;
  transition: 0.3s;
}
.hover-info:hover {
  scale: 0.8;
}
.hover-info a {
  font-size: 26px;
}
.exit {
  width: 40px;
  height: 40px;
  position: absolute;
  top: 20px;
  right: 40px;
}
@media (max-width: 1300px) {
  .info-wrapper {
    gap: 20px;
  }
  .info-wrapper-phone {
    flex-direction: column;
    gap: 20px;
    height: auto;
    padding-top: 15px;
    padding-bottom: 15px;
  }
  .info-wrapper img {
    width: 25px;
    height: 25px;
  }
  .info {
    align-items: center;
  }
  span {
    font-size: 13px;
    line-height: 16px;
  }
  .info-wrapper p {
    font-size: 14px;
  }
  a {
    font-size: 14px;
  }
  .logo {
    width: 110px;
  }
  .links {
    gap: 20px;
  }
}
@media (max-width: 1100px) {
  .info-wrapper {
    gap: 10px;
  }
  .info-wrapper img {
    width: 17px;
    height: 17px;
  }
  span {
    font-size: 12px;
    line-height: 15px;
  }
  .info-wrapper p {
    font-size: 12px;
  }
  a {
    font-size: 12px;
  }
  .logo {
    width: 100px;
  }
}
@media (max-width: 950px) {
  .head {
    width: 85%;
  }
}
@media (max-width: 750px) {
  .head {
    display: block;
    position: relative;
  }
  .menu {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    right: 0px;
  }
  .info-wrapper {
    display: none;
  }
  .logo {
    width: 80px;
  }
  .head {
    width: 90%;
  }
  .info-wrapper img {
    width: 13px;
    height: 13px;
  }
  .links-header {
    display: none;
  }
}
@media (max-width: 550px) {
  .exit {
    width: 25px;
    height: 25px;
    top: 8px;
    right: 20px;
  }
  .info-wrapper-phone p {
    font-size: 14px;
  }
  .logo {
    width: 70px;
  }
  .MenuHide {
    padding-top: 20px;
    padding-bottom: 20px;
  }
  .info-wrapper-phone {
    padding-top: 15px;
    padding-bottom: 30px;
    margin-bottom: 40px;
  }
}
@media (max-width: 350px) {
  .hover-info a {
    font-size: 18px;
  }
  .info-wrapper-phone p {
    font-size: 12px;
  }
  .exit {
    width: 40px;
    height: 40px;
    top: 15px;
    right: 20px;
  }
}
</style>
