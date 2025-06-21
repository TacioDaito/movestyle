<template>
  <ContainerComponent>
    
    <header>
      <nav><NavBar/></nav>
    </header>

    <main>

      <section>
        <HomeCotent/>  
      </section>
      
      <section>
        <PlansContent/>
      </section>

      <section>
        <ClassesContent/>
      </section>

      <section>
        <ContactContent/>
      </section>

    </main>

    <footer>
    </footer>

  </ContainerComponent>
</template>

<script setup>
import NavBar from '@/components/NavBar.vue';
import HomeCotent from '@/components/HomeContent.vue';
import AuthorName from '@/components/AuthorName.vue';
import ContainerComponent from '@/components/ContainerComponent.vue';
import { Container } from 'postcss';
function handleClick() {
  alert("Hello from Vue 3 + Tailwind 4!")
}

</script>
