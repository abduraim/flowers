<template>

    <div class="main-container">

        <header-element></header-element>

        <welcome-section></welcome-section>

        <about-section></about-section>

        <welcome-section></welcome-section>

    </div>

</template>

<script>

    import HeaderElement from './elements/HeaderElement';
    import WelcomeSection from './sections/WelcomeSection';
    import AboutSection from './sections/AboutSection'

    export default {
        name: "App",
        components: {
            HeaderElement,
            WelcomeSection,
            AboutSection,
        }
    }
</script>

<style lang="scss" scoped>

    //@import "../../sass/variables";







</style>
