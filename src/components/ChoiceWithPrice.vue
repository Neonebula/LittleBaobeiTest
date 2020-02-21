<template>
  <div>
    <div>{{ choice.name }}</div>
    <div>{{ choice.description }}</div>
    <div>{{ choice.price }}€</div>
  </div>
</template>

<script>
export default {
  name: "ChoiceWithPrice",
  props: {
    choice: Object
  }
};
</script>

<style scoped></style>
