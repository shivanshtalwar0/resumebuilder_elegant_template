<template>
  <v-flex
    :class="cpadding+' '+cmargin+' '+partition"

  >
    <slot></slot>
  </v-flex>
</template>

<script>
    export default {
        name: "columncontainer",
      props:['arrangement','cpadding','cmargin','small','xsmall','medium','large','xlarge','elements'],
      created(){

      },
      computed:{
          partition(){
            let arr=this.arrangement.split(",")

            return 'xs'+Math.abs(12/arr[0])+' '+'sm'+Math.abs(12/arr[1])+' '+'md'+Math.abs(12/arr[2])+' '+'lg'+Math.abs(12/arr[3])+' '+'xl'+Math.abs(12/arr[4])
          }

      }
    }
</script>

<style scoped>

</style>
