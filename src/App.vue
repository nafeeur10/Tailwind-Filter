<template>
  <div id="app" class="h-screen bg-gray-200">
    <CustomFilter />
  </div>
</template>

<script>
import CustomFilter from './components/CustomFilter.vue'

export default {
  name: 'App',
  components: {
    CustomFilter
  }
}
</script>
