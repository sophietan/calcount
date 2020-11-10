<template>
<div class="panel"> 
  <h1>Yesterday </h1>
    <p> Calories Eaten: {{ calories }} </p>
</div>
</template>

<script>
export default {
  name: 'Yesterday',
  props: {
  },
  data() {
    return {
      calories: this.calories,
    }
  }
}
</script>
