<template>
  <div>
    <p v-text="'Meu texto'"></p>
    <p v-html="myHtml"></p>
<br>
<br>
<br>
<br>
<br>

    <HelloWorld :list="list"></HelloWorld>
  </div>
</template>

<script>
export default {
  name: 'VHtml',

  components: {
    HelloWorld: () => import('../components/HelloWorld.vue'),
  },

  data() {
    return {
      html: 'Minha HTML',
      list: [
        { label: 'label01', id: 1, color: 'red' },
        { label: 'label02', id: 1, color: 'green' },
      ],
    };
  },

  computed: {
    myHtml() {
      return `<div class="bg" >
        <h1>${this.html}</h1>
      </div>
    `;
    },
  },

  mounted() {
  },
};
</script>

<style lang="scss">
.bg {
  background: red;
}
</style>style
