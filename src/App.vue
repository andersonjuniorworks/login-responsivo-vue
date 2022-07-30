<template>
  <div id="app">
    <Login />
  </div>
</template>

<script>
import Login from './components/Login.vue';

export default {
  name: 'App',
  components: {
    Login,
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400;500;600;700;800;900&display=swap');

* {
  font-family: 'Poppins', sans-serif;
}

body {
  margin: 0;
  padding: 0;
  box-sizing: content-box;
}
</style>
