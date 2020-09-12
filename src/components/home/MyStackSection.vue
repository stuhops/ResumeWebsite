<template>
  <div id="main-container">
    <div id="secondary-container">
      <div id="statement">
        <h2 id="header-text" class="flex">{{ headline }}</h2>
        <p class="flex">{{ description }}</p>
      </div>
      <div id="stacks">
        <div class="stack">
          <h3>Day to Day use</h3>
          <ul class="stack-list">
            <li>Django</li>
            <li>Python</li>
            <li>JavaScript</li>
            <li>Linux</li>
            <li>PostgreSQL</li>
            <li>Git</li>
            <li>HTML / CSS</li>
          </ul>
        </div>
        <div class="stack">
          <h3>Good understanding</h3>
          <ul class="stack-list">
            <li>Vue</li>
            <li>Docker</li>
            <li>GitHub Actions</li>
            <li>C++</li>
            <li>UX / UI</li>
          </ul>
        </div>
        <div class="stack">
          <h3>Familiarity with</h3>
          <ul class="stack-list">
            <li>React</li>
            <li>React Native</li>
            <li>Node.js</li>
            <li>Flask</li>
            <li>Java</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "TriplePictureStatementSection",
  props: {
    headline: String,
    description: String,
    image1: String,
    image2: String,
    image3: String
  }
};
</script>

<style scoped>
* {
  color: #f5f5f5;
}

h3 {
  text-align: center;
}

#content-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

#header-text {
  flex: 1;
  font-size: clamp(48px, 5vw, 72px);
  margin: 0;
}

#main-container {
  width: 100vw;
  max-width: 100vw;
  min-height: 60vh;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center top;
  background-color: #202020;
  display: flex;
  justify-content: center;
  align-items: center;
}

#secondary-container {
  border-style: solid;
  border-color: #f5f5f5;
  flex: 1;
  max-width: 1396px;
  margin: 10vh 20vw 10vh 20vw;
  padding: 64px 0 64px 0;
  display: flex;
  justify-content: flex-start;
  align-items: center;
  flex-direction: column;
  flex-wrap: wrap;
}

#stacks {
  max-width: 1396px;
  width: 95vw;
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  flex-wrap: wrap;
}

#statement {
  max-width: 1396px;
  width: 100%;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  display: flex;
  flex: 1;
}

.flex {
  flex: 1;
}

.stack {
  flex: 1;
  justify-content: center;
  max-width: 364px;
  width: 20vw;
  min-width: 100px;
  margin: 14px 3vw 14px 3vw;
}

.stack-list {
  flex: 1;
  width: auto;
  display: table;
  margin: 0 auto;
}

@media screen and (max-width: 526px) {
  #stacks {
    flex-direction: column;
  }

  .stack {
    flex: 1;
    width: 100%;
  }
}
</style>
