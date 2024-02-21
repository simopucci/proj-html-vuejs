<script>
    export default {
        props: {
            socials: Array,
            supportLinks: Array,
            aboutLinks: Array,
            faqLinks: Array
        }
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

        <div class="footer-links d-flex">
            <div class="get-in-touch">
                <div class="title">
                    Get In Touch
                </div>
                <div class="question">
                    Have a question for us?
                </div>
                <div class="question">
                    we'll answer your problem here
                </div>
                <div class="socials mt-3">
                    <div v-for="social in socials">
                        <i :class="social.name" :style="social.color"></i>
                    </div>
                </div>
            </div>

            <div class="support">
                <div class="title">Support</div>
                <ul v-for="link in supportLinks">
                    <li><a :href="link.url">{{ link.text }}</a></li>
                </ul>
            </div>

            <div class="about">
                <div class="title">About</div>
                <ul v-for="link in aboutLinks">
                    <li><a :href="link.url">{{ link.text }}</a></li>
                </ul>
            </div>

            <div class="faq">
                <div class="title">Faq</div>
                <ul v-for="link in faqLinks">
                    <li><a :href="link.url">{{ link.text }}</a></li>
                </ul>
            </div>

            <div class="contact">
                <div class="title">Contact Me</div>
                <div class="position-container d-flex">
                    <div>
                        <i class="fa-solid fa-location-arrow"></i>
                    </div>
                    <div class="location">
                        <div>4500 Mercantile plaza, suite</div>
                        <div>300, fort worth,TX,76137,USA</div>
                    </div>
                </div>

                <div class="phone-container d-flex">
                    <div>
                        <i class="fa-solid fa-phone"></i>
                    </div>
                    <div class="phone">
                        +1(817)901 3377
                    </div>
                </div>

                <div class="email-container d-flex">
                    <div>
                        <i class="fa-solid fa-envelope"></i>
                    </div>
                    <div class="email">
                        info@example.com
                    </div>
                </div>
            </div>

        </div>

        <div class="copyright">
            Copyright 2022 by AttDogMilo.com
        </div>
    </footer>
</template>


<style lang="scss" scoped>
footer {
    background-color: black;
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

    .footer-links {
        width: 70%;
        margin: 0 auto;
        padding-bottom: 40px;
        gap: 100px;

        .title {
            color: #CE7C2A;
            margin-bottom: 30px;
        }

        .question {
            font-size: .6rem;
            color: white;
        }

        .socials {
            display: flex;
        }

        ul {
            list-style: none;
            padding: 0;
            line-height: 10px;

            a {
                color: white;
                font-size: .7rem;
            }
        }

        .position-container {
            margin-bottom: 30px;

            .location {
                font-size: .7rem;
                color: white;
            }
        }

        .phone-container {
            margin-bottom: 30px;

            .phone {
                font-size: .7rem;
                color: white;
            }
        }

        .email {
            font-size: .7rem;
            color: white;
        }
    }
    
    .copyright {
        border-top: 1px solid rgb(81, 81, 81);
        text-align: center;
        color: white;
    }
}

i {
    color: #CE7C2A;
    margin-right: 5px;
}
</style>