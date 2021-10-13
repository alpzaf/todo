<template>
    <div class="xl:container m-auto">
      <div class="row">
        <!--
        <div class="todo-input bg-gray-200 mt-5 xl:rounded py-5 px-5 flex items-center">
          <input class="border-none bg-white xl:rounded w-10/12 px-5 py-5">
          <button class="w-44 block bg-gray-400 px-5 py-1 xl:rounded text-white ml-auto">+</button>
        </div>
        -->
        <div class="todo-item bg-gray-200 mt-5 xl:rounded py-5 px-5">
          <p class="text-black-500 h-24 overflow-scroll px-10 py-5 bg-white w-75 mx-auto text-left xl:rounded"> {{ todo.content }} </p>
          <button class="w-44 block bg-gray-400 px-5 py-1 xl:rounded mt-5 text-white ml-auto">Tamamlandı</button>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  props : ["todo"]
}
</script>