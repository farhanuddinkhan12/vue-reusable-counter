<template>
    <div>
        <button @click="incrementCount">Clicked {{ count }} times</button>
    </div>
</template>

<script>
    import useCounter from '../composables/useCounter';
    export default {
        name: 'ClickCounter',

        setup(){
            const {count, incrementCount} = useCounter();

            return {
                count, 
                incrementCount
            }
        }
    }
</script>

<style scoped>

</style>