<template>
  <div class="menu">
    <a v-for="(item, i) in menus" :key="i">{{ item }}</a>
  </div>
  <div v-for="(item, index) in products" :key="index">
    <h4>{{ item }}원룸</h4>
    <p>{{ price1 }} 만원</p>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      price1: 60,
      price2: 70,
      menus: ["Home", "Products", "About"],
      products: ["역삼동원룸", "천호동원룸", "마포구원룸"],
    };
  },
  components: {},
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
.menu {
  background: darkslateblue;
  padding: 15px;
  border-radius: 5px;
}
.menu a {
  color: white;
  padding: 10px;
}
</style>
