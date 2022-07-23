<template>
  {{ getSum() }}
</template>

<script>
export default {
  name: "App",

  data() {
    return {
      num1: 1,
      num2: 2,
    };
  },

  methods: {
    getSum: function () {
      alert(this.num1 + this.num2);
    },
  },
};
</script>
