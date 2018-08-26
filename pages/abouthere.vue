<template>
    <main>
        <nuxt-link to="/">back</nuxt-link>
        <h1>About this site</h1>
        <h2>The stack</h2>
        <p>My main objective was to create a personal page that utilizes server side rendering and has performance as a key feature. I wanted first meaningful paint to be around one second (or approximately a 99 Lighthouse score). I also wanted very low configuration and cognitive overhead when spinning the site up so I chose to build with Vue and Node using Nuxt.js. It's hosted on Netlify -- which I really can't recommend strongly enough.</p>
        <h2>The design</h2>
        <p>It's intentionally "workmanlike" in it's design and execution. This makes it simpler to maintain for me and I think quieter websites that communicate simply and effectively are beautiful. The typefaces are system fonts and the colors were chosen for accessibility.</p>
    </main>
</template>

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