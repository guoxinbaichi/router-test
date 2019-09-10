<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <div class="row">
      <div class="col-xs-2 col-xs-offset-2">
        <div class="list-group">
          <!--使用指令v-link进行导航            最新版写法-->
          <router-link to="/home">Go to Foo</router-link>
          <router-link to="/about">Go to Bar</router-link>
            <!--用于渲染匹配的组件-->
          <router-view></router-view>
        </div>
      </div>
      <div class="col-xs-6">
        <div class="panel">
          <div class="panel-body">


          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
  },

}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
