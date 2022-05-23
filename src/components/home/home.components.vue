<template>
    <div id="page-top">
        <navigation-bar/>
        <masthead/>
    </div>
</template>
<script>
import NavigationBar from '@/components/home/partials/NavigationBar.vue';
import Masthead from '@/components/home/partials/MastHead.vue';

export default {
  name: 'home-component',
  components: {
    NavigationBar,
    Masthead,
  },
};
</script>
<style lang="">

</style>
