<template>
  <header ref="header">
    Header clicked: {{ headerCount }}
    <button @click.stop="onCountUpClicked">Count up</button>
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
  },
  methods: {
    onCountUpClicked() {
      this.headerCount ++
    }
  },
  beforeCreate () {
    console.group('=== beforeCreate header ===')
    console.log(this.$el)
    console.log(this.$refs.header)
  },
  created () {
    console.group('=== created header ===')
    console.log(this.$el)
    console.log(this.$refs.header)
  },
  beforeMount () {
    console.group('=== beforeMount header ===')
    console.log(this.$el)
    console.log(this.$refs.header)
  },
  mounted () {
    console.group('=== mounted header ===')
    console.log(this.$el)
    console.log(this.$refs.header)
  },
  beforeUpdate () {
    console.group('=== beforeUpdate header ===')
    console.log(this.$el)
    console.log(this.$refs.header)
  },
  updated () {
    console.group('=== updated header ===')
    console.log(this.$el)
    console.log(this.$refs.header)
  },
  beforeDestroy () {
    console.group('=== beforeDestroy header ===')
    console.log(this.$el)
    console.log(this.$refs.header)
  },
  destroyed () {
    console.group('=== destroyed header ===')
    console.log(this.$el)
    console.log(this.$refs.header)
  }
};
</script>
