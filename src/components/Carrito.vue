<template>
  <div class="text-center">
    <h2 class="text-xl font-semibold">Productos agregados al carrito</h2>
    <table
      class="text-sm text-left text-gray-500 dark:text-gray-400 w-1/2 mx-auto my-6"
    >
      <thead
        class="text-xs text-gray-800 uppercase bg-gray-50 dark:bg-gray-700 dark:text-gray-400"
      >
        <tr>
          <th scope="col" class="px-6 py-3">ID</th>
          <th scope="col" class="px-6 py-3">Producto</th>
          <th scope="col" class="px-6 py-3">Cantidad</th>
          <th scope="col" class="px-6 py-3">$</th>
          <th scope="col" class="px-6 py-3">Total</th>
        </tr>
      </thead>
      <tbody>
        <tr
          v-for="(producto, i) of carrito"
          :key="i"
          class="bg-gray-300 border-b dark:bg-gray-800 dark:border-gray-700"
        >
          <td class="px-6 py-4 text-gray-900 dark:text-white">1</td>
          <td
            class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap dark:text-white"
          >
            {{ producto.producto }}
          </td>
          <td class="px-6 py-4 text-gray-900 dark:text-white">
            {{ producto.cantidad }}
          </td>
          <td class="px-6 py-4 text-gray-900 dark:text-white">
            {{ producto.precio }}
          </td>
          <td class="px-6 py-4 text-gray-900 dark:text-white">
            {{ producto.total }}
          </td>
        </tr>
      </tbody>
    </table>
    <button
      class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm w-full sm:w-auto px-5 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
    >
      Volver
    </button>
  </div>
</template>

<script>
export default {
  name: "CartComponent",

  data() {
    return {
      carrito: [
        {
          producto: "Producto X",
          cantidad: 4,
          precio: 580,
          total: 2320,
        },
        {
          producto: "Producto Y",
          cantidad: 2,
          precio: 400,
          total: 800,
        },
        {
          producto: "Producto Z",
          cantidad: 1,
          precio: 500,
          total: 500,
        },
      ],
    };
  },
};
</script>

<style></style>
