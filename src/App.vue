<template>
  <Today/>
  <Yesterday/>
  <Summary/>
</template>

<script>
import Today from './components/Today.vue'
import Yesterday from './components/Yesterday.vue'
import Summary from './components/Summary.vue'

export default {
  name: 'App',
  components: {
    Today,
    Yesterday,
    Summary
  }
}
</script>
