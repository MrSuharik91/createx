<script>
import { setDevtoolsHook } from "vue";

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
      if (this.infoEmail.includes("@") && this.Checked) {
        this.infoName = "";
        this.infoPhone = "";
        this.infoEmail = "";
        this.infoMessage = "";
        this.Checked = false;
        this.email = false;
      } else {
        if (!this.infoEmail.includes("@")) {
          this.email = true;
        } else {
          this.email = false;
        }
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
.disscus-wrapper h1 {
  font-size: 28px;
  font-weight: 700;
  line-height: 42px;
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
  width: 45%;
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
  cursor: pointer;
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
@media (max-width: 1200px) {
  .disscus-wrapper {
    background-size: contain;
    background-size: 130% 100%;
  }
}
@media (max-width: 1200px) {
  .disscus-wrapper h1 {
    font-size: 23px;
    line-height: 36px;
  }
  .checkbox-wrapper span {
    font-size: 12px;
    line-height: 18px;
  }
}
@media (max-width: 1000px) {
  .disscus-wrapper h1 {
    font-size: 20px;
    line-height: 30px;
  }
  .checkbox-wrapper span {
    font-size: 10px;
    line-height: 16px;
  }
}
@media (max-width: 700px) {
  .disscus-wrapper h1 {
    font-size: 16px;
    line-height: 28px;
  }
  .checkbox-wrapper span {
    font-size: 8px;
    line-height: 14px;
    text-align: center;
  }
  .checkbox-wrapper {
    flex-direction: column-reverse;
  }
  .disscus p {
    font-size: 14px;
  }
  .disscus {
    width: 65%;
  }
  .disscus-wrapper button {
    width: 134px;
    line-height: 40px;
  }
}

@media (max-width: 450px) {
  .disscus-wrapper h1 {
    font-size: 13px;
    line-height: 24px;
  }
  .disscus-wrapper button {
    width: 100px;
    line-height: 40px;
  }
  .inputs {
    background: #f4f5f6;
    margin: 0 auto;
    width: 90%;
    height: 44px;
    border: none;
    padding-left: 12px;
  }
}
</style>
