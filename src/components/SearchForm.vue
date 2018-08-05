<template>
<div>
  <div class="field">
      <input class="input" v-model="fromCity" type="text" placeholder="From">
  </div>
  <div class="field">
      <input class="input" v-model="toCity" type="text" placeholder="To">
  </div>
  <div class="field">
      <button class="button is-success">
        Login
      </button>
  </div>
</div>
</template>

<script>
export default {
  data () {
    return {
        fromCity: "",
        toCity: ""
    }
  }
}
</script>

<style lang="scss" scoped>

input, button {
  font-family: 'C64';
}

</style>
