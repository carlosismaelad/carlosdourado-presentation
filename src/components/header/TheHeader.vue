<template>
    <section class="header-container">
        <div class="logo-container">
            <Logo/>
        </div>
        <div>
            <BurgerMenu/>
        </div>
    </section>
</template>

<script setup lang="ts">
import Logo from '../logo/Logo.vue'
import BurgerMenu from '../menu-icon/BurgerMenu.vue'

</script>

<style>

.header-container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 0 1rem;
    height: 3rem;
    margin-left: 1rem;
}

.button-container{
    display: flex;
    align-items: left;
    justify-content: flex-end;
}
</style>