<template>
  <div>
    <h2>ChildComponent4.vue</h2>
    <button @click="updateParent(Math.random())">
      Update parent value in App.vue
    </button>
  </div>
</template>

<script>
export default {
  inject: ["updateParent"],
};
</script>