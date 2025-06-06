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

    <main>
      <BackgroundImage>
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
      </BackgroundImage>
    </main>

    <footer>
      <AuthorName/>
    </footer>

  </ContainerComponent>
</template>

<script setup>
import NavLink from '@/components/NavLink.vue';
import NavBar from '@/components/NavBar.vue';
import NavRow from '@/components/NavRow.vue';
import LogoImage from '@/components/LogoImage.vue';
import BackgroundImage from '@/components/BackgroundImage.vue';
import HomeCotent from '@/components/HomeContent.vue';
import AuthorName from '@/components/AuthorName.vue';
import ContainerComponent from '@/components/ContainerComponent.vue';
import { Container } from 'postcss';
function handleClick() {
  alert("Hello from Vue 3 + Tailwind 4!")
}

</script>
