<script>
export default {
    name: 'AppCardBlack',

}
</script>

<template>
    <div class="app-card-black">

        <div class="card-content">
            <div class="title">
                <hr>
                <h4>The Best Table in Town</h4>
            </div>
            <div class="info">

                <h2>Fine dining experience</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, voluptatum.</p>
                <button>Explore the menu</button>
            </div>

        </div>

    </div>
</template>

<style scoped lang="scss">
.app-card-black {
    background-color: transparent;
}

.card-content {
    color: white;
    padding: 2rem;
    padding-top: 0;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);


    h2 {
        font-size: 3rem;
        margin-bottom: 70px;
        text-transform: uppercase;
    }

    p {


        margin-bottom: 70px;
    }

    .title {
        display: flex;
        align-items: center;
        margin-bottom: 70px;

        hr {
            border: 1px solid white;
            width: 70px;
        }

        H4 {
            margin-left: 30px;
            font-size: 1.5rem;
        }
    }

    .info {
        margin-left: 100px;

        button {
            max-width: 230px;
            background-color: transparent;
            color: white;
            border: 1px solid white;
            padding: 15px 30px;
            font-size: 0.8rem;
            text-transform: uppercase;
            cursor: pointer;

            &:hover {
                background-color: white;
                color: black;
            }
        }
    }
}
</style>