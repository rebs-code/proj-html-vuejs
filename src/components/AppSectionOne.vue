<script>
import AppCardWhite from './AppCardWhite.vue';
export default {
    name: 'AppSectionOne',
    data() {
        return {
            cardInfo: [{
                cardImage: '../public/img/sushi-1.png',
                cardTitle: 'The Best Table in Town',
                cardText: 'Sed aenean egestas ut aliquam turpis mauris, molestie. Vitae tellus tempor sem id tempus neque, tellus turpis turpis. Morbi tortor id gravida aliquet.',
                buttonText: 'Explore the menu'
            },
            {
                cardImage: '../public/img/sushi-2.png',
                cardTitle: 'Perfect for Groups',
                cardText: 'Quam eu proin sit massa condimentum, Volutpat non pulvinar aliquet nunc. Orci elementum in aliquet a gravida vivamus aliquam turpis vitae.',
                buttonText: 'Make a reservation'
            },
            {
                cardImage: '../public/img/sushi-3.png',
                cardTitle: 'Fresh Produce Everyday',
                cardText: 'Hendrerit amet, volutpat leo non, commodo meacenas scelerisque ticindunt. Morbi voluptate morbi purus quisque sit sagittis orci elementum gravida.',
                buttonText: 'Learn more about us'
            }
            ]
        }
    },
    components: {
        AppCardWhite,
    },


}

</script>
<template>
    <section class="app-section-one">
        <div class="container-fluid px-5">
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
                <AppCardWhite class="col-3 card-white" :cardImage="cardInfo[0].cardImage" :cardTitle="cardInfo[0].cardTitle"
                    :cardText="cardInfo[0].cardText" :buttonText="cardInfo[0].buttonText" />
                <AppCardWhite class="col-3 card-white" :cardImage="cardInfo[1].cardImage" :cardTitle="cardInfo[1].cardTitle"
                    :cardText="cardInfo[1].cardText" :buttonText="cardInfo[1].buttonText" />
                <AppCardWhite class="col-3 card-white" :cardImage="cardInfo[2].cardImage" :cardTitle="cardInfo[2].cardTitle"
                    :cardText="cardInfo[2].cardText" :buttonText="cardInfo[2].buttonText" />

            </div>
        </div>
    </section>
</template>
<style scoped lang="scss">
.app-section-one {
    margin-bottom: 130px;

    .section-1-top {
        display: flex;
        justify-content: space-between;
        align-items: center;

        padding: 130px;

        .section-1-top-left {
            padding: 0 25px 0 25px;
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
        justify-content: center;
        align-items: center;
        padding: 0 20px;

        .card-white {
            margin: 0 10px;
            padding: 0 30px;
            text-align: center;
        }
    }
}
</style>