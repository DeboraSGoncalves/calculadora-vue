<script setup>

</script>

<template>
  <div id="app">
    <h1>Calculadora</h1>
    <div class="calculator">
      <input type="number" v-model="number1" placeholder="Digite o primeiro número" />
      <select v-model="operation">
        <option value="add">Somar</option>
        <option value="subtract">Subtrair</option>
        <option value="multiply">Multiplicar</option>
        <option value="divide">Dividir</option>
      </select>
      <input type="number" v-model="number2" placeholder="Digite o segundo número" />
      <p>Resultado: {{ result }}</p>
    </div>
  </div>
</template>

<style scoped>
#app{
  font-family: Arial, Helvetica, sans-serif;
  text-align: center;
  margin-top: 50px;
}
.calculator{
  display: inline-block;
  text-align: left;

}
input, select{
  display: block;
  margin: 10px 0;
  padding: 5px;
  font-size: 16px;
}


</style>
