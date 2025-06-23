<template>

  <header>
    <nav>
      <NavBar />
    </nav>
  </header>

  <ContainerComponent>

    <main>
      <section>
        <HomeCotent />
      </section>

      <section>
        <PlansContent />
      </section>

      <section>
        <ClassesContent />
      </section>

      <section>
        <ContactContent />
      </section>

    </main>

    <footer>
    </footer>

  </ContainerComponent>

</template>

<script setup>
import NavBar from '@/components/NavBar.vue';
import HomeCotent from '@/components/HomeContent.vue';
import PlansContent from '@/components/PlansContent.vue';
import AuthorName from '@/components/AuthorName.vue';
import ContainerComponent from '@/components/ContainerComponent.vue';

</script>