<template>
    <div>
        <h1>Cool, hi.<br>My name is<br>D.A. Kahn.</h1>
        <p id="description">I'm a JavaScript developer working for <a href="/">IBM Design</a> in Austin, Texas.💀<p>
        <p id="links">Check out my <span><a href="/">Github</a></span> for code and to see the kinds of projects that interest me. Head to my <span><a href="/">LinkedIn</a></span> to get in touch or read what I've written on my <span><a href="/">Medium</a></span>.
        </p>
    </div>
</template>

<script>
import Caricature from "../static/caricature.svg";

export default {
  name: "menu",
  components: {
    Caricature
  }
};
</script>

<style>
@font-face {
  font-family: "DDCHardware-Compressed";
  src: url("../static/DDCHardware-Compressed.otf");
}

@font-face {
  font-family: "DDCHardware-Condensed";
  src: url("../static/DDCHardware-Condensed.otf");
}

body {
  align-items: center;
  background-color: #a8bfff;
  color: #4d4d4d;
  display: flex;
  font-family: sans-serif;
  max-width: 375px;
  height: 100vh;
  padding-right: 24px;
  padding-left: 24px;
}

h1 {
  font-family: "DDCHardware-Condensed";
  font-size: 64px;
  line-height: 64px;
  margin-left: -5px;
  margin-bottom: 16px;
}

#description {
  font-family: "DDCHardware-Compressed";
  font-size: 24px;
  line-height: 40px;
  margin: 32px 0 32px 0;
}

#links {
  font-size: 16px;
  line-height: 32px;
  font-family: "DDCHardware-Condensed";
}

a {
  color: #f1f4ff;
  font-size: 24px;
  text-decoration: none;
}
</style>