<template>
  <div class="menu">
    <h1>Menu</h1>
    <h3>Choix du pain :</h3>
    <div class="flex">
      <div>Bao</div>
      <div class="separateur">|</div>
      <div>Ramen</div>
    </div>
    <ChoiceWithPrice
      v-for="choice in choices"
      :key="choice.name"
      :choice="choice"
    />
  </div>
</template>

<script>
import ChoiceWithPrice from "@/components/ChoiceWithPrice.vue";

export default {
  name: "MenuSection",
  data() {
    return {
      choices: [
        { name: "Beef classic", description: "Lorem Impsum", price: 10 },
        { name: "Chick crousti", description: "Lorem Impsum", price: 11 },
        { name: "Fish crousti", description: "Lorem Impsum", price: 13 },
        { name: "Beef festif", description: "Lorem Impsum", price: 13 },
        { name: "Veggie cheese", description: "Lorem Impsum", price: 12 }
      ]
    };
  },
  components: {
    ChoiceWithPrice
  }
};
</script>

<style scoped>
.flex {
  display: flex;
  justify-content: center;
}
.separateur {
  margin-left: 5px;
  margin-right: 5px;
}
</style>
