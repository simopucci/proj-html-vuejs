<script>
    export default {
        data() {
            return {
                activeLink: 0,
            };
        },

        props: {
            headerLinks: Array,
            logoPath: String,
            socials: Array,
        },

        methods: {
            generatePath(path) {
                return new URL(path, import.meta.url).href;
            },

            linkClick(index) {
                this.activeLink = index;
            },
        },
    }
</script>

<template>
    <!-- Top header -->
    <div class="top-header">
        <div class="contact-box">
            <div class="contacts">
                <i class="fa-solid fa-envelope" style="color: #CE7C2A;"></i><span>info@example.com</span>

                <i class="fa-solid fa-phone" style="color: #CE7C2A;"></i><span>+1(817)901 3377</span>
            </div>
            <div class="socials" >
                <div v-for="social in socials">
                    <i :class="social.name" :style="social.color"></i>
                </div>
            </div>
        </div>
    </div>
    <header>
        <!-- Bottom header -->
        <div class="header-box d-flex">
            <!-- Logo -->
            <div class="logo">
                <img :src="generatePath(logoPath)" alt="Logo">
            </div>
            
            <!-- Nav -->
            <nav class="d-flex align-items-center">
                <ul>
                    <li v-for="(link, i) in headerLinks" @click="linkClick(i)">
                        <a :href="link.url" :class="{'active': i == activeLink}">{{ link.text }}</a>
                    </li>
                </ul>
                <!-- Button -->
                <button class="btn rounded-pill">Get In Toch!</button>
            </nav>
        </div>

    </header>
</template>

<style lang="scss" scoped>
.top-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #7F7045;
    width: 100%;
    height: 45px;
    padding: 0 40px;

    .contact-box {
        display: flex;
        justify-content: space-between;
        width: 70%;
        margin: 0 auto;

        .contacts {
            color: rgb(253, 254, 237);
            font-size: smaller;

            span {
                margin-right: 30px;
            }
        }

        .socials {
            display: flex;

            i {
                cursor: pointer;
                font-size: larger;
            }
        }
    }

}

header {
  
  width: 70%;
  margin: 0 auto;

  
  .header-box {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 10px 20px;
    }
}

.logo img {
  max-height: 50px;
}

nav ul {
  list-style-type: none;
  margin: 0;
  padding: 0;

  li {
    display: inline-block;
    margin-right: 30px;
  }

  li a {
    font-weight: 500;
  }
}

button {
    color: white;
  cursor: pointer;
  background-color: #CE7C2A;

  &:hover {
    color: white;
    background-color: #143D62;
  }
}

.active {
    color: #CE7C2A;
}

</style>