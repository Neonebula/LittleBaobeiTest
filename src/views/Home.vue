<template>
  <div class="home">
    <Presentation />
    <MenuSection />
  </div>
</template>

<script>
// @ is an alias to /src
import MenuSection from "@/components/Menu.vue";
import Presentation from "@/components/Presentation.vue";

export default {
  name: "Home",
  components: {
    MenuSection,
    Presentation
  }
};
</script>
