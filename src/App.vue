<template>
  <div style="background-color: #e5e5e5; padding: 15px; text-align: center">
    <HeaderView />
  </div>
  <br /><br /><br />
  <div>
    <div class="menu">
      <LeftView />
    </div>

    <div class="main">
      <TimeView />
    </div>
  </div>
  <div class="project">
    <ProjectView />
  </div>
  <div
    style="
      background-color: #e5e5e5;
      text-align: center;
      padding: 10px;
      margin-top: 7px;
    "
  >
    <FooterView />
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import HeaderView from "./components/HeaderView.vue";
import FooterView from "./components/FooterView.vue";
import LeftView from "./components/LeftSideBar.vue";
//import RightView from "./components/RightSideBar.vue";
import TimeView from "./components/TimeLine.vue";
import ProjectView from "./components/ProjectView.vue";

export default {
  name: "App",
  components: {
    // HelloWorld,
    FooterView,
    HeaderView,
    LeftView,
    //RightView,
    TimeView,
    ProjectView,
  },
};
</script>

<style>
.banner {
  background-color: blueviolet;
}
* {
  box-sizing: border-box;
}

.menu {
  float: left;
  width: 30%;
  text-align: center;
}
a {
  text-decoration-color: black;
}

.menu a {
  background-color: #e5e5e5;
  padding: 8px;
  margin-top: 7px;
  display: block;
  width: 100%;
  color: black;
}

.main {
  background-color: #fafafa;
  float: left;
  width: 70%;
  padding: 0 20px;
}
.project {
  float: left;
  width: 100%;
}

.right {
  background-color: #eae4e4;
  float: left;
  width: 20%;
  padding: 15px;
  margin-top: 7px;
  text-align: center;
}

@media only screen and (max-width: 620px) {
  /* For mobile phones: */
  .menu,
  .main,
  .right {
    width: 100%;
  }
}
</style>
