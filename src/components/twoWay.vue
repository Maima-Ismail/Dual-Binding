<template>
  <div>
    <h2>Two-Way Binding with Buttons</h2>
    <p>Counter: {{ counter }}</p>
    <button @click="increment">Increment</button>
    <button @click="decrement">Decrement</button>
    <button @click="reset">Reset</button>
    <br />
    <input type="number" v-model="counter" />
  </div>
</template>

<script>
export default {
  name: 'twoWay',
  data() {
    return {
      counter: 0, // This data property will hold the counter value
    }
  },
  methods: {
    increment() {
      this.counter++
    },
    decrement() {
      this.counter--
    },
    reset() {
      this.counter = 0
    },
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h2 {
  margin-bottom: 10px;
}
p {
  margin-top: 10px;
}
button {
  margin-right: 10px;
  padding: 8px 16px;
  font-size: 16px;
  cursor: pointer;
}
input {
  margin-top: 10px;
  padding: 8px;
  font-size: 16px;
}
</style>
