<template>
  <main>
    <h1>Cool, hi. I'm @dakahn.</h1>
    <section
      id="description"
    >I'm a web developer, an advocate for accessibility online, an outspoken enemy of needless complexity, and a musician.</section>
    <section class="links">
      <ul>
        <li>
          <a href="https://github.com/dakahn">Github</a>
        </li>
        <li>
          <a href="https://www.linkedin.com/in/daanguiano/">Linkedin</a>
        </li>
        <li>
          <nuxt-link to="/abouthere">About this site</nuxt-link>
        </li>
      </ul>
      <div alt="A caricature of me in a cowboy hat." title="Howdy!" id="caricature"></div>
    </section>
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
  height: 100vh;
  padding-right: 8px;
  padding-left: 8px;
  margin: 0;
}

#caricature {
  height: 144px;
  width: 144px;
  background: url(~/static/caricature.svg);
  background-size: 144px 144px;
  margin-top: 2rem;
  margin-left: -4px;
}

h1 {
  font-size: 48px;
  line-height: 58px;
  margin-left: -5px;
  margin-top: 0;
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