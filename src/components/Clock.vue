<template>
    <div class="h-1/4 w-full text-center mt-10">
        <h1 class="text-4xl">Compteur de seconde:</h1>
        <h1 class="text-4xl my-auto text-red-700">{{counter}}</h1>
        <h1 class="text-4xl my-auto text-red-700">{{hour}}</h1>
    </div>
</template>

<script>
    export default {
        name: 'Clock',
        data() {
            return {
                counter: 0,
                hour: new Date().toLocaleTimeString()
            }
        },
        mounted(){
            setInterval(() => {
                this.counter++
                this.hour = new Date().toLocaleTimeString()
            }, 1000)
        }
    }
</script>