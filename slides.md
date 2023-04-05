---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: /img/background.jpg
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
# page transition
transition: slide-left
# use UnoCSS
css: unocss
title: Modern Vue - Complete
level: 1
---

<SendKey :slide="$slidev.nav.currentPage" keys="t"/>

[__add slide for "Ways of using Vue"__](https://vuejs.org/guide/extras/ways-of-using-vue.html)

# <span class="mv" id="begin">Modern <logos-vue />ue</span>: Complete

How will Vue influence your future today?

<div class="abs-br m-6 flex gap-2">
  <a href="https://github.com/BOT-TC/mv_main" target="_blank" alt="GitHub"
    class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
transition: slide-left
hideInToc: true
---

# Table of Contents

<Toc mode="all" columns="2" maxDepth="1" />

<style>
h1 {
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
}
</style>

---
transition: slide-left
title: What will we learn?
level: 1
---

# What We Will Learn?

Our goal is to give you a full tool box. When you get ready to use the material on a job or a project of your own
making, these courses are designed to give you a foundation to execute your vision.

- **[Vue 3](https://vuejs.org/)** - The Progressive JavaScript Framework
- **[Devtools](https://vuejs.org/guide/scaling-up/tooling.html#browser-devtools)** - Explore Vue inside out during dev.
- **[Pinia](https://pinia.vuejs.org/)** - Type Safe, Extensible, and Modular by design.
- **[Slidev](https://sli.dev/)** - Presentation Slides for Developers
- **[TypeScript](https://www.typescriptlang.org/)** - Better tooling and more reliable code.
- **[Router](https://router.vuejs.org/)** - Expressive, configurable and convenient routing
- **[VitePress](https://vitepress.dev/)** - Static Site Generator, Documentation
- **[VueUse](https://vueuse.org/)** - Collection of Essential Vue Composition Utilities

<br>
<br>

<small class="translucent">Courses built with [OLS](https://businessof.technology/ols)</small>

<!--
You can have `style` tag in markdown to override the style for the current page.
Learn more about slides: https://sli.dev/guide/syntax#embedded-styles
-->

<style>
h1 {
  background-image: linear-gradient(45deg, #4EC5D4 15%, #146b8c 30%);
}
</style>

<!--
Here is another comment.
-->

---
src: ./pages/course-collections.md
---

---
layout: cover
background: '/img/background.jpg'
hideInToc: true
hide: true
---

<h1><span class="bot-b">Business</span> <span class="bot-o">of</span> <span class="bot-t">Technology</span></h1>

How will Vue influence your future today?

<style>
  @import url("https://fonts.googleapis.com/css?family=Sacramento&display=swap");

h1 .bot-b{
  font-size: calc(20px + 6vh);
  line-height: calc(20px + 8vh);
/*   text-shadow: 0 0 5px #f562ff, 0 0 15px #f562ff, 0 0 25px #f562ff,
    0 0 20px #f562ff, 0 0 30px #890092, 0 0 80px #890092, 0 0 80px #890092;
  color: #fccaff; */
  text-shadow: 0 0 5px #ff6500, 0 0 15px #ff6500, 0 0 20px #ff6500, 0 0 40px #ff6500, 0 0 60px #ff0000, 0 0 10px #ff2d00, 0 0 98px #ff0000;
    color: #ff0000;
  font-family: "Sacramento", cursive;
  text-align: center;
  animation: blink 12s infinite;
  -webkit-animation: blink 12s infinite;
}
h1 .bot-o{
  font-size: calc(20px + 6vh);
  line-height: calc(20px + 8vh);
/*   text-shadow: 0 0 5px #f562ff, 0 0 15px #f562ff, 0 0 25px #f562ff,
    0 0 20px #f562ff, 0 0 30px #890092, 0 0 80px #890092, 0 0 80px #890092;
  color: #fccaff; */
  text-shadow: 0 0 5px #00ff65, 0 0 15px #00ff65, 0 0 20px #00ff65, 0 0 40px #00ff65, 0 0 60px #00ff00, 0 0 10px #00ff2d, 0 0 98px #ff0000;
    color: #00ff00;
  font-family: "Sacramento", cursive;
  text-align: center;
  animation: blink 12s infinite;
  -webkit-animation: blink 12s infinite;
}
h1 .bot-t{
  font-size: calc(20px + 6vh);
  line-height: calc(20px + 8vh);
/*   text-shadow: 0 0 5px #f562ff, 0 0 15px #f562ff, 0 0 25px #f562ff,
    0 0 20px #f562ff, 0 0 30px #890092, 0 0 80px #890092, 0 0 80px #890092;
  color: #fccaff; */
  text-shadow: 0 0 5px #0065ff, 0 0 15px #0065ff, 0 0 20px #0065ff, 0 0 40px #0065ff, 0 0 60px #0000ff, 0 0 10px #002dff, 0 0 98px #0000ff;
    color: #0000ff;
  font-family: "Sacramento", cursive;
  text-align: center;
  animation: blink 12s infinite;
  -webkit-animation: blink 12s infinite;
}

@-webkit-keyframes blink .bot-b{
  20%,
  24%,
  55% {
    color: #111;
    text-shadow: none;
  }

  0%,
  19%,
  21%,
  23%,
  25%,
  54%,
  56%,
  100% {
/*     color: #fccaff;
    text-shadow: 0 0 5px #f562ff, 0 0 15px #f562ff, 0 0 25px #f562ff,
      0 0 20px #f562ff, 0 0 30px #890092, 0 0 80px #890092, 0 0 80px #890092; */
  text-shadow: 0 0 2px #ff6500, 0 0 6px #ff6500, 0 0 8px #ff6500, 0 0 16px #ff6500, 0 0 18px #ff0000, 0 0 4px #ff2d00, 0 0 40px #ff0000;
    color: #ff0000;
  }
}
@-webkit-keyframes blink .bot-o{
  20%,
  24%,
  55% {
    color: #111;
    text-shadow: none;
  }

  0%,
  19%,
  21%,
  23%,
  25%,
  54%,
  56%,
  100% {
/*     color: #fccaff;
    text-shadow: 0 0 5px #f562ff, 0 0 15px #f562ff, 0 0 25px #f562ff,
      0 0 20px #f562ff, 0 0 30px #890092, 0 0 80px #890092, 0 0 80px #890092; */
  text-shadow: 0 0 2px #65ff00, 0 0 6px #65ff00, 0 0 8px #65ff00, 0 0 16px #65ff00, 0 0 18px #00ff00, 0 0 4px #2dff00, 0 0 40px #00ff00;
    color: #00ff00;
  }
}
@-webkit-keyframes blink .bot-t{
  20%,
  24%,
  55% {
    color: #111;
    text-shadow: none;
  }

  0%,
  19%,
  21%,
  23%,
  25%,
  54%,
  56%,
  100% {
/*     color: #fccaff;
    text-shadow: 0 0 5px #f562ff, 0 0 15px #f562ff, 0 0 25px #f562ff,
      0 0 20px #f562ff, 0 0 30px #890092, 0 0 80px #890092, 0 0 80px #890092; */
  text-shadow: 0 0 2px #0065ff, 0 0 6px #0065ff, 0 0 8px #0065ff, 0 0 16px #0065ff, 0 0 18px #0000ff, 0 0 4px #2d00ff, 0 0 40px #0000ff;
    color: #0000ff;
  }
}

@keyframes blink .bot-b{
  20%,
  24%,
  55% {
    color: #111;
    text-shadow: none;
  }

  0%,
  19%,
  21%,
  23%,
  25%,
  54%,
  56%,
  100% {
/*     color: #fccaff;
    text-shadow: 0 0 5px #f562ff, 0 0 15px #f562ff, 0 0 25px #f562ff,
      0 0 20px #f562ff, 0 0 30px #890092, 0 0 80px #890092, 0 0 80px #890092; */
  text-shadow: 0 0 2px #ff4500, 0 0 6px #ff4500, 0 0 8px #ff4500, 0 0 16px #ff4500, 0 0 18px #ff0000, 0 0 4px #ff2500, 0 0 40px #ff0000;
    color: #ff0000;
  }
}
@keyframes blink .bot-o{
  20%,
  24%,
  55% {
    color: #111;
    text-shadow: none;
  }

  0%,
  19%,
  21%,
  23%,
  25%,
  54%,
  56%,
  100% {
/*     color: #fccaff;
    text-shadow: 0 0 5px #f562ff, 0 0 15px #f562ff, 0 0 25px #f562ff,
      0 0 20px #f562ff, 0 0 30px #890092, 0 0 80px #890092, 0 0 80px #890092; */
  text-shadow: 0 0 2px #00ff45, 0 0 6px #00ff45, 0 0 8px #00ff45, 0 0 16px #00ff45, 0 0 18px #ff0000, 0 0 4px #00ff25, 0 0 40px #ff0000;
    color: #00ff00;
  }
}
@keyframes blink .bot-t{
  20%,
  24%,
  55% {
    color: #111;
    text-shadow: none;
  }

  0%,
  19%,
  21%,
  23%,
  25%,
  54%,
  56%,
  100% {
/*     color: #fccaff;
    text-shadow: 0 0 5px #f562ff, 0 0 15px #f562ff, 0 0 25px #f562ff,
      0 0 20px #f562ff, 0 0 30px #890092, 0 0 80px #890092, 0 0 80px #890092; */
  text-shadow: 0 0 2px #0045ff, 0 0 6px #0045ff, 0 0 8px #0045ff, 0 0 16px #0045ff, 0 0 18px #0000ff, 0 0 4px #2500ff, 0 0 40px #0000ff;
    color: #0000ff;
  }
}
</style>
