<template>
    <Page>
        <ActionBar>
            <Label text="Vue lessons"/>
        </ActionBar>

        <GridLayout>
            <Lessons />
            <ShoppingCart />
        </GridLayout>
    </Page>
</template>

<script>
  import Lessons from './views/Lessons.vue'
  import ShoppingCart from './views/ShoppingCart.vue'
  export default {
    computed: {
      message() {
        return "Vue Lessons";
      }
    }
  };
</script>

<style scoped lang="scss">
    @import '@nativescript/theme/scss/variables/blue';

    // Custom styles
    .fas {
        @include colorize($color: accent);
    }

    .info {
        font-size: 20;
        horizontal-align: center;
        vertical-align: center;
    }
</style>
