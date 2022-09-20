<template>
    <div>
        <h1>
            COUNTER: {{ couter }}
        </h1>
        <button @click="decrement">
            Decrement
        </button>
        <button @click="increment">
            Increment
        </button>
    </div>
</template>

<script>
    export default{
        name: 'Counter',
        data: () => ({
            couter: 0
        }),
        methods: {
            decrement: function(){
                this.counter--
            },
            increment: function(){
                this.counter++
            }
        }
    }
</script>