<template>
    <div class="h-1/4 w-full text-center mt-10">
        <h1 class="text-4xl my-auto text-green-700">{{text}}</h1>
        <h2 class="text-2xl my-auto text-yellow-700">{{msg}}</h2>
    </div>
</template>

<script>
    export default {
        name: 'Message',
        props: {
            msg: String
        },
        data(){
            return{
                text: 'Bienvenue sur ma première application VueJS'
            }
        }
    }
</script>
