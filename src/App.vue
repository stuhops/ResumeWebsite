<template>
  <nav class="navbar navbar-expand-sm navbar-light">
    <!-- Links -->
    <ul class="navbar-nav">
      <li class="nav-item">
        <a class="nav-link" href="#">Link 1</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Link 2</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Link 3</a>
      </li>
    </ul>
  </nav>
  <div id="app">
    <router-view />
  </div>
</template>

<style>
@font-face {
  font-family: "Crimson";
  src: local("Crimson"),
    url("./assets/fonts/Crimson-Semibold.otf") format("opentype");
}

* {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #f5f5f5;
}

h1, h2, h3, h4, h5, h6 {
  font-family: Crimson, serif;
}
</style>
