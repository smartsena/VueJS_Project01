<template>
    <div>
        <!-- <div v-for="obj in listUsers" v-bind:key="obj.id" class="todos-itens"> -->
        <div v-for="(obj, index) in listUsers" v-bind:key="obj.id" class="todos-itens">
            {{index}} - {{obj.name + " --- Titulo: " + obj.title}}
        </div>
    </div>

</template>

<script>
export default {
    data() {
        return{
        listUsers: [
            {
            "userId": 1,
            "id": 7,
            "name": "João",
            "title": "illo expedita consequatur quia in",
            "completed": false
            },
            {
            "userId": 1,
            "id": 8,
            "name": "Cintya",
            "title": "quo adipisci enim quam ut ab",
            "completed": true
            },
            {
            "userId": 1,
            "id": 9,
            "name": "Gabriel",
            "title": "molestiae perspiciatis ipsa",
            "completed": false
            },
            {
            "userId": 1,
            "id": 10,
            "name": "Mostafa",
            "title": "illo est ratione doloremque quia maiores aut",
            "completed": true
            },
            {
            "userId": 1,
            "id": 11,
            "name": "Andreza",
            "title": "vero rerum temporibus dolor",
            "completed": true
            },]
        }
    }
}

</script>

<style>
    .todos-itens {
        background: #300;
        color: #fff;
        margin: 0 0 5px 0;
        padding: 3px 6px;
    }
</style>
