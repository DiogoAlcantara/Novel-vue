<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <Editor />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { Editor } from 'novel-vue';
import 'novel-vue/dist/style.css';

export default defineComponent({
  name: 'HelloWorld',
  components: {
    Editor, // Adicionando o componente Editor como um componente filho
  },
  props: {
    msg: String,
  },
});
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
