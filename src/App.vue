<template>
  <div class="min-w-screen min-h-screen bg-gray-950 text-gray-200">
    <header>
      <div id="navbar" class="p-4 fixed top-0 left-0 right-0 z-50 transition-colors duration-300
      text-2xl font-bold">
        <a href="#" class="hover:text-blue-500">Sign In</a>
        <a href="#" class="hover:text-blue-500">Light</a>
        <a href="#" class="hover:text-blue-500">Steady</a>
        <a href="#" class="hover:text-blue-500">Fierce</a>
      </div>
    </header>

    <main class="p-6 bg-[url(src/assets/images/bg.jpg)] bg-center bg-cover bg-no-repeat
    bg-fixed flex items-center justify-center h-screen">
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
window.addEventListener('scroll', () => {
  const header = document.getElementById('navbar');
  header.classList.toggle('bg-purple-300', window.scrollY > 10);
  header.classList.toggle('text-gray-900', window.scrollY > 10);
});
</script>
