<template>
  <div>
    <p>Сумма чисел объекта - {{ obj.x + obj.y + obj.z }}</p>
  </div>
</template>

<script>
export default {
  name: "App",

  data() {
    return {
      obj: { x: 1, y: 2, z: 3 },
    };
  },
};
</script>
