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
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: "App"
};
</script>

<style>
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
  color: green;
  text-decoration: none;
  font-size: 1.2em;
}
li {
  list-style-type: none;
  margin: 10px;
}
.router-link-active {
  color: blue;
}
</style>
