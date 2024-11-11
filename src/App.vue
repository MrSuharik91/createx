<script setup>
import top from "./components/top.vue";
import construction from "./components/construction.vue";
import Bureau from "./components/Bureau.vue";
import values from "./components/values.vue";
import question from "./components/question.vue";
import services from "./components/services.vue";
import selected from "./components/selected.vue";
import partners from "./components/partners.vue";
import news from "./components/news.vue";
import disscus from "./components/disscus.vue";
import bott from "./components/bott.vue";
</script>
<template>
  <div>
    <top />
    <construction />
    <Bureau />
    <values />
    <question />
    <services />
    <selected />
    <div class="explore">
      <h2>Explore all our works</h2>
      <button>View portfolio</button>
    </div>
    <partners />
    <news />
    <disscus />
    <bott />
  </div>
</template>
<style>
* {
  padding: 0;
  margin: 0;
}
a {
  text-decoration: none;
}
.explore {
  margin-top: 80px;
  display: flex;
  justify-content: center;
  gap: 40px;
  align-items: center;
  margin-bottom: 125px;
}
.explore h2 {
  font-size: 28px;
  font-weight: 700;
  line-height: 42px;
}
.explore button {
  background: #ff5a30;
  font-size: 16px;
  font-weight: 700;
  line-height: 52px;
  border: none;
  color: white;
  width: 224px;
  height: 52px;
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
