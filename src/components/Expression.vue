<script setup>
 const number = 1454;
 const done = true;
 const msg = "This is a title line."; 


 const evenOdd = () => {
    return (number%2) == 0 ? 'Number is Even' : 'Number is Odd';
 }

 const alertShow = () => {
    alert('Hi Asif, are you sure to delete?');
 }

</script>

<template>
    <div>
       <p>{{ evenOdd() }}</p>
        <h3>{{ done ? 'complete' : 'Pending' }}</h3>

        <p class="desc" :class="done ? 'active' : ''">{{ msg }}</p>
        <p>{{ msg.split("").reverse().join("") }}</p>

        <p :class="`item-${number}`"> {{ msg }}</p>    //dynamic class add


        <button @click.prevent="alertShow()">Click Here</button>
    </div>
</template>

<style scoped>

p{
    color:rgb(225, 238, 183);
}
p.active{
    color: chartreuse;
}

</style>