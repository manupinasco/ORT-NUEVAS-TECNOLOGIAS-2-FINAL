<template>

  <section class="src-components-text">
    <br>

    Color: <input type="text" v-model.trim="color" style="size: 200px">
    Fondo: <input type="text" v-model.trim="fondo">
    Size: <input type="text" v-model.trim="size">
    <br>
    <br>
    <hr>
    <br>
    Texto: <input type="text" v-model.trim="text" :style="getStyle">
    <br>
    <br>
    Cantidad de palabras {{getCantPalabras}}
  </section>

</template>

<script>

  export default  {
    name: 'src-components-text',
    props: [],
    mounted () {

    },
    data () {
      return {
        text: "",
        fondo: "",
        color: "",
        size: ""
      }
    },
    methods: {

    },
    computed: {
      getStyle() {
        return `background-color: ${this.fondo}; color: ${this.color}; font-size: ${this.size}`
      },
      getCantPalabras() {
        if(this.text.length) {
          return this.text.split(" ").length
        }
        else {
          return 0
        }
      }
    }
}


</script>

<style scoped lang="css">
  .src-components-text {
    
  }
</style>
