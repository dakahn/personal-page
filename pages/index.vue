<template>
      <main>
        <h1>Cool, hi. I'm @dakahn.</h1>
        <section id="description">I'm a web developer, an advocate for accessibility online, an outspoken enemy of needless complexity, and a musician.</section>
        <ul>
          <li><a href="https://github.com/dakahn">Github</a></li>
          <li><a href="https://medium.com/@dakahn">Medium</a></li>
          <li><a href="https://codepen.io/dakahn/#">Codepen</a></li>
          <li><a href="https://stackoverflow.com/users/9963925/dak">Stack Overflow</a></li>
          <li><a href="https://www.linkedin.com/in/daanguiano/">Linkedin</a></li>
          <li><a href="https://soundcloud.com/user-740902594">Soundcloud</a></li>
          <li><nuxt-link to="/abouthere">About this site</nuxt-link></li>
        </ul>
      </main>
</template>
<script>
export default {
  head() {
    return {
      title: "dakahn.netlify.com - Home",
      meta: [
        {
          hid: "description",
          name: "description",
          content: "The landing page for D.A. Kahn's personal site."
        }
      ]
    };
  }
};
</script>

<style>
body {
  color: #4d4d4d;
  background-color: #cddcdc;
  background-image: radial-gradient(
      at 50% 100%,
      rgba(255, 255, 255, 0.5) 0%,
      rgba(0, 0, 0, 0.5) 100%
    ),
    linear-gradient(
      to bottom,
      rgba(255, 255, 255, 0.25) 0%,
      rgba(0, 0, 0, 0.25) 100%
    );
  background-blend-mode: screen, overlay;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
    Oxygen-Sans, Ubuntu, Cantarell, "Helvetica Neue", sans-serif;
  min-height: 100vh;
  padding-right: 8px;
  padding-left: 8px;
}

h1 {
  font-size: 48px;
  line-height: 58px;
  margin-left: -5px;
  margin-bottom: 16px;
}

#description {
  font-size: 26px;
  margin: 32px 0 32px 0;
}

ul {
  font-size: 18px;
  list-style-position: inside;
  line-height: 32px;
  margin: 0;
  padding: 0;
}

a {
  color: #551a8b;
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