<template>
    <div> 
        <slot></slot>
    </div>
</template>
<script>
export default {
    props:{
        quote: String
    }
}
</script>
<style scoped>
    div{
        border:  1px solid #ccc;
        box-shadow: 1px 1px 2px black;
        padding: 30px;
        margin : 30px auto;
    }
    h2{
        color: red;
    }
</style>