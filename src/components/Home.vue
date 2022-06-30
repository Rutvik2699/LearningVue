<template>
<div>
  <h1>Hello from Home component</h1>

  <!-- using v-f and v-else to d oconditional rendering -->
  <!-- Function 1 -->
  <h1 v-if="show">Conditional Rendering</h1>
  <h1 v-else>Conditional Rendering is false</h1>

  <button v-on:click="display">Toggle Element</button>


  
  <!-- <h2>{{data}}</h2>
  <h2>{{msg}}</h2> 
  
  ON click and mouseover-->
<!-- //Hello function called on Click and Hello call parameter passed to Hello function below -->
<!-- Function 2 -->
  <button v-on:click="hello('Hello Call')">Call Hello Function</button>
   <button v-on:mouseover="hello('Hello Call')">Call function when hover</button>


   <!-- Function3 
   Loops-->

   <h1>For loop in Vue js</h1>
   <table border=1px>
    <tr>
        <td>Id</td>
        <td>Name</td>
        <td>Email</td>
    </tr>
    <tr v-for="user in users" :key="user.id">
        <td>{{user.id}}</td>
        <td>{{user.name}}</td>
        <td>{{user.email}}</td>
    </tr>

   </table>


   <!-- Function 4 
   Component-->
  </div>
</template>

<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name:'Home',
    props:{
        data:String,
        msg:String
    },methods:{
        //Function 2 
        //Hello function created and data passed to alert
        hello(data){
            console.log("Hello console called");
            alert(data);
        },
        //Function 1
        //To hide and display conditional elements 
        display(){
            this.show=!this.show
        }
    },
   
    
    data(){
         //To check if the function is true or false and display output accordingly
        //Function 1
       // return{show:false};

        return {

            //Function 3
            users:[
                {id:1,name:'peter',email:'peter@test.com'},
                 {id:2,name:'bruce',email:'bruce@test.com'},
                 {id:3,name:'tony',email:'tony@test.com'},
                  {id:4,name:'sam',email:'sam@test.com'}           
            
            ]}
    }

}
</script>

<style>

</style>