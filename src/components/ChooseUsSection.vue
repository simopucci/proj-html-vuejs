<script>
    export default {
        
    }
</script>

<template>
     <section class="choose-us d-flex">
        <div class="choose-left">
            <img src="../assets/img/why.png" alt="choose Us">
        </div>

        <div class="about-right m-5">
            <img src="../assets/img/dog-icon.png" alt="Zampa">
            <span class="ms-3">Choose Us</span>
            <h3 class="my-4 fw-semibold">Why Choose Us?</h3>
            <div class="safety">
                <img src="../assets/img/w-3.png" alt="Dog safety">
                <div class="ms-4">
                    <h5 class="fw-semibold">Safety First</h5>
                    <p>Its is a long established fact that a reader will be distructed by the readable content of a page when looking at its layout.</p>
                </div>
            </div>

            <div class="play-yards">
                <img src="../assets/img/w-2.png" alt="playyards">
                <div class="ms-4">
                    <h5 class="fw-semibold">Play Yards</h5>
                    <p>Its is a long established fact that a reader will be distructed by the readable content of a page when looking at its layout.</p>
                </div>
            </div>

            <div class="monitor-pets">
                <img src="../assets/img/w-1.png" alt="monitor pets">
                <div class="ms-4">
                    <h5 class="fw-semibold">Monitor Your Pets</h5>
                    <p>Its is a long established fact that a reader will be distructed by the readable content of a page when looking at its layout.</p>
                </div>
            </div>
        </div>
    </section>
</template>


<style lang="scss" scoped>

.safety {
    display: flex;

    img {
        width: 120px;
    }

    p {
        font-size: .9rem;
    }
}

.play-yards {
    display: flex;
    margin-left: 150px;

    img {
        width: 120px;
    }

    p {
        font-size: .9rem;
    }
}

.monitor-pets {
    display: flex;
    margin-left: 280px;

    img {
        width: 120px;
    }

    p {
        font-size: .9rem;
    }
}

</style>