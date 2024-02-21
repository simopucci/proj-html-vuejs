<script>
    import CardService from './CardService.vue';

    export default {
        data() {
            return {
                cards: [
                    {
                        image: '../assets/img/d-1.png',
                        title: 'Pet Sitting',
                        content: 'The readable content of a page when looking at its layout.'
                    },
                    {
                        image: '../assets/img/d-2.png',
                        title: 'Puppy Sitting',
                        content: 'The readable content of a page when looking at its layout.'
                    },
                    {
                        image: '../assets/img/d-3.png',
                        title: 'Dog Walking',
                        content: 'The readable content of a page when looking at its layout.'
                    },
                    {
                        image: '../assets/img/d-4.png',
                        title: 'Night Care',
                        content: 'The readable content of a page when looking at its layout.'
                    },
                    {
                        image: '../assets/img/d-5.png',
                        title: 'Pet Sitting',
                        content: 'The readable content of a page when looking at its layout.'
                    },
                ]
            }
        },
        
        components: { CardService }
    }
</script>

<template>
    <section class="service-section py-5">
        <h6>Service</h6>
        <h5>DogMilo Pet Care Services For Your Best Friends.</h5>
        <img src="../assets/img/dog-left.png" alt="Dog" class="dog-left">
        <img src="../assets/img/dog-logo.png" alt="Dog" class="dog-right">
        <CardService
        :cards="cards">
        </CardService>
    </section>
</template>


<style lang="scss" scoped>

.service-section {
    background-color: #F5F5F5;
    position: relative;

    h6 {
        font-size: small;
        text-align: center;
        margin-bottom: 15px;
        color: #7F7045;
    }

    h5 {
        font-weight: 600;
        width: 300px;
        text-align: center;
        margin: 0 auto;
        padding-bottom: 30px;
    }
}

.dog-left {
    position: absolute;
    left: 0;
    top: 50px;
    width: 150px;
}

.dog-right {
    position: absolute;
    right: 0;
    top: 50px;
    width: 200px;
}
</style>