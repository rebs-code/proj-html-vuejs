<script>
export default {
    name: 'AppFooterTop',
    data() {
        return {
            socialIcons: [
                {
                    icon: 'fa-brands fa-facebook-f',
                },
                {
                    icon: 'fa-brands fa-twitter',
                },
                {
                    icon: 'fa-brands fa-youtube',
                },
                {
                    icon: 'fa-brands fa-instagram',
                },
                {
                    icon: 'fa-brands fa-linkedin',
                },
            ]
        }
    }
}
</script>

<template>
    <div class="footer-top d-flex align-items-center justify-content-center">
        <div class="footer-info d-flex flex-column align-items-center">
            <img src="../assets/img/logo-restaurant-2x-600x115.png" alt="logo footer" class="mb-5">
            <p class="text-size text-white mb-5">Quam eu proin sit massa condimentum. Voluptat non pulviqar aliquet nunc.
                Quam eu
                proin sit
                massa condimentum.
            </p>
            <ul class="d-flex">
                <li v-for="icon in socialIcons" class="m-2">
                    <div class="social-icon">
                        <font-awesome-icon :icon='icon.icon' />
                    </div>
                </li>
            </ul>
        </div>
    </div>
</template>

<style scoped lang="scss">
.footer-top {
    height: 630px;
    background-image: linear-gradient(to bottom, rgba(0, 0, 0, 1) 0%, rgba(0, 0, 0, 1) 5%, rgba(0, 0, 0, 0) 100%), url('../public/img/footer.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;

    .footer-info {
        width: 40%;
        text-align: center;
    }

    img {
        width: 300px;
    }
}

.social-icon {
    width: 50px;
    height: 50px;
    border-radius: 50%;
    border: 1px solid white;
    /* Set a background color for the circle */
    background-color: white;
    text-align: center;
    line-height: 50px;
    /* vertically center the icon */
    font-size: 24px;
    /* font size for the icon */
    color: black;
    /* color for the icon */
}
</style>