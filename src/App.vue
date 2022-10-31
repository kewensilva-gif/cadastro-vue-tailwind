<template>
<div class="w-screen h-screen flex items-center justify-center dark:bg-gray-900 bg-gray-50">
  <div class="bg-white shadow-xl w-full sm:10/12 md:w-8/12 lg:w-6/12 p-6">
    <h4 class="font-semibold text-md mb-3 border-b border-gray-300">Login</h4>

    <div class="space-y-3">
        <input 
          type="text"
          class="px-3 py-2 placeholder-gray-200 border border-gray-300 w-full"
          placeholder="E-mail"
          >

        <input 
          type="password"
          class="px-3 py-2 placeholder-gray-200 border border-gray-300 w-full"
          placeholder="Senha"
        >

        <div class="text-right">
          <button class="rounded px-3 py-2 bg-green-400 hover:bg-green-500 text-green-900">Login</button>
        </div>
      </div>
  </div>
    <DarkMode />
</div>

</template>

<script>
import DarkMode from "./components/DarkMode.vue";
export default {
  name: "App",
  components: {
    DarkMode
  }

}
</script>