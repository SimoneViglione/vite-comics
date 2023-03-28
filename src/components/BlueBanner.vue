<script>
export default {

data () {
  return {
    market: [
        {
            icon: '',
            product: 'DIGITAL COMICS'
        },
        {
            icon: '',
            product: 'DC MERCHANDISE'
        },
        {
            icon: '',
            product: 'SUBSCRIPTION'
        },
        {
            icon: '',
            product: 'COMIC SHOP LOCATOR'
        },
        {
            icon: '',
            product: 'DC POWER VISA'
        },
    ]
    }},
    methods: {
        
      
    }
}
       
</script>

<template>
    <div class="blue-banner d-flex">
        <div v-for="item in market" :key="item.product" class="market d-flex">
            <div class="product-img">
               <img> 
            </div>
            
            <h3>{{ item.product }}</h3>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.blue-banner {
    height: 200px;
    background-color: rgb(2, 130, 249);
    justify-content: center;
}

.market {
    align-items: center;
    gap: 1rem;
}

.product-img {
    width: 70px;
    height: 100px;

        img {
            width: 100%;
            height: 100px;
        }
}
</style>