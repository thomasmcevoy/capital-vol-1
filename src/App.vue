<template>
  <div id="container">
    <div v-html="notes" />
  </div>
</template>

<script>
import notes from '/static/notes.md';

export default {
  name: 'App',
  data() {
    return {
      notes
    }
  }
}
</script>

<style>
*,*:before,*:after{
  box-sizing:border-box;
  font-feature-settings:"kern";
  -webkit-font-kerning:normal;
  font-kerning:normal;
  -moz-osx-font-smoothing:grayscale !important;
  -webkit-font-smoothing:antialiased !important
}

body {
  background-color: rgb(246, 246, 246);
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "Roboto", "Oxygen", "Ubuntu", "Cantarell", "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif;
}

#app {
  margin: 5vh 1vw;
}

#container {
  max-width: 1100px;
  margin: auto;
}

h1 {
  font-size: clamp(2rem, 5vw, 4rem);
  font-weight: 800;
}

h2 {
  font-size: clamp(.75rem, 1.75vw, 1.25rem);
  font-weight: 300;
  font-family: "Verdana", sans-serif;
  letter-spacing: .09em;
  text-transform: uppercase;
  color: rgb(102, 102, 102);
  margin: 3.5em auto 1.75em;
  border-bottom: solid thin rgb(102, 102, 102);
  padding-bottom: .18em;
}

h3 {
  font-size: clamp(1.25rem, 3.1vw, 2.5rem);
  font-weight: 800;
  margin: 0 auto .15em;
}

h4 {
  font-size: clamp(1.125rem, 2.33vw, 2rem);
  max-width: 36em;
  margin-bottom: 0;
}

h5 {
  font-size: clamp(1rem, 2vw, 1.6rem);
  max-width: 54em;
  margin-bottom: 0;
}

h6 {
  max-width: 500px;
}

ul {
  list-style-type: none;
  padding: 0;
  margin-top: 0;
}

li {
  color: rgb(70, 70, 70);
  font-family: "Georgia", "Garamond", "Times", serif;
  font-size: clamp(1.125rem, 2.15vw, 1.5rem);
  font-weight: 300;
  letter-spacing: .01em;
  line-height: 1.5em;
  max-width: 34em;
  margin-top: .5em;
}

li:first-child {
  margin-top: .2em;
}
li:last-child {
  margin-bottom: 2.5em;
}

li>h5 {
  color: rgb(0, 0, 0);
    max-width: 74em;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "Roboto", "Oxygen", "Ubuntu", "Cantarell", "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif;
}

em {
  color: rgb(34, 34, 34);
  font-style: italic;
  font-weight: 600;
}
</style>
