
<template>
<html lang="en">
  <main>
    <head>
      <title>An introduction to Accessibility</title>
    </head>
    <h1>An introduction to Accessibility</h1>
    <h2>What is web accessibility?</h2>
    <p>(borrowing heavily from Todd Liebsch from Deque) "Designing and developing for the web so that people with disabilities can perceive, understand, navigate, interact, and contribute without barriers or added frustration."</p>
    <h2>What do we mean by "people with disabilities"?</h2>
    <p>When it comes to the web there are four main categories. Remember that each category is a spectrum of ability.</p>
    <h3
      id="ul-label"
    >Categories of people with disabilities on the web and some of the tools they use</h3>
    <ul aria-labelledby="ul-label">
      <li>visual - magnifiers, braille devices, screen readers</li>
      <li>auditory - closed captioning, subtitling</li>
      <li>motor - sip and puff, mouth stick, single switch</li>
      <li>cognitive - increased line height, letter spacing, assistive fonts</li>
    </ul>

    <h2>How many potential users with disabilities are there?</h2>
    <p>
      According to the
      <a
        href="https://www.who.int/disabilities/world_report/2011/report/en/"
      >WHO World Report on Accessibility</a> roughly 15% (approx. 1 billion) of the worlds population are experiencing a disability making them the world's largest minority.
    </p>
    <p>
      According to the
      <a
        href="https://www.cdc.gov/media/releases/2018/p0816-disability.html"
      >Center for Disease Control's statistics</a> 61 million or 1 in 4 American adults are living with a disability.
    </p>
    <h2>The state of web accessibility</h2>
    <p>
      In February of 2019 Webaim
      <a
        href="https://webaim.org/projects/million/"
      >surveyed the top 1,000,000 most visited websites</a> for accessibility errors and found:
    </p>
    <ul>
      <li>97.8% of sites had detectable accessibility errors</li>
      <li>The average homepage contained 59.6 detectable accessibility errors</li>
      <li>Users with disabilities can expect to encounter a detectable error on 1 in every 13 elements on the page</li>
    </ul>
    <h2>What are some misconceptions about accessibility?</h2>
    <ul>
      <li>
        <span class="bold">"I don't have users with disabilities".</span> Aside from the wild assumption that the 0 of the 1 billion people living with disabilities will never come into contact with your application/website consider that you yourself will someday be the user of an accessibility affordance as you age.
      </li>
      <li>
        <span class="bold">Accessibility is a nice-to-have feature for post-mvp.</span> The expectation is that your website is usable, accessible, and WCAG compliant at launch. Integrate accessibility as a practice into every stage of your design and development -- from early ideation to release.
      </li>
      <li>
        <span class="bold">My automated tooling (Stark, DAP, Axe) will find any problems I have.</span>The very best automated tooling we have is capable of catching at best approximately
        <a
          href="https://accessibility.blog.gov.uk/2017/02/24/what-we-found-when-we-tested-tools-on-the-worlds-least-accessible-webpage/"
        >40% of accessibility errors.</a>
      </li>
    </ul>
    <h2>How do we make sure our products are accessible?</h2>
    <p>
      Accessibility requirements at IBM are based on the
      <a
        href="https://www.w3.org/TR/WCAG21/"
      >Web Content Accessibility Guidelines (WCAG)</a>; With a three pronged attack for auditing components/sites called Accessibility Verification Tests (AVT):
    </p>
    <ul>
      <li>
        AVT1 - automated testing with
        <a
          href="https://www.ibm.com/able/dynamic-assessment-plug-in.html"
        >The Dynamic Accessibility Plugin (DAP).</a>
      </li>
      <li>AVT2 - keyboard testing, all mouse functionality must have a corresponding keyboard control</li>
      <li>AVT3 - screen reader testing using JAWS on Windows and VoiceOver on macOS</li>
    </ul>
    <p>Although it can take time to master, integrating these checks seamlessly into your workflow should be the end goal.</p>
    <p>
      That said, true usability and accessibility can only come from direct contribution and direct collaboration with users with disabilities.
      <a
        href="https://www.ibm.com/blogs/age-and-ability/tag/team-able/"
      >IBM's Team Able</a> are volunteer users with disabilities who can provide valuable and insightful feedback, test usability/accessibility assumptions on prototypes and projects. 🤙♿
    </p>
  </main>
</html>
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

.bold {
  font-weight: bold;
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
