<script>
    import JumboSection from './JumboSection.vue';
    import AboutUsSection from './AboutUsSection.vue';
    import ServiceSection from './ServiceSection.vue';
    import ChooseUsSection from './ChooseUsSection.vue';

    export default {
        data() {
            return {
                
            };
        },

        components: { JumboSection, AboutUsSection, ServiceSection, ChooseUsSection }
    }
</script>

<template>
    <JumboSection></JumboSection>
    <AboutUsSection></AboutUsSection>
    <ServiceSection></ServiceSection>
    <ChooseUsSection></ChooseUsSection>
</template>

<style lang="scss" scoped>

</style>