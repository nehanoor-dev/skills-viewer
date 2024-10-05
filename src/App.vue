<template>  ye main compoenet ha ... is mei sary component ko call krty hn
  <v-app>
    <Navbar /> 
    <v-main>
      <v-container>
        <transition name="fade" mode="out-in">
          <section class="hero" key="hero" style="text-align: center; padding: 50px 0; position: relative;">
            <v-img
              class="rounded-circle profile-image"
              src="https://img.freepik.com/premium-photo/young-software-developer-ai-generated_1059430-18874.jpg"
              width="150"
              height="150"
              style="border: 3px solid #6200ea; position: relative; z-index: 2; margin-bottom: 250px;"
            ></v-img>
            <div class="overlay">
              <h1 class="name">Neha Noor</h1>
              <h2 class="title">Full Stack Developer</h2>
              <p class="tagline">Crafting solutions, one line of code at a time.</p>
            </div>
          </section>
        </transition>
        <transition name="fade" mode="out-in">
          <About key="about" />  <!-- ye about compoent call hoa ha
          -->
        </transition>
        <transition name="fade" mode="out-in">
          <Skills key="skills" />
        </transition>
        <transition name="fade" mode="out-in">
          <Projects key="projects" />
        </transition>
        <transition name="fade" mode="out-in">
          <Contact key="contact" />
        </transition>
      </v-container>
    </v-main>
    <Footer />
  </v-app>
</template>

/** ye script tag mei vue hoti ha  */
<script>
import Navbar from './components/Navbar.vue';
import About from './components/About.vue';
import Skills from './components/Skills.vue';
import Projects from './components/Projects.vue';
import Contact from './components/Contact.vue';
import Footer from './components/Footer.vue';

export default {
  components: {
    Navbar, // ye sary compoent calll kiye ha
    About,
    Skills,
    Projects,
    Contact,
    Footer,
  },
}
</script>

<style>
.fade-enter-active, .fade-leave-active {
  transition: opacity 0.5s ease;
}
.fade-enter, .fade-leave-to {
  opacity: 0;
}
.hero {
  position: relative;
  padding: 50px 0;
 }
.profile-image {
  display: block;
  margin: 0 auto;
}
.overlay {
  position: absolute;
  top: 70%;
  left: 50%;
  transform: translate(-50%, -50%);
  color: #6200ea;
  text-align: center;
  z-index: 1;
}
.name {
  font-family: 'Roboto', sans-serif;
  font-size: 2.5rem;
  margin: 0;
}
.title {
  font-size: 1.5rem;
  color: #333;
  margin: 0;
}
.tagline {
  font-size: 1.2rem;
  color: #555;
}
</style>


