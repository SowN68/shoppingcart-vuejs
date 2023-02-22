<template>
  <div class="navigation">
    <h1>VueFood</h1>
    <header-btn></header-btn>
  </div>
</template>

<script>
import HeaderBtn from './HeaderBtn.vue';

export default {

    components:{
        HeaderBtn
    }
}
</script>

<style>
.navigation{
    width: 100%;
    height: 64px;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    background-color: brown;
    color: white;
    margin-bottom: 40px;
    padding: 0 20px 0 56px;
}
</style>