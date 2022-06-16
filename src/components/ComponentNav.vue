<template>
  <nav>
    Nav clicked: {{ navCount }}
    <button>Count up</button>
  </nav>
</template>

<script>
export default {
  name: "ComponentNav",
  data() {
    return {
      navCount: 0
    };
  },
};
</script>
