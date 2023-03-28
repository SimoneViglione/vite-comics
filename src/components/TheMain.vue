<script>
export default {

data () {
    return {
        products: [
        {
            "thumb": "https://static.dc.com/2023-03/LEGIONOB_Cv1_00111_DIGITAL.jpg?w=640",
            "price": "$19.99",
            "series": "Action Comics",
            "type": "comic book"
        },
        {
            "thumb": "https://static.dc.com/2023-03/BA_Cv9_00911_DIGITAL.jpg?w=640",
            "price": "$3.99",
            "series": "American Vampire 1976",
            "type": "comic book"
        },
        {
            "thumb": "https://static.dc.com/2023-03/ST_GH_Cv3_00311_DIGITAL.jpg?w=640",
            "price": "$16.99",
            "series": "Aquaman",
            "type": "graphic novel"
        },
        {
            "thumb": "https://static.dc.com/2023-03/MS30A_Cv1_00111_DIGITAL.jpg?w=640",
            "price": "$2.99",
            "series": "Batgirl",
            "type": "comic book"
        },
        {
            "thumb": "https://static.dc.com/2023-03/MS30A_Cv1_00111_DIGITAL.jpg?w=640", 
            "price": "$3.99",
            "series": "Batman",
            "type": "comic book"
        },
        {
            "thumb": "https://static.dc.com/2023-03/BMSMWF_Cv13_01311_DIGITAL.jpg?w=640",
            "price": "$2.99",
            "series": "Batman Beyond",
            "type": "comic book"
        },
        {
            "thumb": "https://static.dc.com/2023-03/NTW_Cv102_10211_DIGITAL-1.jpg?w=640",
            "price": "$3.99",
            "series": "Batman/Superman",
            "type": "comic book"
        },
        {
            "thumb": "https://static.dc.com/2023-03/FLS_Cv795_79511_DIGITAL.jpg?w=640",
            "price": "$4.99",
            "series": "Batman/Superman Annual",
            "type": "comic book"
        },
        {
            "thumb": "https://static.dc.com/2023-03/DCConnect_35-CVR.jpg?w=640",
            "price": "$5.99",
            "series": "Batman: The Joker War Zone",
            "type": "comic book"
        },
        {
            "thumb": "https://static.dc.com/2023-03/ROBIN_v3%20%28Cover%29.jpg?w=640",
            "price": "$6.99",
            "series": "Batman: Three Jokers",
            "type": "comic book"
        },
        {
            "thumb": "https://static.dc.com/2023-03/LP-ROTG_Cv1_00111_DIGITAL.jpg?w=640",
            "price": "$4.99",
            "series": "Batman: White Knight Presents: Harley Quinn",
            "type": "comic book"
        },
        {
            "thumb": "https://static.dc.com/2023-03/SM_LOST_Cv1_00111_DIGITAL.jpg?w=640",
            "price": "$16.99",
            "series": "Catwoman",
            "type": "graphic novel"
        }
        ]
        }
    }
}
</script>

<template>
    <div class="jumbotron">

    </div>

    <div class="product-window d-flex">

        <div class="current">CURRENT SERIES</div>

        <div class="products d-flex">
            <div v-for="(product, index) in products" :key="index" class="product d-flex">
                <img :src="product.thumb" />
                <span>{{ product.series }}</span>
            </div>
        </div>  
        
        <div class="load-button"> LOAD MORE </div>
    </div>
    
</template>

<style lang="scss" scoped>
    .jumbotron {
        background-image: url(../assets/img/jumbotron.jpg);
        width: 100%;
        height: 400px;
        background-size: cover;
        background-repeat: no-repeat;
    }

    .product-window {
        background-color: rgb(28, 28, 28);
        width: 100%;
        height: 570px;
        flex-direction: column;
    }

    .products {
        width: 100%;
        height: 500px;
        gap: 10px;
        flex-wrap: wrap;
        justify-content: center;
    }

    .product {
        width: calc((100% / 6) - 6rem);
        height: 150px;
        flex-direction: column;
        margin: 1rem 2rem;
        
        img {
            width: 100%;
            height: 150px;
            margin-bottom: 10px;
        }

    }

    .load-button {
        align-self: center;
        background-color: rgb(2, 130, 249);
        font-weight: 600;
        font-size: 12px;
        padding: 5px 30px;
        margin-bottom: 15px;
        cursor: pointer;

        &:hover {
            cursor: pointer;
        }

    }

    .current {
        background-color: rgb(2, 130, 249);
        font-weight: 600;
        font-size: 20px;
        padding: 5px 30px;
        width: 200px;
        margin-top: -20px;
        margin-left: 100px;
    }

    </style>