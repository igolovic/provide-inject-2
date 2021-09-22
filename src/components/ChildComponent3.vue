<template>
  <div>
    <h2>ChildComponent3.vue</h2>
    <ChildComponent4 />
  </div>
</template>

<script>
import ChildComponent4 from "./ChildComponent4.vue";

export default {
  components: {
    ChildComponent4,
  },
};
</script>