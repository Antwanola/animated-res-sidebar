<template>
  <aside :class="`${expanded && 'is_expanded'}`" >
    <div class="logo">
      <img src="../assets/vue.svg" alt="logo"/>     
    </div>
    <div class="menu-toggle-wrap"  @click="toggleMenu">
      <button class="menu-toggle-class">
        <span class="material-icons">
          keyboard_double_arrow_right
          </span>
      </button>
    </div>
    <h4>Menu</h4>
  <div class="menu">
    <router-link class="button" to="/">
      <span class="material-icons">home</span>
      <span class="text">Home</span>
    </router-link>

    <router-link class="button" to="/about">
      <span class="material-icons">assignment</span>
      <span class="text">About</span>
    </router-link>

    <router-link class="button" to="/">
      <span class="material-icons">visibility</span>
      <span class="text">Team</span>
    </router-link>

    <router-link class="button" to="/">
      <span class="material-icons">email</span>
      <span class="text">contact us</span>
    </router-link>
  </div>
  </aside>

  
</template>

<script setup>
import { ref } from "vue"
 const expanded = ref (false)

 const toggleMenu = () => expanded.value =  !expanded.value


</script>

