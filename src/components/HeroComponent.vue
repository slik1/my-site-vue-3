<template>
  <section id="hero">
    <div class="big-textbox">
      <h1>Gary Saunders</h1>
      <div class="intro-message">{{ introMsg }}</div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'HeroComponent',
  props: {
    introMsg: String,
  },
};
</script>

<style lang="scss" scoped>

.big-textbox {
  display: flex;
  width: 100%;
  height: calc(100vh - 60px);
  justify-content: center;
  flex-direction: column;
  align-items: center;
  max-width: 480px;
  margin: 0 auto 30px;

  h1 {
    font-size: var(--font-size-landing);
    margin: 1rem 0;
    font-weight: 900;
    text-transform: uppercase;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    line-height: 0.9;
    position: relative;
    display: inline-block;
    z-index: 2;

    &:before{
      content: "";
      display: inline-block;
      border: 10px solid var(--color-light-green);
      position: absolute;
      top: -50px;
      width: 100%;
      height: 100%;
      border-radius: 10px;
      left: -50px;
      z-index: -1;
    }
  }

  .intro-message{
    font-size: var(--font-size-lg);
  }
}

</style>
