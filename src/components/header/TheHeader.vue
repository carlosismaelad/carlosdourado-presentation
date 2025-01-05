<template>
    <section class="header-container">
        <div class="logo-container">
            <Logo/>
        </div>
        <div class="button-container">
            <ButtonHeader text="Sobre"/>
            <ButtonHeader text="Projetos"/>
            <ButtonHeader text="Contato"/>
        </div>
    </section>
</template>

<script setup lang="ts">
import Logo from '../logo/Logo.vue'
import ButtonHeader from '../button/TheButton.vue'
</script>

<style>

.header-container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 5rem;
    margin: auto 3rem;
}

.button-container{
    display: flex;
    align-items: left;
    justify-content: flex-end;
}
</style>