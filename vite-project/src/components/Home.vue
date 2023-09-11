<template>
    <h2>Hello World from Home</h2>
</template>

<!-- vue logic -->

<script>
    export default {
        activated (){
            console.log ('activated app')
        },
        deactivated(){
            console.log('deactivated app')
        }
    }
</script>