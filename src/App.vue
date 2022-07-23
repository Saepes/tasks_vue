<template>
  <div>
    <input type="text" v-model="num" />
    <p>Квадрат числа - {{ showMult(num) }}</p>
  </div>

  <div>
    <button @click="clickBtn(1)">Кнопка 1</button>
    <button @click="clickBtn(2)">Кнопка 2</button>
    <p>Число - {{ show() }}</p>
  </div>
</template>

<script>
export default {
  name: "App",

  data() {
    return {
      num: "",
      num1: 2,
      num2: 3,
      res: "",
    };
  },

  methods: {
    showMult: function () {
      return this.num * this.num;
    },

    clickBtn: function (n) {
      if (n === 1) {
        this.res = this.num1 * this.num1;
      } else if (n === 2) {
        this.res = this.num2 * this.num2 * this.num2;
      }
    },

    show: function () {
      return this.res;
    },
  },
};
</script>
