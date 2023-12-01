<template>
    

    <div  :class="book.availability ? 'green': 'red' ">

                        <h2>{{book.location}}</h2>
                        <h4>Best Place in this Location : {{book.places_in_location}}</h4>
                        <h4>Hotel Dates(DD.MM) : {{book.hotel_dates}}</h4>
                        <h4>Best Time to Visit : {{book.best_time_to_visit}}</h4>
                        <h4>Price of the Hotel : {{book.price_of_Hotel}}</h4>
                        <img :src="book.photo" alt="Hotel Photo" style="max-width: 100%;" />
 
                        
    </div>
</template>

<script>

export default{
    name: 'SingleBook',
    props:{
        book: Array
    }
}
</script>

<style scoped>

.green{
    background-color: green;
}

h4{
    margin: 2px;
}

div{
    background-color: #ffb89e;
    color: black;
    padding: 1em;
    text-align: center;
    width: 80%;
    margin: auto;
    

}

.red{
background-color: orangered !important;

}


</style>