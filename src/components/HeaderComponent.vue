<template>
  <header class="header">
    <div class="header-title">
      <HeaderWelcome/>
    </div>
    <div class="header-buttons">
      <HeaderButton label="Botão 1" 
      v-show="showButton1" />
      <HeaderButton label="Botão 2" 
      v-if="showButton2" />
      <HeaderButton label="Botão 3" />
      <HeaderButton label="Botão 4" />
    </div>
    
  </header>
</template>

<script>
// Header do projeto
import HeaderButton from "./HeaderButton.vue"
import HeaderWelcome from "./HeaderWelcome.vue";

export default {
  name: "HeaderComponent",
  components: {
    HeaderButton,
    HeaderWelcome
  },
  data(){
    return {
      showButton1: false,
      showButton2: false,
      nome: "vueTest"
    }
  }
};

</script>

<style scoped>
.header{
  display: flex;
  align-items: center;
  justify-content: space-between;
  background-color: #1aa72c;
  padding: 0 20px;
}

.header-title{
  margin-right: auto;
  background-color: antiquewhite;
}

.header-buttons {
  display: flex;;
  padding: 15px;
  gap: 30px;
}
</style>
