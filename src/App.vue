<template>
    <div class="container">
        <div class="row">
            <div class="col-xs-12">
                <br>
                <button class="btn btn-primary" @click="selectedComponent = 'appBlue'">Load Blue Template</button>
                <button class="btn btn-success"  @click="selectedComponent = 'appGreen'">Load Green Template</button>
                <button class="btn btn-danger"  @click="selectedComponent = 'appRed'">Load Red Template</button>
                <hr>
                <component :is="selectedComponent"></component>
                <!-- <app-blue>
                    <h1 slot="blueSlot">blue slot title</h1>
                    <p slot="blueSlot">blue slot desc</p>
                </app-blue>
                <app-green>
                    <h1 slot="greenSlot">green slot title</h1>
                    <p slot="greenSlot">green slot desc</p>
                </app-green>
                <app-red>
                    <h1 slot="redSlot">red slot title</h1>
                    <p slot="redSlot">red slot desc</p>
                </app-red> -->
            </div>
        </div>
    </div>
</template>

<script>
    import Blue from './components/Blue.vue';
    import Green from './components/Green.vue';
    import Red from './components/Red.vue';

    export default {
        data: function(){
            return {
                selectedComponent: "appBlue"
            }
        },        
        components: {
            appBlue: Blue,
            appGreen: Green,
            appRed: Red
        }
    }
</script>

<style>
</style>
