<script>

export default {
    name: 'AppMain',

}

</script>

<template>
  
    <main>
        <div id="bg-main"></div>

        <div id="comics">

            <div class="container">
                <h2>current series</h2>

                <div class="comic">
                    <img src="/img/dc-logo.png" alt="">
                    <h4>titolo</h4>
                </div>
                <div class="comic">
                    <img src="/img/dc-logo.png" alt="">
                    <h4>titolo</h4>
                </div>
                <div class="comic">
                    <img src="/img/dc-logo.png" alt="">
                    <h4>titolo</h4>
                </div>
                <div class="comic">
                    <img src="/img/dc-logo.png" alt="">
                    <h4>titolo</h4>
                </div>
                <div class="comic">
                    <img src="/img/dc-logo.png" alt="">
                    <h4>titolo</h4>
                </div>
                <div class="comic">
                    <img src="/img/dc-logo.png" alt="">
                    <h4>titolo</h4>
                </div>
                <div class="comic">
                    <img src="/img/dc-logo.png" alt="">
                    <h4>titolo</h4>
                </div>
                <div class="comic">
                    <img src="/img/dc-logo.png" alt="">
                    <h4>titolo</h4>
                </div>
                
            </div>
        </div>


    </main>

  
</template>

<style lang="scss">

@use '../styles/variables.scss' as *;

main {

    background-color: $sec_color;

    #bg-main {
        background-image: url('/img/jumbotron.jpg');
        background-size: cover;
        background-position: top;
        width: 100%;
        height: 400px;
    }

    #comics {

        .container {
            position: relative;
            flex-wrap: wrap;
            gap: 40px 20px;

            // test
            height: 400px;

            .comic {
                display: flex;
                flex-direction: column;
                align-items: center;

                width: calc(100% / 6 - 20px / 6 * 5);

                // test
                border: 1px solid red;
            }

            h2 {
                position: absolute;
                left: 0px;
                top: -20px;

                padding: 12px 18px;

                text-transform: uppercase;
                font-size: 1.3em;

                background-color: $primary_color;
                color: white;

            }

        }

    }

}

</style>