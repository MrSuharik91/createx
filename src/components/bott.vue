<template>
  <footer>
    <div class="footer-wrapper">
      <div>
        <div class="logo-footer">
          <img src="/logo-2.svg" alt="" />
          <div class="media">
            <img src="/Whatsapp.svg" alt="" />
            <img src="/Messanger.svg" alt="" />
            <img src="/Facebook.svg" alt="" />
            <img src="/Twitter.svg" alt="" />
            <img src="/YouTube.svg" alt="" />
          </div>
        </div>
        <p>
          Createx Construction Bureau has been successfully operating in the USA
          <br />
          construction market since 2000. We are proud to offer you quality
          <br />
          construction and exemplary service. Our mission is to set the highest
          <br />
          standards for construction sphere.
        </p>
      </div>
      <div>
        <h1>Let’s stay in touch</h1>
        <div class="input-btn">
          <input type="text" placeholder="Your email address " />
          <button>subscribe</button>
        </div>
        <h4>
          *Subscribe to our newsletter to receive communications and early
          updates from Createx
          <br />
          Construction Bureau.
        </h4>
      </div>
    </div>
    <div class="info-bott">
      <div class="info-bott-wrapper">
        <h2>HEAD OFFICE</h2>
        <p>8502 Preston Rd. Inglewood, New York</p>
        <p>Call:(405) 555-0128</p>
        <p>Email:hello@createx.com</p>
      </div>
      <div>
        <h2>WHO WE ARE</h2>
        <p>About Us</p>
        <p>Available Positions</p>
        <p>Contacts</p>
      </div>
      <div>
        <h2>OUR EXPERIENCE</h2>
        <p>Services</p>
        <p>Work</p>
        <p>News</p>
      </div>
    </div>
    <div class="bott-div">
      <p>© All rights reserved. Made by Createx Studio</p>
      <div class="bott-div-top">
        <span>GO TO TOP</span>
        <a href="#to-top"><img id="to-top" src="/up-btn.svg" alt="" /></a>
      </div>
    </div>
  </footer>
</template>
<style>
footer {
  background: #1e212c;
  height: 566px;
  width: 100%;
  padding-top: 80px;
}
.logo-footer {
  display: flex;
  gap: 60px;
}
.footer-wrapper p {
  font-size: 14px;
  font-weight: 400;
  line-height: 21px;
  color: white;
  margin-top: 24px;
}
.media {
  display: flex;
  gap: 16px;
}
.footer-wrapper {
  display: flex;
  width: 65%;
  margin: 0 auto;
  justify-content: space-between;
}
.footer-wrapper h4 {
  font-size: 12px;
  font-weight: 400;
  line-height: 18px;
}
.footer-wrapper h1 {
  color: white;
  font-size: 24px;
  font-weight: 700;
  line-height: 36px;
  margin-bottom: 24px;
}
.input-btn button {
  width: 131px;
  height: 45.6px;
  background: #ff5a30;
  border: none;
  color: white;
  font-size: 14px;
  font-weight: 700;
  line-height: 44px;
}
.input-btn input {
  height: 44px;
  background: #ffffff1f;
  width: 364px;
  padding-left: 15px;
  border: 1px solid #ffffff33;
}
.footer-wrapper h4 {
  color: white;
  margin-top: 16px;
  font-size: 12px;
  font-weight: 400;
  line-height: 18px;
  margin-bottom: 50px;
}
.info-bott {
  display: flex;
  width: 65%;
  margin: 0 auto;
  justify-content: space-between;
}
.info-bott p {
  color: white;
  font-size: 16px;
  font-weight: 400;
  line-height: 25.6px;
}
.info-bott h2 {
  font-size: 16px;
  font-weight: 700;
  line-height: 24px;
  margin-bottom: 13px;
  color: white;
}
.bott-div {
  display: flex;
  justify-content: space-between;
  width: 65%;
  margin: 0 auto;
  align-items: end;
}
.bott-div p {
  margin-top: 60px;
  color: #ffffff;
  font-size: 12px;
  font-weight: 400;
  line-height: 18px;
}
.bott-div-top {
  margin-top: 60px;
  display: flex;
  align-items: end;
  gap: 16px;
}
.bott-div-top span {
  font-size: 14px;
  font-weight: 400;
  line-height: 21px;
  color: white;
}
</style>
