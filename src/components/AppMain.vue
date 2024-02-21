<script>
    import JumboSection from './JumboSection.vue';
    import AboutUsSection from './AboutUsSection.vue';
    import ServiceSection from './ServiceSection.vue';
    import ChooseUsSection from './ChooseUsSection.vue';
    import ReviewSection from './ReviewSection.vue';

    export default {
        data() {
            return {
                
            };
        },

        components: { JumboSection, AboutUsSection, ServiceSection, ChooseUsSection, ReviewSection }
    }
</script>

<template>
    <JumboSection></JumboSection>
    <AboutUsSection></AboutUsSection>
    <ServiceSection></ServiceSection>
    <ChooseUsSection></ChooseUsSection>
    <ReviewSection></ReviewSection>
</template>

<style lang="scss" scoped>

</style>