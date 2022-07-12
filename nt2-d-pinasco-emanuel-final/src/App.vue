<template>
  <div id="app">
     <TextStyle />

     <br>
     <br>
     
    <table class="table table-bordered">
      <tr>
        <th>Número de pregunta
        </th>
        <th>Respuesta</th>
      </tr>
      <tr>
        <td>
          1
        </td>
        <td>
          b
        </td>
      </tr>
      <tr>
        <td>
          2
        </td>
        <td>
          c
        </td>
      </tr>
      <tr>
        <td>
          3
        </td>
        <td>
          b
        </td>
      </tr>
      <tr>
        <td>
          4
        </td>
        <td>
          d
        </td>
      </tr>
      <tr>
        <td>
          5
        </td>
        <td>
          d
        </td>
      </tr>

    </table>
  </div>
</template>

<script>
import TextStyle from './components/Text.vue'

export default {
  name: 'App',
  components: {
     TextStyle
  },

}
</script>

<style>
#app {
  padding: 20px;
}
</style>
