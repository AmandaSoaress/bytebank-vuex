<template>
  <nav class="navbar navbar-expand-lg navbar-bytebank">
    <a class="navbar-brand" href="#">ByteBank</a>
    <button
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target="#navbarSupportedContent"
      aria-controls="navbarSupportedContent"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse">
      <BarraNavegacaoQuandoLogado v-if="usuarioEstaLogado" />
      <BarraNavegacaoQuandoDeslogado v-else />
    </div>
  </nav>
</template>
<script>
import BarraNavegacaoQuandoLogado from "./BarraNavegacaoQuandoLogado";
import BarraNavegacaoQuandoDeslogado from "./BarraNavegacaoQuandoDeslogado";
import { mapGetters } from "vuex";

export default {
  components: {
    BarraNavegacaoQuandoLogado,
    BarraNavegacaoQuandoDeslogado,
  },
  computed: {
    ...mapGetters(["usuarioEstaLogado"]),
  },
};
</script>
<style>
.navbar {
  background: #b72c79eb;
}
.navbar-bytebank a {
  color: #fff;
}
.navbar-bytebank a:hover {
  color: #000;
}
</style>
