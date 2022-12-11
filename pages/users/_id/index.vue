<template>
  <div>
    User: {{this.$route.params.id}}
  </div>
</template>

<script>
export default {
  validate(context) {
    return (/\d+$/g).test(context.params.id);
  }
}
</script>

<style>

</style>