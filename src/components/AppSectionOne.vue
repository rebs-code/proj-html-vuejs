<script>
export default {
    name: 'AppSectionOne',


}

</script>
<template>
    <div class="app-section-one px-5">
        <div class="container-fluid">
            <div class="section-1-top">
                <div class="section-1-top-left col-6">
                    <p class="text-size"><span class="fw-bold text-uppercase">Hac tellus, felis risus at</span> mattis
                        mattis. Eget euismod semper eget
                        tortor, donec
                        amet, blandit.
                        Tristisque facilisi faucibus elementum feugiat in nam in feugiat. Ipsum odio etiam dius facilis amet
                        vulputate.</p>
                    <h2 class="text-uppercase fw-bold">Food is our common ground, a universal experience.</h2>
                    <p class="text-size">Tristique tempus condimentum diam donec. Condimentuim ullamcorper sit elementum
                        gendrerit mi nilla in
                        consequat, ut. Metus, nullam scelerisque netus viverra dui.</p>
                    <img src="../assets/img/signature.jpg" alt="Chef Signature">
                </div>
                <div class="section-1-top-right col-6">
                    <img src="../assets/img/info22x.jpg" alt="Chef" class="w-100">
                    <h6 class="text-size">California Rolls - $22</h6>
                </div>

            </div>
            <div class="section-1-bottom">

            </div>
        </div>
    </div>
</template>
<style scoped lang="scss">
.app-section-one {
    .section-1-top {
        display: flex;
        justify-content: space-between;
        align-items: center;

        padding: 130px;

        .section-1-top-left {
            padding: 0 50px 0 50px;
            margin-right: 50px;

            p {
                margin-bottom: 60px;
            }

            h2 {
                margin-bottom: 60px;
                line-height: 1.4;
                font-size: 2.5rem;
            }

            img {
                width: 200px;
            }
        }

        .section-1-top-right {
            position: relative;

            h6 {
                margin-top: 30px;
                font-weight: 400;
                text-transform: uppercase;
                position: absolute;
                left: 50%;
                bottom: 5%;
                transform: translateX(-50%);
                color: white;
                font-weight: bold;
            }
        }
    }

    .section-1-bottom {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
}
</style>