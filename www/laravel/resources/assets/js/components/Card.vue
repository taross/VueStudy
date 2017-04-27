<template>
    <div class="card">
        <div></div>

        {{ discribe }}
    </div>
</template>

<script>
    export default {
        data(){
            return{
                discribe:"This is card content."
            }
        }
    }
</script>

<style scoped="Card" lang="scss">
    .card{
        width:120px;
        height:160px;
        border: solid silver;
        border-radius: 10px;
        margin:10px;
    }

</style>