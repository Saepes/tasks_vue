<template>
  <div>
    <input type="text" v-model="day" />
    <p>День недели - {{ showWeekDay(day) }}</p>
  </div>

  <div>
    <p>Сегодня - {{ showWeekDayToday() }}</p>
  </div>
</template>

<script>
export default {
  name: "App",

  data() {
    return {
      day: "",
    };
  },

  methods: {
    showWeekDay: function (day) {
      return this.getWeekDay(this.day);
    },

    showWeekDayToday: function () {
      let dateToday = new Date().getDate();
      return this.getWeekDay(dateToday);
    },

    getWeekDay: function (day) {
      let days = ["ВС", "ПН", "ВТ", "СР", "ЧТ", "ПТ", "СБ"];
      let date = new Date(2022, 6, day);

      return days[date.getDay()];
    },
  },
};
</script>
