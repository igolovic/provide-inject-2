<template>
  <h2>App.vue, parentValue is: <em>{{ parentValue }}</em></h2>
  <ChildComponent1 />
</template>

<script>
import ChildComponent1 from "./components/ChildComponent1.vue";

export default {
  data() {
    return {
      parentValue: "",
    };
  },
  components: {
    ChildComponent1,
  },
  provide() {
    return {
      updateParentValueEvent: this.updateParentValue,
    };
  },
  methods: {
    updateParentValue($value) {
      this.parentValue = $value;
    },
  },
};
</script>

<style>
html {
  font-family: "Roboto", sans-serif;
  background-color: gainsboro;
}

body {
  margin: 0;
}

div {
  border: blue 1px solid;
  padding: 10px;
}

h2 em{
  color: blue;
}
</style>