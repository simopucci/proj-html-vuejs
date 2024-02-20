<script>
    export default {
        
    }
</script>

<template>
    <section class="about-us my-5 d-flex">
        <div class="about-left">
            <img src="../assets/img/about.png" alt="About Us">
        </div>

        <div class="about-right m-5">
            <img src="../assets/img/dog-icon.png" alt="Zampa">
            <span>About Us</span>
            <h3 class="my-3">Welcome DogMilo Pets</h3>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit iure ipsam laboriosam magnam ab dicta dolore repellat aut quos earum odio fugit temporibus consectetur, cumque dolorum eos at esse dolor!</p>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sapiente nam, iure reiciendis perspiciatis maiores quia, at ad cumque asperiores illum saepe labore! Possimus deleniti non veritatis eveniet consequuntur reprehenderit dolore.</p>
        </div>
        <img src="../assets/img/dog-logo.png" alt="" class="dog-logo">
    </section>
</template>


<style lang="scss" scoped>
    .about-us {
        width: 70%;
        margin: 0 auto;
    }

    .about-left {

        img {
            width: 300px;
            cursor: pointer;
        }
    }

    .about-right {

        position: relative;

        img {
            margin-right: 15px;
            cursor: pointer;
        }

        span {
            font-size: small;
        }

        p {
            font-size: smaller;
        }

    }
.dog-logo {
    position: absolute;
    right: 0;
    width: 200px;
}
</style>