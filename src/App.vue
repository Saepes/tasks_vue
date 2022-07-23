<template>
  <div>
    <button @click="getDate">Кнопка</button>

    <button @mouseover="getDate">Кнопка</button>
  </div>
</template>

<script>
export default {
  name: "App",

  methods: {
    getDate: () => {
      let date = new Date().toISOString().slice(0, 10);
      return alert(date);
    },
  },
};
</script>
