<template>
  <div>
    <p>Квадрат числа - {{ num * num }}</p>
    <p>Сумма чисел - {{ num1 + num2 + num3 }}</p>
  </div>
</template>

<script>
export default {
  name: "App",

  data() {
    return {
      num: 5,
      num1: 1,
      num2: 2,
      num3: 3,
    };
  },
};
</script>
