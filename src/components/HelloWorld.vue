<template>
  <div>
    <h1>{{ msg }}</h1>
    <button @click="alertClick()">Contar</button>
    <p>{{ contador }}</p>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  data: () => ({
    contador: 0
  }),
  methods: {
    alertClick() {
      this.contador++
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
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
