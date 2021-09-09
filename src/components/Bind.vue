<template>
    <div class="h-1/4 w-full text-center mt-10" v-bind:title='message' >
        <h1 class="text-4xl">Bind:</h1>
        <h1 class="text-4xl my-auto text-indigo-700"> Passe la souris sur moi </h1>
    </div>
</template>

<script>
    export default {
        name: 'Bind',
        data(){
            return {
                message: 'oui tu passe bien ta souris dessus'
            }
        }
    }
</script>