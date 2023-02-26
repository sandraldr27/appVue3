<script>
import RawHtmlData from '../components/myComponents/RawHtmlData.vue';
import SingleComponent from '../components/myComponents/SingleComponent.vue';
export default {
  components: { SingleComponent, RawHtmlData },};
</script>

<template>
    <div>
        <h1>My Single Page from FEMCoder Málaga</h1>
        <h3>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</h3>
        --------------------------------------------------------------------------------------------
        <single-component></single-component>
        <single-component></single-component>
        <single-component></single-component>
        <single-component></single-component>
        --------------------------------------------------------------------------------------------
        <raw-html-data></raw-html-data> 
        --------------------------------------------------------------------------------------------

    </div>
</template>

<style lang="css" scoped>
h1{
    color: red;
}
</style>
