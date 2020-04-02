<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script lang="ts">
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  methods: {
    person (name:string) {
      return 'hello' + name
    }
  },
  mounted () {
    interface SquareConfig {
        color: string;
        area: number;
    }

    function createSquare(config: SquareConfig): { color: string; area: number } {
      let newConfig = {color: 'red', area: 100}
      newConfig.color = config.color
      newConfig.area = config.area
      return newConfig
    }

    let mySquare = createSquare({ color: "red", area: 100 });
    console.log(mySquare)
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
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
