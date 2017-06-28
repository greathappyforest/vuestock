<template>
 <div>
    <app-stock v-for="(stock,index) in stocks" :stock="stock"></app-stock>
 </div>  
</template>


<script>
    import Stock from './Stock.vue';
    export default {
        data() {
            return {
                stocks: [{
                    id: 1,
                    name: 'Coke',
                    price: 110
                }, {
                    id: 2,
                    name: 'Apple',
                    price: 200
                }, {
                    id: 3,
                    name: 'Google',
                    price: 300
                }, {
                    id: 4,
                    name: 'facebook',
                    price: 150
                }, {
                    id: 4,
                    name: 'amazon',
                    price: 150
                }]

            }
        },
        components: {
            appStock: Stock
        }

    }
</script>