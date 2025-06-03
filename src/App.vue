<template>
  <ContainerComponent>

    <header>
      <NavBar>
        <NavRow>
          <NavLink to="#">HOME</NavLink>
          <NavLink to="#">PLANS</NavLink>
        </NavRow>
        <LogoImage/>
        <NavRow>
          <NavLink to="#">CLASSES</NavLink>
          <NavLink to="#">CONTACT</NavLink>
        </NavRow>
      </NavBar>
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
    
  </ContainerComponent>
</template>

<script setup>
import NavLink from '@/components/NavLink.vue';
import NavBar from '@/components/NavBar.vue';
import NavRow from '@/components/NavRow.vue';
import LogoImage from '@/components/LogoImage.vue';
import ContainerComponent from '@/components/ContainerComponent.vue';
import { Container } from 'postcss';
function handleClick() {
  alert("Hello from Vue 3 + Tailwind 4!")
}

</script>
