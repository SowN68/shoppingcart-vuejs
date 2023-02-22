<template>
    <div class="menu-list--container">
        <input v-model="searchItem" type="text" placeholder="Search item" class="search-bar">
        <button>Add item</button>
        <menu-item v-for="item in filterItem" :key="item.id" :name="item.name" :price="item.price"></menu-item>
    </div>
</template>
<script>
import MenuItem from './MenuItem.vue'

export default {
    data() {
        return {
            searchItem: '',
            menuList: [
                {
                    id: 0,
                    name: 'Fish',
                    price: '$10'
                },
                {
                    id: 1,
                    name: 'Tomato',
                    price: '$5'
                },
                {
                    id: 2,
                    name: 'Potato',
                    price: '$3'
                },
                {
                    id: 3,
                    name: 'Meat',
                    price: '$12'
                },
                {
                    id: 4,
                    name: 'Vegetable',
                    price: '$22'
                },
            ]
        }
    },
    components: {
        MenuItem,
    },
    computed: {
        filterItem() {
            return this.menuList.filter(item => { return item.name.toLowerCase().includes(this.searchItem.toLowerCase()) })

        }
    }
}
</script>

<style>
.menu-list--container {
    width: 100%;
    display: flex;
    flex-direction: column;
    flex-wrap: nowrap;
    align-items: center;
    gap: 25px;
}

.search-bar {
    width: 60%;
    height: 40px;
    font-size: 16px;
    padding: 15px 0px 15px 20px;
    border: 1px solid gray;
    border-radius: 10px;
    outline: none;
}
</style>