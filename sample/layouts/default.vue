<template>
  <div class="layout-default">
    <h1>layout-default</h1>
    <nuxt />
    <TheFirstModal />
    <TheSecondModal />
    <modal-portal />
  </div>
</template>

<script>
import TheFirstModal from '~/components/TheFirstModal.vue'
import TheSecondModal from '~/components/TheSecondModal.vue'

export default {
  components: {
    TheFirstModal,
    TheSecondModal,
  },
}
</script>
