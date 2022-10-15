<template>
  <aside :class="`${expanded && 'is_expanded'}`">
    <div class="logo">
      <img src="../assets/vue.svg" alt="logo">     
    </div>
    <div class="menu-toggle-wrap"  @click="toggleMenu">
      <button class="menu-toggle-class">
        <span class="material-icons">
          keyboard_double_arrow_right
          </span>
      </button>
    </div>
  </aside>
</template>

<script setup>
import { ref } from "vue"
 const expanded = ref (false)

 const toggleMenu = () =>{
  expanded.value =  !expanded.value
 }

</script>

<style lang="scss" scoped>
</style>import logo from "../assets/vue.svg"