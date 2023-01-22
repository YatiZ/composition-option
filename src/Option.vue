<template>
    <h4>The current count is....</h4>
    <h1>{{ count }}</h1>
    <button @click="subtractCount()">-</button>
    <button @click="addCount()">+</button>
</template>

<style scoped>

</style>

<script>
export default({
    data(){
        return{
            count: 0
        }
    },
    methods:{
        addCount(){
            this.count = this.count+1
        },
        subtractCount(){
            this.count = this.count-1
        }
    }
})
</script>
