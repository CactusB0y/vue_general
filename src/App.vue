<template>
    <Navbar/>
    <Message msg='et je vais vous montrer certaines bases de VueJS'/>
    <Bind/>
    <Clock/>
    <For/>
    <If/>
    <ElseIf/>
</template>

<script>
    import Navbar from './components/Navbar.vue'
    import Message from './components/Message.vue'
    import Bind from './components/Bind.vue'
    import Clock from './components/Clock.vue'
    import For from './components/For.vue'
    import If from './components/If.vue'
    import ElseIf from './components/ElseIf.vue'

    export default{
        name: 'App',
        components: {
            Navbar,
            Message,
            Bind,
            Clock,
            For,
            If,
            ElseIf
        }
    }
</script>
