<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">خانه</router-link> |
      <router-link to="/about">درباره ما</router-link>
    </div>
    <h1>رویدادها و مناسبت ها</h1>
    <router-view />
  </div>
</template>

<style>


#app {
  direction: rtl;
  font-family: 'IRANSans' !important;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  font-family: 'IRANSans' !important;
  padding: 30px;
}

#nav a {
  text-decoration: none;
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

h4 {
  font-size: 20px;
}
</style>
