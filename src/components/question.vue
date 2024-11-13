<template>
  <div class="question">
    <h1>Want to know more? Ask us a question:</h1>
    <div class="question-wrapper">
      <div class="name-phone-div">
        <h2>Name</h2>
        <input
          type="text"
          name=""
          id=""
          placeholder="Your name"
          class="name-phone"
        />
      </div>
      <div class="phone-div">
        <h2>Phone</h2>
        <input
          type="number"
          name=""
          id=""
          placeholder="Your phone"
          class="name-phone"
        />
      </div>
      <div class="message-div">
        <h2>Message</h2>
        <input
          type="text"
          name=""
          id=""
          placeholder="Your message"
          class="message"
        />
      </div>
      <button>Send</button>
    </div>
  </div>
</template>
<style>
.question {
  width: 65%;
  margin: 0 auto;
  text-align: center;
}
.name-phone {
  padding-left: 15px;
  height: 44px;
  width: 100%;
}
.message {
  padding-left: 15px;
  width: 100%;
  height: 44px;
}
.question-wrapper {
  display: flex;
  gap: 34px;
  justify-content: center;
  align-items: end;
}
.question-wrapper div {
  display: flex;
  flex-direction: column;
  align-items: start;
}
.question-wrapper div h2 {
  font-size: 14px;
  font-weight: 400;
  line-height: 21px;
  color: #424551;
  margin-bottom: 8px;
}
.question-wrapper button {
  height: 47.2px;
  background: #ff5a30;
  border: none;
  font-size: 14px;
  font-weight: 700;
  line-height: 44px;
  color: white;
  width: 10%;
  cursor: pointer;
}
.question h1 {
  font-size: 28px;
  font-weight: 700;
  line-height: 42px;
  margin-bottom: 35px;
  color: #424551;
}
.name-phone-div {
  width: 20%;
}
.message-div {
  width: 30%;
}
input[type="number"]::-webkit-outer-spin-button,
input[type="number"]::-webkit-inner-spin-button {
  -webkit-appearance: none;
  margin: 0;
}
@media (max-width: 850px) {
  .question-wrapper {
    gap: 24px;
  }
  .question {
    width: 75%;
  }
}
@media (max-width: 700px) {
  .question-wrapper {
    display: block;
  }
  .question {
    text-align: start;
  }
  .name-phone-div {
    width: 100%;
  }
  .message-div {
    width: 100%;
  }
  .phone-div {
    margin-top: 25px;
    margin-bottom: 25px;
  }
  .question-wrapper button {
    width: 30%;
    margin-top: 25px;
  }
}
@media (max-width: 450px) {
  .question h1 {
    font-size: 18px;
    line-height: 26px;
  }
  .question-wrapper button {
    width: 40%;
  }
}
</style>
