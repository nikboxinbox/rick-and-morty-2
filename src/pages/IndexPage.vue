<template lang="pug">
q-page
  .characters__list
    CharacterList
  q-page-sticky.pagination-container(position="bottom" :offset="[0, 18]")
    PaginationComponent

</template>

<script>
// Components
import CharacterList from "../components/CharactersList.vue";
import PaginationComponent from "../components/PaginationComponent.vue";

export default {
  components: {
    CharacterList,
    PaginationComponent
  },
  name: "IndexPage"
};
</script>
<style lang="stylus">
q-page
  padding-top 100px
</style>
