<template>
  <h1>My name is {{name}}, and I am {{age}} years old.</h1>
</template>

<script>
import {ref} from "vue";

export default {
  setup() {
    const name = ref('Bob');
    const age = ref(99);

    return {
      name,
      age
    }
  }

}
</script>

<style>

</style>
