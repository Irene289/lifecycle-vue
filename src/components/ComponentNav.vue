<template>
  <nav ref="nav">
    Nav clicked: {{ navCount }}
    <button @click.stop="onCountUpClicked">Count up</button>
  </nav>
</template>

<script>
export default {
  name: "ComponentNav",
  data() {
    return {
      navCount: 0,
    };
  },
  methods: {
    onCountUpClicked() {
      this.navCount++;
    },
  },
  beforeCreate() {
    console.group("=== beforeCreate nav ===");
    console.log(this.$el);
    console.log(this.$refs.nav);
  },
  created() {
    console.group("=== created nav ===");
    console.log(this.$el);
    console.log(this.$refs.nav);
  },
  beforeMount() {
    console.group("=== beforeMount nav ===");
    console.log(this.$el);
    console.log(this.$refs.nav);
  },
  mounted() {
    console.group("=== mounted nav ===");
    console.log(this.$el);
    console.log(this.$refs.nav);
  },
  beforeUpdate() {
    console.group("=== beforeUpdate nav ===");
    console.log(this.$el);
    console.log(this.$refs.nav);
  },
  updated() {
    console.group("=== updated nav ===");
    console.log(this.$el);
    console.log(this.$refs.nav);
  },
  beforeDestroy() {
    console.group("=== beforeDestroy nav ===");
    console.log(this.$el);
    console.log(this.$refs.nav);
  },
  destroyed() {
    console.group("=== destroyed nav ===");
    console.log(this.$el);
    console.log(this.$refs.nav);
  },
};
</script>

<style scoped>
  nav {
    margin: 1rem;
  }
</style>