<template>
  <div>
    User id:
    <v-text-field v-model="id"></v-text-field>
    <v-btn @click="loadUser">
      goto
    </v-btn>
  </div>
</template>

<script>
export default {
  data() {
    return {
      id: ''
    }
  },
  methods:{
    loadUser() {
      this.$router.push(`/users/${this.id}`)
    }
  }
}
</script>

<style>

</style>