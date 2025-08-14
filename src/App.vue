<template>
  <div id="app">
    <button @click="isVisible = !isVisible">
      {{ isVisible ? 'Hide' : 'Show' }} Message
    </button>

    <p v-if="isVisible">
      🎉 Hello! You toggled me on.
    </p>
  </div>
</template>

<script>
export default {
  name: 'App',
  data(){
    return {
      isVisible: false
    }
  }
}
</script>
