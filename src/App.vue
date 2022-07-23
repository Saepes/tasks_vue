<template>
  <div>
    <p>Имя - {{ name }}</p>
  </div>

  <div>
    <p>Фамилия - {{ surn }}</p>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      name: 'John',
      surn: 'smit',
    }
  }
}
</script>
