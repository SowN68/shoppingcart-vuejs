<template>
  <NavBar />
  <menu-list></menu-list>
</template>

<script>
import MenuList from './components/menu/MenuList.vue';
import NavBar from './components/navigation/NavBar.vue';

export default {
  name: 'App',
  components: {
    MenuList,
    NavBar
  }
}
</script>

<style>
*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
button{
  cursor:pointer
}
#app{
  width: 100%;
}
</style>
