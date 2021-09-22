<template>
  <div>
    <h2>ChildComponent2.vue</h2>
    <ChildComponent3 />
  </div>
</template>

<script>
import ChildComponent3 from "./ChildComponent3.vue";

export default {
  components: {
    ChildComponent3,
  },
};
</script>