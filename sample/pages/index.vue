<template>
  <div class="page-index">
    <h2>page-index</h2>
    <ul>
      <li>
        <nuxt-link to="/another">page-another</nuxt-link>
      </li>
    </ul>
    <button @click="openFirstModal">openFirstModal</button>
  </div>
</template>

<script>
export default {
  methods: {
    async openFirstModal() {
      await this.$store.dispatch('modal/openFirstModal')
    },
  },
}
</script>
