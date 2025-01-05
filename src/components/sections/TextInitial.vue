<template>
    <div class="presentation">
        <h1>Hello! My name is Carlos and i'm a
            <br/>
            <span ref="typedElement" class="tech">{{currentWord}}</span>
            <span>developer!</span>
        </h1>
    </div>
</template>

<script>
import Typewriter from 'typewriter-effect/dist/core';
export default {
  name: "TextInitial",
  mounted() {
    const options = {
      strings: ['Java', 'Node.js', 'C#', 'Javascript', 'Vue.js', 'React', 'Back end', 'Front end'],
      autoStart: true,
      loop: true,
      cursor: '|',
      delay: 75,
      deleteSpeed: 40,
    };

    new Typewriter(this.$refs.typedElement, options);
  },
};

</script>

<style>
.presentation{
    display: flex;
    margin: 5rem auto;
    color: beige;
    place-content: center;
    font-family: "Roboto Mono", sans-serif;
    font-weight: 600;
    font-size: 1.5rem;
    text-wrap: wrap;

}

.tech {
    color: var(--primary-color);
    margin-top: 1rem; 
    display: inline-block;
}


</style>