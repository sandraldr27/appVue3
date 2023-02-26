<script>
import DirectiveVif from '../components/myComponents/directives/DirectiveVif.vue';
import DirectiveVShow from '../components/myComponents/directives/DirectiveVShow.vue';
import RawHtmlData from '../components/myComponents/RawHtmlData.vue';
import SingleComponent from '../components/myComponents/SingleComponent.vue';
export default {
  components: { SingleComponent, RawHtmlData, DirectiveVShow, DirectiveVif },};
</script>

<template>
    <div>
        <h1>My Single Page from FEMCoder Málaga</h1>
        <h3>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</h3>
        --------------------------------------------------------------------------------------------
        <raw-html-data></raw-html-data> 
        --------------------------------------------------------------------------------------------
        <single-component></single-component>
        <single-component></single-component>
        <single-component></single-component>
        <single-component></single-component>
        --------------------------------------------------------------------------------------------
        <DirectiveVShow></DirectiveVShow>
        --------------------------------------------------------------------------------------------
        <directive-vif></directive-vif>
        --------------------------------------------------------------------------------------------
    </div>
</template> 

<style lang="css" scoped>
h1{
    color: red;
}
</style>
