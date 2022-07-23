<template>
  <div>
    <p>
      {{ arr[0] }}
    </p>

    <p>
      {{ arr[1] }}
    </p>

    <p>
      {{ arr[2] }}
    </p>
  </div>

  <div>
    <p>Сумма чисел массива - {{ arr2[0] + arr2[1] + arr2[2] }}</p>
  </div>
</template>

<script>
export default {
  name: "App",

  data() {
    return {
      arr: ["x", "y", "z"],
      arr2: [1, 2, 3],
    };
  },
};
</script>
