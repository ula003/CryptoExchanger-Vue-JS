<template>
    <input min="0" type="number" @input="changeAmount($event.target.value)" placeholder="Введите Число"> <br>
    <button @click="convert()">Конвертировать</button>
</template>

<script>
export default{
    props:{
        changeAmount: {
            type: Function,
            required: true,
        },
        convert: {
            type:Function,
            required:true,
        }
    }
}

</script>
<style scoped>
input{
    outline: none;
    border-radius: 3px;
    border: none;
    padding: 10px 15px;
    background-color: #fafafa;
    width: 500px;
    position: relative;
    top: -50px;
    font-size: 1.2em;
}
button{
    position: relative;
    top:-20px;
    padding: 15px 20px;
    color: white;
    text-transform: uppercase;
    cursor: pointer;
    background: #1a032d;
    border: 0;
    border-radius: 3px;
}
</style>