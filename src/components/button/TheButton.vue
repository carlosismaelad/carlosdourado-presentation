<template>
    <button class="buttonHeader">{{ text }}</button>
</template>

<script>

export default {
  name: 'ButtonHeader',
  props: {
    text: {
      type: String,
    }
  }
}
</script>


<style>

.buttonHeader{
    background-color: none;
    border: none;
    padding: 4px;
    font-size: 20px;
    font-weight: 600;
    font-family: "Roboto Mono", sans-serif;
    font-weight: 600;
    margin-right: 1rem;
    cursor: pointer;
    color: var(--primary-color);
}



</style>