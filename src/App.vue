<template>
  <div id="app">
    <h1>Where have you been?</h1>
    <USMap />
  </div>
</template>

<script>
import USMap from './components/USMap.vue';

export default {
  name: 'app',
  components: {
    USMap,
  }
}
</script>

<style>

#app {
  max-width: 959px;
  margin: 0 auto;
}

.state path,
.state circle {
  fill: #D5D9DE;
}
.state path:hover,
.state circle:hover {
  fill: #A0A5AB;
  cursor: pointer;
}
.state path.selected,
.state circle.selected {
  fill: #35B4C6;
}
</style>
