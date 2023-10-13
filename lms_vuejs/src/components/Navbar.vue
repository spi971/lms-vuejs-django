<template>
    <nav class="navbar is-primary" role="navigation" aria-label="main navigation">
        <div class="navbar-brand">
            <a class="navbar-item is-size-4" href="/">
                Learny
            </a>

            <a role="button" class="navbar-burger" :class="{ 'is-active': active }" aria-label="menu" aria-expanded="false"
                data-target="navbar-menu" @click="handleBurgerClick">
                <span aria-hidden="true"></span>
                <span aria-hidden="true"></span>
                <span aria-hidden="true"></span>
            </a>
        </div>

        <div id="navbar-menu" class="navbar-menu" :class="{ 'is-active': active }">
            <div class="navbar-start">
                <router-link to="/" class="navbar-item" @click="handleBurgerClick">Home</router-link>
                <router-link to="/about" class="navbar-item" @click="handleBurgerClick">About</router-link>
            </div>

            <div class="navbar-end">
                <div class="navbar-item">
                    <div class="buttons">
                        <router-link to="/signup" class="button is-primary" @click="handleBurgerClick">
                            <strong>Sign up</strong>
                        </router-link>
                        <router-link to="/login" class="button is-light" @click="handleBurgerClick">
                            Log in
                        </router-link>
                    </div>
                </div>
            </div>
        </div>
    </nav>
</template>
<script  setup>
import { ref } from 'vue';
let active = ref(false)

const handleBurgerClick = () => {
    active.value = !active.value;
}
</script>

<style lang="css" scoped>
.navbar {
    min-height: 5rem;
}
</style>