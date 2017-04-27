<template>
    <div class="container">
        <div class="row">
            <div class="col-md-2">
                {{ test }}
            </div>

            <div class="col-md-10 container-card">
                <card v-for="n in 10"></card>
            </div>
        </div>

    </div>
</template>

<script>
    import CardComponent from "./Card.vue"

    export default {
        mounted() {
            console.log('Component mounted.')
        },
        data(){
            return{
                test:"Hello!"
            }
        },
        components:{
            "card": CardComponent
        }
    }
</script>
<style lang="scss">
    .container-card{
        display: flex;
        flex-wrap: wrap;
        align-content: space-around;
    }
</style>