<template>
    <div>
      <span class="count">{{ count }}</span>
      <button @click="increment">Increment</button>
    </div>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      Default: ''
    }
  },
  data () {
    return {
      count: 0
    }
  },

  methods: {
    increment () {
      this.count++
    }
  }
}
</script>
