<script>
    export default {
        
    }
</script>

<template>
    <footer>
        <div class="newsletter rounded d-flex">
            <img src="../assets/img/news.png" alt="">
            <div class="d-flex justify-content-center align-items-center flex-column">
                <h5 class="text-white">Subscribe to Our Newsletter</h5>
                <div class="input-group flex-nowrap email">
                    <input type="text" class="form-control" placeholder="Your Email Here">
                    <span class="input-group-text" id="addon-wrapping">@</span>
                </div>
            </div>
        </div>
    </footer>
</template>


<style lang="scss" scoped>
footer {
    background-color: black;
    height: 400px;
    position: relative;

    .newsletter {
        position: relative;
        background-color: #CE7C2A;
        top: -80px;
        height: 150px;
        width: 600px;
        margin: 0 auto;

        .email {
            width: 300px;
        }

        img {
            width: 240px;
            height: 210px;
            position: relative;
            top: -60px;
            margin-right: 50px;
        }
    }

    
}
</style>