<template>
  <div id="main-container">
    <div id="secondary-container">
      <div id="statement">
        <h2 id="header-text" class="flex">{{ headline }}</h2>
      </div>
      <div id="buttons">
        <a id="email" href="mailto:stuart.hops@gmail.com">
          <button class="outlined-button-light">Contact Me</button>
        </a>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "WorkWithMeSection",
  props: {
    headline: String,
  }
};
</script>

<style scoped>
* {
  color: #f5f5f5;
}

h3 {
  text-align: center;
  color: #E1A87A;
}

#buttons {
  margin: 32px 0 0 0;
}

#header-text {
  flex: 1;
  margin: 0;
}

#main-container {
  max-width: 100vw;
  min-height: 50vh;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center top;
  background-color: #202020;
  display: flex;
  justify-content: center;
  align-items: center;
}

#secondary-container {
  flex: 1;
  max-width: 1396px;
  padding: 64px 8px 64px 8px;
  display: flex;
  justify-content: flex-start;
  align-items: center;
  flex-direction: column;
  flex-wrap: wrap;
}

#statement {
  max-width: 1396px;
  width: 100%;
  justify-content: center;
  align-items: center;
  text-align: center;
  flex-direction: column;
  display: flex;
  flex: 1;
}

.flex {
  flex: 1;
}
</style>
