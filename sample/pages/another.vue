<template>
  <div class="page-another">
    <h2>page-another</h2>
    <ul>
      <li>
        <nuxt-link to="/">page-index</nuxt-link>
      </li>
    </ul>
    <button @click="openSecondModal">openSecondModal</button>
  </div>
</template>

<script>
export default {
  layout: 'another',

  methods: {
    openSecondModal() {
      this.$modal.push('the-second-modal')
    },
  },
}
</script>
