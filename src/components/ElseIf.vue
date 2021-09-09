<template>
    <div class="h-1/4 w-full text-center mt-10">

        <h1 class="text-4xl mb-5">v-else-if/v-model:</h1>
        <h1 v-if="number < 5" class="text-4xl text-blue-500 mb-5">Je suis inférieur à 5</h1>
        <h1 v-else-if="number >= 5 && number < 10" class="text-4xl text-red-500 mb-5">Je suis supérieur ou égale à 5 et inférier à 10</h1>
        <h1 v-else class="text-4xl text-yellow-500 mb-5">Je suis supérieur à 10</h1>

        <div class="w-1/12 mx-auto">
            <label class="text-gray-700 dark:text-gray-200" for="username">Rentre un nombre ou un chiffre</label>
            <input v-model="number" id="username" type="number" class="block w-full px-4 py-2 mt-2 text-gray-700 bg-white border border-gray-300 rounded-md dark:bg-gray-800 dark:text-gray-300 dark:border-gray-600 focus:border-blue-500 dark:focus:border-blue-500 focus:outline-none focus:ring">
        </div>

    </div>
</template>

<script>
    export default {
        name: 'ElseIf',
        data() {
            return {
                number: 4
            }
        }
    }
</script>