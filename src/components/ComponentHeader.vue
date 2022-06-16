<template>
  <header> 
    Header clicked: {{ headerCount }} 
    <button> Count up </button>
    <ComponentNav />
  </header>
</template>

<script>
import ComponentNav from './ComponentNav.vue'

export default {
  name: "ComponentHeader",
  components: {
    ComponentNav
  },
  data() {
    return {
      headerCount: 0
    }
  }
};
</script>
