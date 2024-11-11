<script>
export default {
  data() {
    return {
      Checked: false,
      email: false,
      infoName: "",
      infoPhone: "",
      infoEmail: "",
      infoMessage: "",
    };
  },
  methods: {
    sendBtn() {
      if (!this.infoEmail.includes("@")) {
        this.email = true;
      } else {
        this.email = false;
      }
    },
  },
};
</script>
<template>
  <div class="disscus-wrapper" id="submit">
    <div class="disscus-inner">
      <div class="disscus">
        <h1>A quick way to discuss details</h1>
        <div>
          <p>Name*</p>
          <input
            v-model="infoName"
            class="inputs"
            type="text"
            placeholder="Your name"
          />
        </div>
        <div>
          <p>Phone*</p>
          <input
            v-model="infoPhone"
            class="inputs"
            type="number"
            placeholder="Your phone number"
          />
        </div>
        <div>
          <p>Email</p>
          <input
            v-model="infoEmail"
            class="inputs"
            type="text"
            placeholder="Your working email"
          />
          <h3 v-if="email">Email должен иметь "@"</h3>
        </div>
        <div>
          <p>Message*</p>
          <input
            v-model="infoMessage"
            type="text"
            class="inputs"
            placeholder="Your message"
          />
        </div>
        <div class="checkbox-wrapper">
          <input
            v-model="Checked"
            class="checkbox"
            type="checkbox"
            name=""
            id=""
          />
          <span
            >I agree to receive communications from Createx
            <br />
            Construction Bureau.</span
          >
        </div>
        <button @click="sendBtn" :class="Checked ? 'active' : 'inactive'">
          send request
        </button>
      </div>
    </div>
  </div>
</template>
<style>
html {
  scroll-behavior: smooth;
}
.disscus-wrapper {
  background-image: url(/discuss-bg.jpg);
  height: 820px;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  align-items: center;
}
.disscus-wrapper h3 {
  width: 65%;
  margin: 0 auto;
  font-size: 14px;
  margin-top: 8px;
}
.disscus-inner {
  width: 65%;
  display: flex;
  justify-content: end;
  margin: 0 auto;
}
.disscus {
  height: 666px;
  background: #ffffff;
  width: 495px;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3), 0 15px 30px rgba(0, 0, 0, 0.25);
  text-align: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  gap: 21px;
}
.disscus p {
  text-align: start;
  width: 87%;
  margin: 0 auto;
  margin-bottom: 8px;
}
.inputs {
  background: #f4f5f6;
  margin: 0 auto;
  width: 85%;
  height: 44px;
  border: none;
  padding-left: 12px;
}
.checkbox {
  width: 16px;
  height: 16px;
}
.checkbox-wrapper {
  display: flex;
  align-items: center;
  width: 85%;
  gap: 12px;
  margin: 0 auto;
}
.checkbox-wrapper span {
  color: #424551;
  text-align: start;
  font-size: 14px;
  font-weight: 400;
  line-height: 21px;
}
.disscus-wrapper button {
  opacity: 0.6;
  width: 174px;
  height: 44px;
  background: #ff5a30;
  border: none;
  font-size: 14px;
  font-weight: 700;
  line-height: 44px;
  color: white;
  margin: 0 auto;
}
.disscus-wrapper button.active {
  background: #ff5a30;
  opacity: 1;
}

.disscus-wrapper button.inactive {
  background: #ff5a30;
  opacity: 0.5;
}
</style>
