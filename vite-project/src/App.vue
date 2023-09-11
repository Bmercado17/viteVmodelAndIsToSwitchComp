

<template>
  <select v-model="componentName">
    <option value="Home">Home</option>
    <option value="About">About</option>
  </select>
  <keep-alive>
    <component :is="componentName"></component>
  </keep-alive>
</template>

<!-- LogicVue -->
<script>
import Home from './components/Home.vue'
import About from './components/About.vue'
export default {
  name: 'App',
  components: {
    Home,
    About
  },
  data(){
    return{
      componentName: 'Home'
    }
  }
}
</script>
<style scoped>
.parent,.div1,.div2,.div3 {
display: flex;

background-color: orange;
display: grid;
grid-template-columns: repeat(3, 1fr);
grid-template-rows: repeat(2, 1fr);
grid-column-gap: 2.5px;
grid-row-gap: 3px;
}
</style>