<template>
    <div class="h-1/4 w-full text-center mt-10">
        <h1 class="text-4xl mb-5">Boucle v-for:</h1>
        <ul>
            <li class="text-purple-600" v-for="(todo, index) in todos" :key="index" >
                {{todo.personne}} va {{todo.text}}
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
        name: 'For',
        data(){
            return {
                todos: [
                    {text: 'Aller faire les courses', personne: 'Tania'},
                    {text: 'Glander toute la sainte journée KUIZINE', personne: 'Cactus'},
                    {text: 'Draguer les milfs les plus chaudes de la région', personne: 'Alexis'},
                ]
            }
        }
    }
</script>