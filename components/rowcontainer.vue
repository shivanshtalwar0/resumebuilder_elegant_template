<template>
  <v-layout row wrap :class="rpadding+' '+rmargin">

       <slot></slot>
  </v-layout>



</template>

<script>
    export default {
        name: "rowcontainer",
      props:['rpadding','rmargin']
    }
</script>

<style scoped>

</style>
