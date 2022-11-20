<template>
  <div class="about">
    <h1 v-if="show">This is an about page</h1>

    <button @click="hide">Esconder / Mostrar</button> {{ show }}
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      show: true,
    };
  },

  methods: {
    hide() {
      this.show = !this.show;
    },
  },
};
</script>
