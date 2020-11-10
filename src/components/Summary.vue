<template>
<div class="panel"> 
  <h1>Week Summary </h1>
    <p> Daily average: {{ average }} </p>
</div>
</template>

<script>
export default {
  name: 'Summary',
  props: {
  },
  data() {
    return {
      average: this.average
    }
  },
}
</script>
