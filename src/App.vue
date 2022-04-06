<template>
  <div id="app" class="container">
    <h1>Tabla de Usuarios</h1>
<table class="table">  
     <tr>
         <th>#</th>
         <th>Nombre</th>
         <th>Apellido</th>
         <th>RUN</th>
         <th>Nacimiento</th>
         <th>Edad</th>
     </tr>
     <tr v-for="(dato, index) in lista" :key="index">
        <td>{{dato.id}}</td>
        <td>{{dato.nombre}}</td>
        <td>{{dato.apellido}}</td>
        <td>{{dato.run}}</td>
        <td>{{dato.nacimiento}}</td>
        <td>{{dato.edad}}</td>
     </tr>
    </table>

  </div>
  </template>
   <script>

 export default {
  name: "app",
  data () {  
    return  {
      lista:[
      {
               id:'1',
               nombre:'Jose',
               apellido:'Perez',
               run:'123456-2',
               nacimiento:'12-04-67',
               edad:'52'

            },
            {
               id:'2',
               nombre:'Maria',
               apellido:'Rodriguez',
               run:'654321-1',
               nacimiento:'30-11-90',
               edad:'29'

            },
            {
               id:'3',
               nombre:'Manuel',
               apellido:'Patiño',
               run:'14223456-6',
               nacimiento:'02-12-59',
               edad:'60'

            },
        
        ],
        }
   },     
 }

 </script> 

 <style>
   *{
    margin:0;
    padding:0;
   }
  .container{
    margin-top: 20px;
    width: 100%;
    height: 100%;
    background-color: #f2f2f2;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0px 0px 10px #000;
    text-align: center;
    }
    h1{
      text-align: center;
      color: #000;
      font-size: 30px;
      font-weight: bold;
    }
    table{
      width: 100%;
      border-collapse: collapse;
      border: 1px solid #000;
      margin-top: 20px;
    }
    table tr{
      border: 1px solid #000;
    }
    .table th, .table td{
      border: 1px solid #000;
      padding: 5px;
    }
   #app{
    margin-top:200px;
     }
   h1{
    text-align: center;
   };

 </style>