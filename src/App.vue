<template>
Number 1: <input v-model.number="number1" type="text">
Number 2: <input v-model.number="number2" type="text">
<button v-on:click='add'>+</button>
<button v-on:click='substract'>-</button>
<button v-on:click='multiply'>*</button>
<button v-on:click='divide'>/</button>
Result: {{result}}
</template>

<script>

export default {
  name: 'App',
  data () {
    return{
      number1: 0,
      number2: 0,
      result: 0
    }
  },
  methods: {
    add () {
      this.result = this.number1 + this.number2
    },
    substract () {
      this.result = this.number1 - this.number2
    },
    multiply () {
      this.result = this.number1 * this.number2
    },
    divide () {
      this.result = this.number1 / this.number2
    }
}
}
</script>

<style>
</style>
