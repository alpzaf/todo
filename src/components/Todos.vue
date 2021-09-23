<template>
    <div class="xl:container mx-auto">
      <div class="row">
        <div class="todo-item bg-gray-200 mt-5 xl:rounded py-5 px-5">
          <p class="text-gray-500 h-24 overflow-scroll px-10 py-5 bg-white w-75 mx-auto text-left xl:rounded" v-text="todoText"></p>
          <button class="w-44 block bg-gray-400 px-5 py-1 xl:rounded mt-5 text-white ml-auto">Tamamlandı</button>
        </div>
      </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            todoText : 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam consectetur maiores impedit consequatur ex esse eligendi quidem itaque deleniti! Sint molestiae laboriosam culpa saepe in facere distinctio? Enim quod cum quibusdam saepe asperiores rerum, nulla officia dignissimos excepturi quia! Cupiditate nesciunt est aliquam molestias, corrupti saepe architecto assumenda neque totam, ut laborum, vero magni sint sed? Cumque sapiente non nulla ab molestiae! Quam totam voluptates harum explicabo minus nulla eveniet esse, aspernatur obcaecati porro quasi sunt expedita nobis ipsa at dolore sequi quaerat neque! Eveniet, labore. Numquam, consectetur labore nemo, iste praesentium rerum pariatur temporibus ducimus, veritatis similique odio beatae.'
        }
    }
}
</script>