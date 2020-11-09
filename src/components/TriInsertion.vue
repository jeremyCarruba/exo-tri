<template>
  <div>
    <h1>Je suis le tri par insertion</h1>
    <Cases :list="list"></Cases>
    <button @click="trier">Trier</button>
  </div>
</template>

<script>
import Cases from "@/components/Cases";
export default {
  name: "Tri",
  components: {
    Cases,
  },
  data() {
    return {
      list: [9, 8, 7, 6, 5, 4, 3, 2, 1],
    };
  },
  methods: {
    trier() {
      this.list = this.list.sort();
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
