<template>
  <div class="min-w-screen min-h-screen bg-gray-950 text-gray-200">
    <header>
      <div id="navbar" class="fixed top-0 left-1/2 transform -translate-x-1/2 z-50 w-160
      transition-[background] duration-300 text-xl font-bold
      [clip-path:polygon(0%_0%,100%_0%,95%_100%,5%_100%)] flex justify-center">
        <div class="flex justify-evenly items-center w-9/10">
          <div class="flex justify-evenly gap-x-6 w-50">
            <a href="#" class="hover:text-blue-500 transition-colors">HOME</a>
            <a href="#" class="hover:text-blue-500 transition-colors">PLANS</a>
          </div>
          <img src="@/assets/images/movestyle.svg" alt="Icon" class="w-20 h-20 mx-4"/>
          <div class="flex justify-evenly gap-x-6 w-50">
            <a href="#" class="hover:text-blue-500 transition-colors">CLASSES</a>
            <a href="#" class="hover:text-blue-500 transition-colors">CONTACT</a>
          </div>
        </div>
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
      © 2025 Tacio Kikuchi
    </footer>
  </div>
</template>

<script setup>
function handleClick() {
  alert("Hello from Vue 3 + Tailwind 4!")
}
window.addEventListener('scroll', () => {
  const header = document.getElementById('navbar');
  header.classList.toggle('bg-black/50', window.scrollY > 10);
});
</script>
