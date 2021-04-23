<template>
  <div id="app">
    <button @click="visible = true">show</button>
    <button @click="visible = false">destroy</button>
    <sub-app v-if="visible"></sub-app>
  </div>
</template>

<script>
import subApp from './child_app'
export default {
  components: {
    subApp,
  },
  data() {
    return {
      visible: false
    }
  }
}
</script>
