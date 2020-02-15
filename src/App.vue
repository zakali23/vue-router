<template>
  <div id="app">
    <nav>
      <ol class="header">
        <li>
          <router-link class="link" :to="{ path: '/home'}">Home</router-link>
        </li>
        <li>
          <router-link class="link" :to="{ path: '/contact'}">Contact</router-link>
        </li>
      </ol>
    </nav>
    <transition
      name="fade"
      enter-active-class="animated fadeInLeft"
      leave-active-class="animated fadeOutRight"
    >
      <router-view></router-view>
    </transition>
  </div>
</template>

<script>
export default {
  name: "App"
};
</script>

<style>
@import "animate.css";
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.header {
  display: flex;
  flex-direction: row;
  justify-content: center;
}
.link {
  color: gray;
  text-decoration: none;
  font-size: 1.2em;
}
li {
  list-style-type: none;
  margin: 10px;
}
.router-link-active {
  color: green;
}
</style>
