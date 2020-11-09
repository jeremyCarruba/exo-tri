<template>
  <div class="cases">
    <div v-for="item in list" :key="item" class="case">
      {{ item }}
    </div>
  </div>
</template>

<script>
export default {
  name: "Cases",
  props: ["list"],
};
</script>

<style lang="scss" scoped>
.case {
  background-color: green;
  height: 50px;
  width: 50px;
  border-radius: 15px;
  border: grey 1px solid;
  color: white;
  font-size: 2rem;
  margin: 5px;
}

.cases {
  display: flex;
}
</style>
