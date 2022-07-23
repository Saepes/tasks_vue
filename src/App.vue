<template>
  {{ getDate() }}
</template>

<script>
export default {
  name: "App",

  methods: {
    getDate: () => {
      let date = new Date().toISOString().slice(0, 10);
      alert(date);
    },
  },
};
</script>
