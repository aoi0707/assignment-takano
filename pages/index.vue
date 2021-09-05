<template>
  <div>
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  components: {}
});
</script>

<style>
body,
h1,
h2,
h3,
h4,
h5,
h6,
p,
div {
  margin: 0px;
  padding: 0px;
}
html {
  font-size: 2.66667vw;
}
.section-inners {
  padding: 7rem 2rem;
}
li {
  list-style: none;
}
@media screen and (min-width: 768px) {
  html {
    font-size: 62.5%;
  }
  body {
    min-width: 108rem;
    font-family: "Lato", "Noto Sans JP", sans-serif;
  }
  .section-inner {
    max-width: 128rem;
    padding: 8rem 4rem;
    margin-right: auto;
    margin-left: auto;
  }
}
</style>
