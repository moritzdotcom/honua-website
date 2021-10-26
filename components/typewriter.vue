<template>
  <div style="min-height: 15vw">
    <h1 style="text-align: center; margin-top: 5rem; background: #0009; font-size: 3.5vw">
      <div class="move-on-scroll" data-direction="left">
        <vue-typer
          text="Mission Atlantis"
          :repeat='0'
          :pre-type-delay='1000'
          :type-delay='70'
        >
        </vue-typer>
      </div>
      <div class="move-on-scroll" data-direction="right">
        <vue-typer
          text="Die Geschichte der Menschheit wird neu geschrieben"
          :repeat='0'
          :pre-type-delay='3000'
          :type-delay='70'
        >
        </vue-typer>
      </div>
      <div class="move-on-scroll" data-direction="left">
        <vue-typer
          text="Wilkommen an Bord."
          :repeat='0'
          :pre-type-delay='7000'
          :type-delay='70'
        >
        </vue-typer>
      </div>
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

  .vue-typer .custom.caret {
    display: none;
  }
</style>
