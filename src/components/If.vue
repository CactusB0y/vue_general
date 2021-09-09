<template>
    <div class="h-1/4 w-full text-center mt-10">
        <h1 class="text-4xl mb-5">v-if/v-else:</h1>
        <h1 v-if="true_false" class="text-2xl text-pink-300">Je suis vrai donc tu me vois</h1>
        <h1 v-else class="text-2xl text-pink-300">MOUHAHAHAHHA JE SUIS FAUX</h1>
        <button @click="changeBoolean" class="px-4 py-2 font-medium tracking-wide text-white transition-colors duration-200 transform bg-blue-600 rounded-md dark:bg-gray-800 hover:bg-blue-500 dark:hover:bg-gray-700 focus:outline-none focus:bg-blue-500 dark:focus:bg-gray-700 mt-5">
            clique ici pour changer le boolean
        </button>
    </div>
</template>

<script>
    export default {
        name: 'If',
        data(){
            return {
                true_false: true
            }
        },
        methods: {
            changeBoolean(){
                if (this.true_false == true) {
                    this.true_false = false
                } else {
                    this.true_false = true
                }
            }
        }
    }
</script>