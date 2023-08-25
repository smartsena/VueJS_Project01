<template>
  <HeaderProject v-if="showflag"/>
  <HeaderProject v-show="showflag"> </HeaderProject>
  <div v-show="showName">
    <b>Usuário: </b>{{firstName + " " + lastName}}
  </div>
  <div v-if="accessLevel === 'admin'"> Conectado como Admin</div>
  <div v-else-if="accessLevel === 'logado'"> Usuário logado</div>
  <div v-else> Login não efetuado</div>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
</template>

<script>
import HeaderProject from './components/HeaderProject.vue';
import HelloWorld from './components/HelloWorld.vue';

export default {
  name: 'App',
  components: {
    HeaderProject,
    HelloWorld,
  },
  data() {
    return{
      showflag: true,
      firstName: 'Ziralda',
      lastName: 'Lafayette',
      showName: true,
      accessLevel: 'admin' //'logado' 'naoLogado'
    }
  },
}
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
