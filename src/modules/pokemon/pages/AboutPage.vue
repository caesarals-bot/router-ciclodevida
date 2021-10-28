<template>
    <h1>About Page</h1>
    <hr>
    <!-- <h2>{{ name }} </h2> -->
    <button @click="onChangeName">Cambiar Nombre</button>

</template>

<script>
export default {

    data(){
        return{
            name: 'Cesar'
            }
    },
    methods: {
        onChangeName(){
            console.log('Se Cambia')
            this.name = 'Melissa'
        }
    },

    beforeCreate(){
        console.log('beforeCreate')
    },
    created(){
        console.log('Create')
    },
    beforeMount(){
        console.log('beforeMount')
    },
    mounted(){
        console.log('mounted')
    },
    beforeUpdate(){
        console.log('beforeUpdate')
    },
    activated(){
        console.log('activated')
    },
    deactivated(){
        console.log('deactivated')
    },
    beforeUnmount(){
        console.log('beforeUnmount')
    },
    unmounted(){
        console.log('unmounted')
    },
    errorCaptured(){
        console.log('unmounted')
    },
    renderTracked(){
        console.log('renderTracked')
    },
    renderTriggered(){
        console.log('renderTriggered')
    },
    errorCaptured(){
        console.log('errorCaptured')
    },
}
</script>