<template>
  <div>
  
   <p v-html="rowHtml"></p>
    <!-- To change name only Once we use v-once function -->
    <h3 v-once>{{name}}</h3>
    <h3>{{name}}</h3>

    <!-- To change yes or no we use OK function and change it by click of button  -->
    <h3>{{ok?"Yes":"No"}}</h3>
    <button v-bind:disabled="disableBtn" v-on:click="updateText">Click me</button>
  </div>
</template>

<script>
export default {
    name:"TemplateInVue",
    data(){
        return{
            //Defingin all the values to the variables
            name:'Anil',
            a:10,
            b:10,
            ok:true,
            //To display TEMPLATE IN VUE JS  dynamically 
            rowHtml:"<h1>Template in Vue Js</h1>",
            //Disabling input
            disableBtn:false
        }
    },
    methods:{
        updateText(){
            //Defining name
            this.name="Peter",
            //Using fucntion to change the yes to No and No to yes
            this.ok=!this.ok
        }
    }
};
</script>

<style>

</style>