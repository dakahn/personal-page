<template>
    <div>
        <h1>Cool, hi. My name is D.A. Kahn.</h1>
        <p id="description">I'm a JavaScript developer working for IBM Design in Austin, Texas.💀<p>
        <p id="links">Check out my <span><a href="https://github.com/dakahn">Github</a></span> for code and projects I'm contributing to. Zip on over to my <span><a href="https://www.linkedin.com/in/daanguiano/">LinkedIn</a></span> profile for some background and to get in touch. To read stuff I've written on the topic of professionally programming computers see my <span><a href="https://medium.com/@dakahn">Medium</a></span>.
        </p>
    </div>
</template>

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
  background-color: #a8bfff;
  color: #4d4d4d;
  height: 100vh;
  padding-right: 8px;
  padding-left: 8px;
}

h1 {
  font-size: 72px;
  font-family: "DDCHardware-Condensed";
  line-height: 64px;
  margin-left: -5px;
  margin-bottom: 16px;
}

#description {
  font-family: "DDCHardware-Condensed";
  font-size: 32px;
  line-height: 40px;
  margin: 32px 0 32px 0;
}

#links {
  font-size: 24px;
  line-height: 32px;
  font-family: "DDCHardware-Condensed";
}

#ibm-link {
  font-size: 42px;
}

a {
  color: #f1f4ff;
  font-size: 32px;
  text-decoration: none;
}

a:hover {
  background-color: #4d4d4d;
}

@media (min-width: 620px) {
  body {
    display: flex;
    align-items: center;
    margin-left: 32px;
    margin-right: 32px;
    max-width: 570px;
  }
}
</style>