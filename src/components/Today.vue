<template>
<div class="panel"> 
  <h1>Today </h1>
    <input v-model="mealType" placeholder="Meal">
    <input v-model="mealItem" placeholder="What did you eat?">
    <input v-model.number="calories" placeholder="Enter calorie amount">
    <button v-on:click="add">Add meal</button>
    <p> Total calories: {{ total }} </p>
    <p> Calories remaining: {{ remainingCalories }} </p>
</div>
</template>

<script>
// TODO: Rename me
export default {
  name: 'Today',
  props: {
    // viewDate
  },
  data() {
    return {
      calories: this.calories,
      total: 0,
      remainingCalories: 1500,
      mealItem: ""
    }
  },
  methods: {
    add: function(e) {
      this.total += this.calories
      this.remainingCalories = 1500 - this.total
    }
  }
}
</script>
