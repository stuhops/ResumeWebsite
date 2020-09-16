<template>
  <nav id="nav">
    <!-- Links -->
    <ul id="nav-link-custom-section" class="nav-section">
      <li class="nav-link-custom">
        <a class="nav-link-custom" href="#"></a>
      </li>
      <li class="nav-link-custom">
        <a class="nav-link-custom" href="#"></a>
      </li>
      <li class="nav-link-custom">
        <a class="nav-link-custom" href="#"></a>
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

@font-face {
  font-family: "ProximaNova";
  src: local("ProximaNova"),
    url("./assets/fonts/ProximaNova-Regular.otf") format("opentype");
}

* {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  box-sizing: border-box;
}

body {
  margin: 0px;
}

h1,
h2 {
  font-family: Crimson, serif;
  color: #f5f5f5;
}

h3,
h4,
h5,
h6 {
  font-family: ProximaNova, sans-serif;
  color: #E1A87A;
}

a,
p,
li {
  font-family: ProximaNova, sans-serif;
  font-size: 16px;
  color: #f5f5f5;
}

a:hover,
button:hover {
  cursor: pointer;
}

p {
  line-height: 2;
}

ul {
  list-style-type: circle;
  list-style-position: inside;
  color: #f5f5f5;
}

#nav {
  margin-bottom: -96px;
  display: flex;
  flex-direction: row;
}

#nav-link-custom-section {
  justify-content: center;
}

.borderless-button-dark {
  max-width: 90vw;
  border-style: none;
  background-color: transparent;
  color: #202020;
  text-shadow: 0px 0px 10px #f5f5f5;
  text-shadow: 0px 0px 10px #f5f5f5;
  padding: 10px 20px 10px 20px;
}

.borderless-button-light {
  max-width: 90vw;
  border-style: none;
  background-color: transparent;
  color: #f5f5f5;
  text-shadow: 0px 0px 10px #202020;
  text-shadow: 0px 0px 10px #202020;
  padding: 10px 20px 10px 20px;
}

.borderless-button-light:hover,
.borderless-button-dark:hover {
  opacity: 0.7;
}

.outlined-button-dark {
  max-width: 90vw;
  border-style: solid;
  border-color: #E1A87A;
  background-color: transparent;
  color: #202020;
  text-shadow: 0px 0px 10px #f5f5f5;
  text-shadow: 0px 0px 10px #f5f5f5;
  padding: 20px 40px 20px 40px;
}

.outlined-button-dark:hover {
  background-color: #202020;
  color: #f5f5f5;
  text-shadow: none;
}

.outlined-button-light {
  max-width: 90vw;
  border-style: solid;
  border-color: #E1A87A;
  background-color: transparent;
  color: #f5f5f5;
  text-shadow: 0px 0px 10px #202020;
  text-shadow: 0px 0px 10px #202020;
  padding: 20px 40px 20px 40px;
}

.outlined-button-light:hover {
  background-color: #f5f5f5;
  color: #202020;
  text-shadow: none;
}

.nav-section {
  height: 96px;
  max-width: 1396px;
  margin: 0 10vw 0 10vw;
  padding: 0;
  flex: 1;
  display: flex;
  flex-direction: row;
  align-items: center;
}

.nav-link-custom {
  flex: 1;
  display: flex;
  justify-content: center;
  font-size: 1.5rem;
  color: #f5f5f5;
  text-shadow: 0px 0px 10px #000000;
  text-shadow: 0px 0px 10px #000000;
}
</style>
