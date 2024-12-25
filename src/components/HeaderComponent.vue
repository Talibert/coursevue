<template>
  <header class="header">
    <HeaderButton label="Botão 1" />
    <HeaderButton label="Botão 2" />
    <HeaderButton label="Botão 3" />
    <HeaderButton label="Botão 4" />
  </header>
</template>

<script>
// Header do projeto
import HeaderButton from "./HeaderButton.vue"

export default {
  name: "HeaderComponent",
  components: {
    HeaderButton,
  },
};

</script>

<style scoped>
.header {
  display: flex;
  justify-content: space-around;
  align-items: center;
  background-color: #1aa72c;
  padding: 20px;
}
</style>
