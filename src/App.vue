<template>

  <header>
    <nav>
      <NavBar />
    </nav>
  </header>

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

</template>

<script setup>
import NavBar from '@/components/NavBar.vue';
import HomeCotent from '@/components/HomeContent.vue';
import PlansContent from '@/components/PlansContent.vue';
import AuthorName from '@/components/AuthorName.vue';

</script>