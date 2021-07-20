<template>
  <div id="container">
    <div v-html="notes" />
  </div>
</template>

<script>
import notes from '@/assets/notes.md';

export default {
  name: 'HelloWorld',
  data() {
    return {
      notes
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h4 {
    max-width: 36em;
}
h5 {
    max-width: 54em;
}
h6 {
    max-width: 500px;
}

ul {
    list-style-type: none;
    position: relative;
    left: 1em;
}
li {
    max-width: 34em;
}
li>h5 {
    max-width: 74em;
}

#container {
    padding: 5vh 1vw;
    overflow: hidden;
}
</style>
