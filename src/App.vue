<template>
  <nav class="header-nav">
    <router-link id="conocimientos-a" to="/"
      ><h3>Conocimientos</h3></router-link
    >
    <router-link id="proyectos-a" to="/proyectos"
      ><h3>Proyectos</h3></router-link
    >
    <router-link style="border: none" id="sobre-mi-a" to="/sobre-mi"
      ><h3>Sobre mi</h3></router-link
    >
  </nav>
  <router-view />
</template>

<style>
* {
  margin: 0;
  box-sizing: border-box;
}

.video-bg {
  position: fixed;
  right: 0;
  top: 0;
  width: 100%;
  height: 100%;
}
video {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
a {
  text-decoration: none;
  color: #000;
  font-size: 1em;
}

body {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2e2f30;
  border: 1px solid #aaa;
  width: 90vw;
  height: 80vh;
  background: rgba(255, 255, 255, 0.25);
  box-shadow: 0 8px 32px 0 rgba(74, 74, 74, 0.37);
  backdrop-filter: blur(2px);
  -webkit-backdrop-filter: blur(4px);
  border-radius: 10px;
  border: 1px solid rgba(255, 255, 255, 0.18);
  display: flex;
  flex-flow: row wrap;
  overflow-y: scroll;
  overflow-x: hidden;
  z-index: 1;
}

#app::-webkit-scrollbar {
  -webkit-appearance: none;
}

#app::-webkit-scrollbar:vertical {
  width: 10px;
}

#app::-webkit-scrollbar-button:increment,
#app::-webkit-scrollbar-button {
  display: none;
}

#app::-webkit-scrollbar:horizontal {
  height: 10px;
}

#app::-webkit-scrollbar-thumb {
  background-color: rgba(221, 221, 221, 0.492);
  border-radius: 20px;
}

#app::-webkit-scrollbar-track {
  border-radius: 10px;
}

.header-nav {
  width: 90vw;
  height: 90px;
  display: flex;
  align-items: center;
  justify-content: center;
}
.header-nav a {
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100%;
  font-size: 1em;
  color: #151515;
}
.header-nav a:hover {
  border: none;
  border-radius: 10px;
  box-shadow: 0 8px 9px 0 rgba(2, 2, 2, 0.574);

  transition: 0.5s ease;
}
.header-nav a:focus {
  border: none;
  border-radius: 10px;
  box-shadow: 0 8px 9px 0 rgba(2, 2, 2, 0.574);

  transition: 0.5s ease;
}

@media all and (max-width: 768px) {
  .header-nav a {
    font-size: 0.9em;
  }
}
</style>
