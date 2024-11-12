<script></script>
<template>
  <div class="selected">
    <h1>
      Browse our selected projects
      <br />
      and learn more about our work
    </h1>
    <div class="projects">
      <div>
        <img src="/Red-Finger.jpg" alt="" />
        <h2>Red Finger Building</h2>
        <p>Business Centers</p>
        <button>View Project</button>
      </div>
      <div>
        <img src="/Cubes-Building.png" alt="" />
        <h2>Cubes Building</h2>
        <p>Business Centers</p>
        <button>View Project</button>
      </div>
      <div>
        <img src="/Pencil-Building.png" alt="" />
        <h2>The Pencil Building</h2>
        <p>Stores & Malls</p>
        <button>View Project</button>
      </div>
    </div>
  </div>
</template>
<style>
.selected {
  display: flex;
  flex-direction: column;
  align-items: start;
}
.selected h1 {
  font-size: 46px;
  font-weight: 700;
  line-height: 59.8px;
  width: 65%;
  margin: 0 auto;
}
.projects {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 30px;
  width: 65%;
  justify-content: center;
  margin: 0 auto;
}
.projects div {
  text-align: center;
  position: relative;
  transition: transform 0.3s ease;
}
.projects div:hover {
  transform: translateY(-60px);
}
.projects div:hover button {
  opacity: 1;
}
.projects div button {
  border: 1px solid #ff5a30;
  background: transparent;
  width: 172px;
  height: 44px;
  position: absolute;
  bottom: -40px;
  left: 50%;
  transform: translateX(-50%);
  opacity: 0;
  transition: opacity 0.3s ease;
}
.projects p {
  color: #787a80;
  font-size: 14px;
  font-weight: 400;
  line-height: 21px;
  margin-bottom: 20px;
}
.projects h2 {
  margin-top: 15px;
  font-size: 20px;
  font-weight: 700;
  line-height: 30px;
  color: #1e212c;
}
.projects img {
  width: 100%;
  margin-top: 60px;
}
@media (max-width: 900px) {
  .selected h1 {
    font-size: 34px;
    line-height: 44px;
  }
  .projects h2 {
    font-size: 16px;
    line-height: 26px;
  }
}
@media (max-width: 750px) {
  .projects h2 {
    font-size: 13px;
    line-height: 22px;
  }
  .selected h1 {
    font-size: 30px;
    line-height: 40px;
  }
}

@media (max-width: 600px) {
  .selected h1 {
    font-size: 24px;
    line-height: 34px;
  }
  .projects {
    grid-template-columns: 1fr;
  }
  .projects h2 {
    font-size: 18px;
    line-height: 30px;
  }
  .projects p {
    font-size: 16px;
  }
}
@media (max-width: 450px) {
  .selected h1 {
    font-size: 16px;
    line-height: 24px;
  }
}

@media (max-width: 350px) {
  .selected h1 {
    font-size: 13px;
    line-height: 20px;
    text-align: center;
  }
}
</style>
