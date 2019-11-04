<template>
    <div class="container">
        <div class="row">
            <div class="col-xs-12">
               <app-quote >
    
                {{title}}
                <h2>ทดสอบการทำงานของ Scoped</h2>
               </app-quote>
            </div>
        </div>
    </div>
</template>

<script>
    import Quote from './components/Quote'
    export default {
        data: function(){
            return{
                title: 'ทดสอบ Slotes'
            };
        },
        components: {
            appQuote: Quote
        }
    }
</script>

<style>
</style>
