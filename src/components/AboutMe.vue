<template>
<section id="about">
    <h2 class="section-header">
        About Me
    </h2>
    <div class="content row">
        <div class="about__text">
            {{aboutMeText}}
        </div>
        <div class="about__pic">
            <img alt="me" :src=aboutMePic />
        </div>
    </div>
</section>
</template>

<script>
export default {
  props: ['aboutMeText', 'aboutMePic'],
  data() {
    return {

    };
  },

};
</script>

<style lang="scss">
</style>
