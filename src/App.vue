<template>
  <div>
    <p>{{ text }}</p>
    <button @click="changeProps()">Кнопка</button>
  </div>

  <div>
    <button @click="changePropsBtn()">Кнопка 1</button>
    <button @click="changePropsBtn2()">Кнопка 2</button>
    <p>{{ text2 }}</p>
  </div>
</template>

<script>
export default {
  name: "App",

  data() {
    return {
      text: "Hello, world",
      text2: "",
    };
  },

  methods: {
    changeProps: function () {
      this.text = "test";
    },

    changePropsBtn: function () {
      this.text2 = "test btn 1";
    },

    changePropsBtn2: function () {
      this.text2 = "test btn 2";
    },
  },
};
</script>
