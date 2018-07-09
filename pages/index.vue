<template>
    <div>
        <h1>My name<br>is D.A. Kahn.</h1>
        <p id="description">I'm a <strong>JavaScript developer</strong> working for IBM Design in Austin, Texas.</p>
        <hr>
        <p>Check out my <span><a href="/">Github</a></span> for code and to see the kinds of projects that interest me. Head to my <span><a href="/">LinkedIn</a></span> to get in touch or read what I've written on my <span><a href="/">Medium</a></span>. 💛
        </p>
    </div>
</template>

<style>
body {
  align-items: center;
  background-image: linear-gradient(to top, #d299c2 0%, #fef9d7 100%);
  background-blend-mode: screen;
  color: #555;
  display: flex;
  font-family: sans-serif;
  height: 100vh;
  max-width: 540px;
  padding-right: 24px;
  padding-left: 24px;
}

h1 {
  font-size: 64px;
  line-height: 72px;
}

hr {
  font-size: 32px;
}

#description {
  font-size: 28px;
}

p {
  font-size: 20px;
  line-height: 40px;
}

a {
  color: #db7093;
  font-size: 24px;
  font-weight: bold;
}
</style>