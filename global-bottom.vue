<!-- global-bottom.vue -->
<template>
  <footer class="absolute bottom-0 left-0 right-0 p-2">
    <small>
      <span class="mv">Modern Vue</span>
      ( <a style="font-style: italic;" href="https://businessof.technology" target="_blank">by Business of Technology</a>
      &nbsp;<line-md:computer-twotone /> )
    </small>

  </footer>
</template>

<!-- https://icones.js.org/ -->

<style>
ol.toc {
  list-style-type: disc !important;
}

ol.toc ol.toc {
  list-style-type: circle !important;
}

h1 .mv {
  background-color: #1b7026;
  background-image: linear-gradient(45deg, #4ed46b 20%, #148c2e 50%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}

h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 20%, #146b8c 50%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}

.translucent {
  color: rgba(200, 200, 200, .3);
}

footer .mv {
  background-color: #1b7026;
  background-image: linear-gradient(45deg, #4ed46b 7%, #148c2e 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}

footer {
  text-align: right;
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 7%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>
