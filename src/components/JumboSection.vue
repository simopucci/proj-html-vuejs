<script>
    export default {
        data() {
            return {

            };
        },

    }
</script>

<template>
    <section class="jumbo-box">
        <div class="welcome-box text-white">
            <div class="welcome">
                <h2 class="text-white">
                    <span class="fw-bold">Welcome to</span><br>
                    DogMilo <span class="fw-bold">Pets</span>
                </h2>
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ipsam doloribus veniam officia expedita.</p>
                <div class="d-flex">
                    <button class="btn rounded-pill my-btn">Get Started</button>
                    <button class="btn"><img src="../assets/img/play.png" alt="play button"></button>
                </div>
            </div>  
        </div>
    </section>
</template>


<style lang="scss" scoped>

.jumbo-box {
    background-image: url('../assets/img/b.png');
    background-position: center;
    height: 450px;
    display: flex;
    align-items: center;

    .welcome-box {
        width: 70%;
        margin: 0 auto;
        padding: 30px;

        .welcome {
            max-width: 450px;

            p {
                font-size: smaller;
            }

            
            .my-btn {
                color: white;
                cursor: pointer;
                background-color: #CE7C2A;
                margin-right: 10px;
                padding: 10px 30px;

               &:hover {
                    color: white;
                    background-color: #143D62;
                }
            
            }

            button {
                display: flex;
                justify-content: center;
                align-items: center;
                background-color: rgb(115, 199, 227);
                padding: 10px;

                img {
                    width: 25px;
                }

                &:hover {
                    color: white;
                    background-color: #143D62;
                }
            }
        }    
    }
}

</style>