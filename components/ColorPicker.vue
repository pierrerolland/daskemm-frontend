<template>
  <div>
    <h3>{{ title }}</h3>
    <v-color-picker hide-inputs v-model="local" />
  </div>
</template>

<script lang="ts">
  export default {
    model: 'value',
    props: {
      title: String,
      value: String
    },
    computed: {
      local: {
        get() { return this.value },
        set(local: string) {this.$emit('input', local)}
      }
    }
  }
</script>
