<template>
  <div>
    <h1>Total Drama Island</h1>
    <div>
      <h2>Characters</h2>
      <table>
        <thead>
          <tr>
            <th>Name</th>
            <th>Bio</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="(character, index) in characters" :key="index">
            <td>{{character.name}}</td>
            <td>{{character.bio}}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<script lang="ts">

import characters from '../data/characters';

export default {
  name: 'CharacterList',
  data() {
    return {
      characters,
    };
  },
};

</script>

<style scoped>

h2 {
  text-align: left;
}

td, th {
  text-align: left;
  padding: 5px;
  padding-right: 20px;
}
</style>
