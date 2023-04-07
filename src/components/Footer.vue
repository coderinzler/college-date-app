<template>
    <footer>
        <p>{{ emailText }}</p>
        <p>{{ numberText }}</p>
        <p>{{ addressText }}</p>
    </footer>
</template>


<script>
    export default{
        data(){
            return{
                emailText:"venta@library.com",
                numberText:"981622558",
                addressText:"Los Manzanos 398"
            }
        }
    }
</script>


<style scoped>
footer{
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    color: white;
    font-weight: bold;
}
</style>