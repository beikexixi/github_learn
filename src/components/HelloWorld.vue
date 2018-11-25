<template>
  <div class="hello">
    <h1>哎哟喂</h1>
    <p>哈哈一哈哈</p>
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <el-rate
      v-model="value3"
      :texts="texts"
      @change="handleChange"
      show-text>
    </el-rate>
    <p>天下之大，无奇不有</p>
    <h1>世间万物，必有始终</h1>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      value3: null,
      texts: ['差', '较差', '一般', '满意', '非常满意']
    }
  },
  methods: {
    handleChange (score) {
      debugger
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
