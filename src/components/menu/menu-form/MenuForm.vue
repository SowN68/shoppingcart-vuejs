<template>
    <div class="menu-form">
        <input type="number" value="0" min="0" max="5" class="input-number">
        <button class="btn-buy">Buy</button>
    </div>
</template>

<!-- <script>
export default {

}
</script> -->

<style>
.input-number{
    width: 40px;
    height: 40px;
    margin-right: 16px;
    padding-left: 5px;
    border: 1px solid;
    border-radius: 8px;
    outline: none;
}
.btn-buy{
    width: 70px;
    height: 40px;
    border: 1px solid;

}
.btn-buy:active{
    background: rgb(91, 91, 91);
    color: white;
}
</style>