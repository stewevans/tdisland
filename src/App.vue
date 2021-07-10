<template>
  <div id="app">
    <CharacterList />
  </div>
</template>

<script lang="ts">
import CharacterList from './components/CharacterList.vue';

export default {
  components: {
    CharacterList,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
