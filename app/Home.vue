<template>
    <Page>
        <ActionBar>
            <Label text="Vue lessons"/>
        </ActionBar>

        <GridLayout>
            <Lessons />
            <Checkout />
        </GridLayout>
    </Page>
</template>

<script>
  import Lessons from './views/Lessons.vue'
  import Checkout from './views/Checkout.vue'
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
