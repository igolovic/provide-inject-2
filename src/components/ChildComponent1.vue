<template>
  <div>
    <h2>ChildComponent1.vue</h2>
    <ChildComponent2 />
  </div>
</template>

<script>
import ChildComponent2 from "./ChildComponent2.vue";

export default {
  components: {
    ChildComponent2,
  },
};
</script>