<template>
  <modal name="the-first-modal">
    <div class="the-first-modal">
      <strong>the-first-modal</strong>
      <button @click="onClick">close and goto "/another"</button>
    </div>
  </modal>
</template>

<script>
export default {
  methods: {
    onClick() {
      const pop = () => this.$modal.pop()
      this.$router.push('/another', pop, pop)
    },
  },
}
</script>
