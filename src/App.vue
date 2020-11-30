<template>
  <div id="app">
    <div id="nav">
      <router-link to="/" v-slot="{ href, navigate }">
        <el-link :href="href" type="primary" @click="navigate">Home</el-link>
      </router-link> | 
      <router-link to="/about" v-slot="{ href, navigate }">
        <el-link :href="href" type="info" @click="navigate">About</el-link>
      </router-link>
    </div>
    <router-view />
  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
