<template>
  <div id="main-container">
    <div class="main-inner">
      <HeroComponent introMsg="I'm a Front-End Developer
      designing and building intuitive user interfaces. Also, I couldn't live without music."/>
      <AboutMe :aboutMeText="aboutMeText" :aboutMePic="require('@/assets/me.jpg')"></AboutMe>
    </div>

  </div>
</template>

<script>
import HeroComponent from './components/HeroComponent.vue';
import AboutMe from './components/AboutMe.vue';

export default {
  name: 'App',
  components: {
    HeroComponent,
    AboutMe,
  },
  data() {
    return {
      aboutMeText: 'This is about me text',
    };
  },
};
</script>

<style lang="scss">
body{
  margin: 0;
  font-family: Poppins,sans-serif;
  font-weight: 300;
  line-height: 1.65;
}

:root {
    --color-text: #3b3b3b;
    --color-light-green: #52ff12;
    --color-green: #519a36;
    --color-purple: #4f345a;
    --color-white: #fff;
    --color-light-gray: #c0c5c1;
    --font-size-sm: 0.8rem;
    --font-size-md: 1rem;
    --font-size-lg: 1.25rem;
    --font-size-xl: 3.815rem;
    --font-size-2xl: 4.768rem;
    --font-size-3xl: 5.96rem;
    --font-size-landing: 5.61rem;
    --line-height-sm: 1.25;
    --line-height-md: 1.5;
    --line-height-lg: 1.75;
}

#main-container{
  .main-inner{
    max-width: 1088px;
    margin: 0 auto;
  }
}
</style>
