<template>
  <component-to-re-render :key="componentKey" />
</template>

<script>
export default {
  data() {
    return {
      componentKey: 0,
    };
  },
  methods: {
    forceRerender() {
      this.componentKey += 1;  
    }
  }
}
</script>
