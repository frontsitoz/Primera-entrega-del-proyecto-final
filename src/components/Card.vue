<template>
  <div
    class="max-w-sm flex flex-col justify-center items-center bg-white border border-gray-200 rounded-lg shadow-md dark:bg-gray-800 dark:border-gray-700"
  >
    <img
      class="rounded-t-lg"
      src="../assets/logo.png"
      :alt="productos.nombre"
    />
    <div class="p-5">
      <h5
        class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white"
      >
        {{ productos.nombre }}
      </h5>
      <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">
        {{ productos.marca }}
      </p>
      <div class="flex gap-4">
        <button
          class="w-auto flex items-center text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
        >
          INFO
          <svg
            aria-hidden="true"
            class="w-4 h-4 ml-2 -mr-1"
            fill="currentColor"
            viewBox="0 0 20 20"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              fill-rule="evenodd"
              d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z"
              clip-rule="evenodd"
            ></path>
          </svg>
        </button>
        <button
          class="w-auto text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
        >
          Comprar
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardComponent",

  data() {
    return {};
  },
  props: {
    productos: Object,
  },
};
</script>

<style></style>
