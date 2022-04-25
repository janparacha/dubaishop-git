<template>
    <article class="w-80 pb">
        <h2 class="t1">Collection Lataffa</h2>
           <img :src= "require(`/public/${image}`)"/>

            <p class="p1 h-20"> {{description}} </p>

            <p> {{price}} € </p>

            <p class="date1"> Posté le <time datetime="2021-01-09">9 janvier</time> par Jan</p>
    </article>
</template> 

<script>
export default {
 name: 'Article',
 props: {
     description:String,
     image:String, 
     price:Number,
 }
}

</script>
