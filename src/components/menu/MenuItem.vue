<template>
  <card-tmp>
    <div class="item-infor">
        <div class="food-name">{{ name }}</div>
        <div class="food-price">{{ price }}</div>
    </div>
    <div class="form">
        <menu-form></menu-form>
    </div>
  </card-tmp>
</template>

<script>
import CardTmp from '../card/CardTmp.vue'
import MenuForm from './menu-form/MenuForm.vue';
export default {

    components:{
        CardTmp,
        MenuForm
    },
    props:{
        name:{
            type: String,
            required:true
        },
        price:{
            type: String,
            required:true
        }
    }
}
</script>

<style>

</style>