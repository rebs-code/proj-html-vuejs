<script>
export default {
    name: 'AppSectionOne',


}

</script>
<template>
    <div class="app-section-one">
        <div class="container-fluid">
            <div class="section-1-top">
                <div class="section-1-top-left col-6">
                    <p class="text-size">Hac tellus, felis risus at mattis mattis. Eget euismod semper eget tortor, donec
                        amet, blandit.
                        Tristisque facilisi faucibus elementum feugiat in nam in feugiat. Ipsum odio etiam dius facilis amet
                        vulputate.</p>
                    <h2 class="text-uppercase fw-bold">Food is our common ground, a universal experience.</h2>
                    <p class="text-size">Tristique tempus condimentum diam donec. Condimentuim ullamcorper sit elementum
                        gendrerit mi nilla in
                        consequat, ut. Metus, nullam scelerisque netus viverra dui.</p>
                    <img src="../assets/img/signature.jpg" alt="Chef Signature">
                </div>

            </div>
            <div class="section-1-bottom">

            </div>
        </div>
    </div>
</template>
<style scoped lang="scss">
.app-section-one {
    padding: 130px;

    .section-1-top {
        display: flex;
        justify-content: space-between;
        align-items: center;

        .section-1-top-left {
            padding: 60px;

            p {
                color: #999;
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
    }

    .section-1-bottom {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
}
</style>