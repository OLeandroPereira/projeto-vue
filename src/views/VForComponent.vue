<template>
    <body>
      <div>
        <ul>
          <li v-for="(item, i) in list" :key="i">{{ item.id }}</li>
        </ul>
      </div>
    </body>
</template>

<script>
export default {
  data() {
    return {
      list: [
        { label: 'label01', id: 1 },
        { label: 'label02', id: 1 },
      ],
    };
  },
};
</script>
