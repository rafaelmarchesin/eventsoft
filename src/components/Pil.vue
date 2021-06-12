<template>
  <div>
      <span>Nome: {{ name }}</span><br>
      <span>Idade: {{ age }}</span><br><br>
  </div>
</template>

<script>
export default {
    props: ['name', 'age']
}
</script>

<style>

</style>