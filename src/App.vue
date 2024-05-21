<template>
  <nav>
    <!-- <router-link to="/">Home</router-link> | -->
    <!-- <router-link to="/about">About</router-link> -->
    <router-view/>
  </nav>
</template>

<style>
body {
  margin: 0 !important;
}
#app {
  max-width: 1920px;
  width: 100%;
  margin: 0 auto;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  font-family: BrinnanRegular !important;
}

span {
  color: #FF540B;
}

:root {
  color-scheme: light dark;
  background-color: #ffffff;
  font-synthesis: none;
  text-rendering: optimizeLegibility;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.secondarybtn {
  width: 200px;
  padding: 20px;
  border-radius: 50px;
  border: none;
  gap: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #FF540B;
  color: #ffffff;
  height: 74px;
  font-family: BrinnanRegular;
  font-weight: 400;
  letter-spacing: 0em;
  font-size: 20px;

}
.a {
  width: 200px;
  padding: 20px;
  border-radius: 50px;
  border: none;
  gap: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #FF540B;
  color: #ffffff;
  height: 74px;
  font-family: BrinnanRegular;
  font-weight: 400;
  letter-spacing: 0em;
  font-size: 20px;

}

.secondarybtn:hover {
  background-color: #ffffff;
  color: #FF540B;
}

.primarybutton {
  width: 200px;
  padding: 15px;
  border-radius: 50px;
  border: 1px solid #2A2929;
  gap: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #00000000;
  color: #2A2929;
  height: 7px;
  font-family: BrinnanRegular;
  font-weight: 400;
  letter-spacing: 0em;
  font-size: 20px;
}

.primarybutton:hover {
  background-color: #2A2929;
  color: #ffffff;
}
/* nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
} */
@font-face {
  font-family: archivo;
  src: url("./assets/Fonts/Archivo-Black.ttf");
}
@font-face {
  font-family: ReportFont;
  src: url("./assets/Fonts/ReportSchoolW00-Heavy.ttf");
}

@font-face {
  font-family: BrinnanRegular;
  src: url("./assets/Fonts/BrinnanRegular.ttf");
}

@font-face {
  font-family: BrinnanBlackOblique;
  src: url("./assets/Fonts/BrinnanBlackOblique.ttf");
}

@font-face {
  font-family: BrinnanBold;
  src: url("./assets/Fonts/BrinnanBold.ttf");
}

@font-face {
  font-family: BrinnanBoldOblique;
  src: url("./assets/Fonts/BrinnanBoldOblique.ttf");
}

@font-face {
  font-family: BrinnanLight;
  src: url("./assets/Fonts/BrinnanLight.ttf");
}

@font-face {
  font-family: BrinnanLightOblique;
  src: url("./assets/Fonts/BrinnanLightOblique.ttf");
}




</style>
