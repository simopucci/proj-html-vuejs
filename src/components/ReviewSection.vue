<script>
    export default {
        
    }
</script>

<template>
    <section class="review-rating">
        <div class="d-flex gap-4">
            <div class="ratings">
                <div>
                    <img src="../assets/img/dog-icon.png" alt="Zampa">
                    <span>Review & Rating</span>
                </div>
                <h2 class="my-4">Over 8000 Customers With 5-Star Review</h2>
                <p>Its is a long established fact that a reader will be distructed by the readable content of a page when looking at its layout.</p>
                <div class="d-flex">
                    <i v-for="star in 5" class="fa-solid fa-star"></i>
                </div>
            </div>
    
            <div class="reviews">
                <div class="d-flex mb-3">
                    <i v-for="star in 5" class="fa-solid fa-star"></i>
                </div>
                <h5 class="mb-3">Great Place</h5>
                <p class="mb-4">Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda explicabo ut voluptate at fugiat voluptatem non est voluptas rerum dolor?</p>
                <div class="d-flex">
                    <div class="rounded-circle profile me-3"></div>
                    <div>
                        <div class="name mb-2">Tobias May</div>
                        <div class="profession">UI/UX Designer</div>
                    </div>
                </div>
            </div>
    
            <div class="reviews">
                <div class="d-flex mb-3">
                    <i v-for="star in 5" class="fa-solid fa-star"></i>
                </div>
                <h5 class="mb-3">Great Place</h5>
                <p class="mb-4">Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda explicabo ut voluptate at fugiat voluptatem non est voluptas rerum dolor?</p>
                <div class="d-flex">
                    <div class="rounded-circle profile me-3"></div>
                    <div>
                        <div class="name mb-2">Tobias May</div>
                        <div class="profession">UI/UX Designer</div>
                    </div>
                </div>
            </div>
        </div>
        <div class="arrows-box">
            <div class="arrow me-3">
                <img src="../assets/img/left-arrow.png" alt="left arrow">
            </div>
            <div class="arrow">
                <img src="../assets/img/next.png" alt="left arrow">
            </div>
        </div>
    </section>
</template>


<style lang="scss" scoped>

.review-rating {
    width: 70%;
    margin: 0 auto;
    margin-top: 80px;
    margin-bottom: 250px;

    .ratings {
        width: 380px;

        img {
            width: 20px;
        }

        span {
            font-size: .7rem;
            margin-left: 10px;
            color: #7F7045;
            font-weight: bold;
        }

        p {
            font-size: small;
        }

        i {
            color: #FFCC01;
            padding: 0;
        }
    }

    .reviews {
        background-color: rgb(226, 226, 226);
        padding: 20px;
        width: 380px;

        i {
            color: #FFCC01;
            padding: 0;
        }

        p {
            font-size: small;
        }

        img {
            width: 100px;
        }

        .profile {
            width: 50px;
            height: 50px;
            background-image: url('../assets/img/t1.png');
            background-size: cover;
        }

        .profession {
            font-size: .7rem;
        }
    }
}

.arrows-box {
    display: flex;
    justify-content: end;
    align-items: center;

    .arrow {
        background-color: #CE7C2A;
        margin-top: 20px;
        padding: 5px;
        cursor: pointer;

        &:hover {
            background-color: #7F7045;
        }
        
        img {
            width: 30px;
        }
    }
}
</style>