<template>
  <div class="hello">
    <h1>Voor betere conversaties</h1>
    <h2>
      Straat Epistemologie (SE) is gespreksmethode om betere gesprekken te
      voeren over lastige onderwerpen.
    </h2>
    <p>Voor meer informatie over SE kunt u terecht bij de volgende bron:</p>
    <ul>
      <li>
        <a href="https://streetepistemology.com/" target="_blank" rel="noopener"
          >https://streetepistemology.com/</a
        >
      </li>
    </ul>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  props: {
    msg: String,
  },
})
export default class HelloWorld extends Vue {
  msg!: string;
}
</script>

<style scoped lang="scss">
h1 {
  margin: 40px 0 0;
  font-size: 30px;
}
h2 {
  margin: 20px 0 0;
  font-style: italic;
}
p {
  margin: 30px 0 0;
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
