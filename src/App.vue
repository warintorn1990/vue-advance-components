<template>
    <div class="container">
        <div class="row">
            <div class="col-xs-12">
                <button @click="selectedComponent = 'appQuote'">Quote</button>
                <button @click="selectedComponent = 'appAuther'">Auther</button>
                <button @click="selectedComponent = 'appNew'">New</button>
            <hr>
            {{selectedComponent}}
            <component :is="selectedComponent"></component>
    
               <!-- <app-quote >
                {{selectedComponent}}
                <h2>ทดสอบการทำงานของ Scoped</h2>
               </app-quote> -->
            </div>
        </div>
    </div>
</template>

<script>
    import Quote from './components/Quote'
    import Auther from './components/Auther'
    import New from './components/New'

    export default {
        data: function(){
            return{
                title: 'ทดสอบ Slotes',
                selectedComponent: 'appQuote'
            };
        },
        components: {
            appQuote: Quote,
            appAuther: Auther,
            appNew: New
        }
    }
</script>

<style>
</style>
