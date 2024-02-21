<script>
    export default {
        data() {
            return {

            }
        },

        props: {
            cards: Array,
            logoPath: String,

        },

        methods: {
            generatePath(path) {
                return new URL(path, import.meta.url).href;
            },
        },
    }
</script>

<template>
    <div class="card-section">
        <div class="card-container" v-for="card in cards">
            <div class="card-box">
                <img :src="generatePath(card.image)" alt="" >
                <div class="title">{{ card.title }}</div>
                <p class="text-center">{{ card.content }}</p>
                <div class="circle rounded-circle">
                    <img src="../assets/img/right.png" alt="arrow next" class="arrow">
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>

.card-section {
    display: flex;
    justify-content: center;
    gap: 30px;

    .card-container {
        background-color: #CE7C2A;
        border-radius: 70px;
        padding: 10px;
        width: 130px;

        &:hover {
            background-color: #7F7045;
        }
        
        .card-box {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            color: white;
            padding: 10px;
    
            img {
                width: 40px;
                height: 40px;
                margin-bottom: 10px;
            }
    
            .title {
                font-size: .7rem;
                font-weight: bold;
                margin-bottom: 5px;
            }

            p {
                font-size: .6rem;
            }

            .circle {
                display: flex;
                justify-content: center;
                align-items: center;
                background-color: #FFCC01;
                width: 40px;
                height: 40px;
                position: relative;
                cursor: pointer;

                &:hover {
                    background-color: #6d603b;
                }
                
                .arrow {
                    width: 10px;
                    height: 20px;
                    position: absolute;
                    top: 12px;
                }
            }
        }
    }
}


</style>