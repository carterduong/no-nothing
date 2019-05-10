<template>
  <div id="container">
    <div id="letters">
        <span id="L1" onclick=${letterClick} @mouseover="hoverOver">N</span>
        <span id="L2" onclick=${letterClick}>O</span>
        <span id="space">&nbsp;</span>
        <span id="L3" onclick=${letterClick}>N</span>
        <span id="L4" onclick=${letterClick}>O</span>
        <span id="L5" onclick=${letterClick}>T</span>
        <span id="L6" onclick=${letterClick}>H</span>
        <span id="L7" onclick=${letterClick}>I</span>
        <span id="L8" onclick=${letterClick}>N</span>
        <span id="L9" onclick=${letterClick}>G</span>
        <span id="at" onclick=${letterClick}>@</span>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
  }
}
</script>

<style scoped>
@font-face {
  font-family: 'Tex-Gyre-Heros';
  src: url('../assets/texgyreheroscn-regular.otf') format('opentype')
}

span:hover {
  filter: drop-shadow(0px 0px 10px white);
  color: black;
  mix-blend-mode: exclusion;
  cursor: pointer;
}

#container {
  height: 100vh;
  width: 100vw;
  background: rgb(0,0,0);
  display: flex;
  align-items: center;
  justify-content: center;
}

#letters {
  font-family: 'Tex-Gyre-Heros';
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  white-space: pre;
  font-size: 100px;
  mix-blend-mode: difference;
  color: white;
  
  user-select: none;
  -moz-user-select: none;
  -webkit-user-select: none;
  -ms-user-select: none;
}

#at {
  font-size: 20px;
}
</style>