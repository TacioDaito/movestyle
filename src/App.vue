<template>
  <div class="min-w-screen min-h-screen bg-gray-950 text-gray-200">
    <header class="bg-purple-900 p-4">
      <h1 class="text-2xl font-bold">My Simple Vue 3 + Tailwind 4 Site</h1>
    </header>

    <main class="p-6">
      <section class="max-w-2xl mx-auto text-center">
        <h2 class="text-xl font-semibold mb-4">Welcome!</h2>
        <p class="mb-6 text-gray-400">This is a clean simple page built with Vue 3 and Tailwind CSS 4.</p>
        <button
          class="bg-blue-800 hover:bg-blue-600 font-medium py-2 px-4 rounded-md transition"
          @click="handleClick"
        >
          Click Me
        </button>
      </section>
    </main>

    <footer class="text-center text-sm text-gray-500 p-4 mt-8">
      © 2025 My Simple Site
    </footer>
  </div>
</template>

<script setup>
function handleClick() {
  alert("Hello from Vue 3 + Tailwind 4!")
}
</script>
