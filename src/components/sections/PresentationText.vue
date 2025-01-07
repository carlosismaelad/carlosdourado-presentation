<template>
  <div class="presentation">
    <h1>
      {{ presentation.initText }}
      <br />
      <span ref="typedElement" class="tech">{{ currentWord }}</span>
      <span>{{ presentation.finalText }}</span>
    </h1>
  </div>
</template>

<script>
import Typewriter from "typewriter-effect/dist/core";
import { presentation } from "../../util/texts/en/presentation";
export default {
  name: "PresentationText",
  data() {
    return {
      presentation,
    };
  },
  mounted() {
    const options = {
      strings: [
        "Java",
        "Node.js",
        "C#",
        "Javascript",
        "Vue.js",
        "React",
        "Back end",
        "Front end",
      ],
      autoStart: true,
      loop: true,
      cursor: "|",
      delay: 75,
      deleteSpeed: 40,
    };

    new Typewriter(this.$refs.typedElement, options);
  },
};
</script>

<style>
.presentation {
  max-width: 11rem;
  display: flex;
  color: beige;
  margin: 2rem auto;
  justify-content: center;
  place-content: center;
  font-weight: 600;
  font-size: 0.8rem;
  overflow: hidden;

}

.tech {
  color: var(--primary-color);
  margin-top: 1rem;
  display: inline-block;
}
</style>
