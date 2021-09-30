<template>
  <div>
    <h1 style="text-align: center; margin-top: 3rem; background: #0009">
      <vue-typer
        text="Mission Honua"
        :repeat='0'
        :pre-type-delay='1000'
        :type-delay='70'
      >
      </vue-typer>
      <br>
      <vue-typer
        text="Die Menschheitsgeschichte Neu Erzählt"
        :repeat='0'
        :pre-type-delay='3000'
        :type-delay='70'
      >
      </vue-typer>
      <br>
      <vue-typer
        text="Wilkommen an Board."
        :repeat='0'
        :pre-type-delay='6000'
        :type-delay='70'
      >
      </vue-typer>
    </h1>
  </div>
</template>

<script>
  import { VueTyper } from 'vue-typer'
  export default {
    components: {
      VueTyper
    }
  }
</script>

<style>
  .vue-typer {
  }

  .vue-typer .custom.char.typed {
    color: white;
  }
  .vue-typer .custom.char.selected {
    background-color: transparent;
  }

  .vue-typer .custom.caret {
    display: none;
  }
</style>
