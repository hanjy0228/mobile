<template>
 <div>
  {{store.state.conut}}
  <button @click="addAction">add</button>
  <button @click="reduceAction">reduce</button>
 </div>
</template>

<script>
import ComponentB from './ComponentB'
import ComponentC from './ComponentC'
import {mapActions} from 'vuex'
export default {
    data(){
        return{
            c:'111'
        }
    },
    methods:{
        ...mapActions(["addAction","reduceAction"])
    },
    components:{
        ComponentB,
        ComponentC
    }
}
</script>


<style >

</style>
