<script>

export default{
  data(){
    return{
      tarefas: [
      {titulo: 'Integração com firebase 🚀✅', body: 'aplicação integrada com Firebase Firestore e auth', created_at: '01/02/23 02:16'},      
      {titulo: 'Ir a academia às 5:20 💪🏻', body: 'aplicação integrada com Firebase Firestore e auth', created_at: '01/02/23 02:16'},      
      {titulo: 'Febre Amarela - Exercícios ✅📚', body: 'aplicação integrada com Firebase Firestore e auth', created_at: '01/02/23 02:16'},      {titulo: 'Integração com firebase 🚀✅', body: 'aplicação integrada com Firebase Firestore e auth', created_at: '01/02/23 02:16'},
      ]
    }
  }
}

</script>

<template>
<div class="wrapper pt-5 mx-auto">


<div class="lg:max-w-md mx-auto" id="container">

<div class=" rounded overflow-hidden shadow-lg mx-auto ">
  <!-- <img class="w-full" src="/img/card-top.jpg" alt="Sunset in the mountains"> -->
  <div class="px-6 py-4">
    <div class="font-bold text-xl mb-2 mx-auto">Tarefas</div>
<!--     <p class="text-gray-700 text-base">
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus quia, nulla! Maiores et perferendis eaque, exercitationem praesentium nihil.
    </p> -->

      <input type="text" placeholder="Digite uma nova tarefa" class="px-4 py-3 w-full light rounded" />

      <button class="btn btn-blue ml-5  mt-5 text-center">
  Salvar
</button>
  </div>

</div>

<div class=" rounded-xl overflow-hidden shadow-lg mx-auto mt-5">
    <div class="px-6 pt-4 pb-2">
    <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">Todas</span>
    <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">Não finalizadas</span>
    <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">Concluidas</span>
  </div>
</div>

<div v-for="task in tarefas" class=" rounded overflow-hidden shadow-lg mx-auto mt-5  ">
  <div>
      <div class="font-bold text-x mb-2 mx-auto px-4">{{task.titulo}}</div>
      <div class="font-thin text-x mb-2 mx-auto px-4">{{task.body}} sdfsdsdf sdfsdf sdfs sdfsdf sdf </div>
      <div class="font-semibold text-sm mb-2 mx-auto px-4">{{task.created_at}}</div>

  </div>

  <hr class="ml-4 mr-4 mb-4 mt-4">

  <div class="btn-group px-4">
    <button class="bg-yellow-500 hover:bg-yellow-700"><span class="mdi mdi-close "></span></button>
    <button class="bg-red-500 hover:bg-red-700"><span class="mdi mdi-trash-can"></span></button>
    <button class="bg-blue-500 hover:bg-blue-700">
<span class="mdi mdi-tag-multiple-outline"></span></button>
  </div>

</div>
  
</div>

</div>
</template>


<style>
  .btn {
    @apply font-bold py-2 px-4 rounded;
  }
  .btn-blue {
    @apply bg-blue-500 text-white;
  }
  .btn-blue:hover {
    @apply bg-blue-700;
  }

  .btn-group button{
@apply  px-1 mb-2 mr-1 rounded-full  text-white font-bold;
    
  }
</style> 