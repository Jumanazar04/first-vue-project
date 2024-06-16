<template>
  <div class="counter container">
    <h1>{{ count }}</h1>
    <button class="btn btn-success" @click="increment">Increment</button>
    <button class="btn-danger btn " @click="decrement">Decrement</button>
    <button class="btn btn-primary" @click="reset">Reset</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    increment() {
      this.count++;
    },
    decrement() {
      this.count--;
    },
    reset() {
      this.count = 0;
    },
  },
};
</script>