<template>
    <section class="guide_section">
        <div class="guide_images">
            <div class="images_container">
                <img class="team" src="../assets/team2.png">
                <img class="square" src="../assets/grid_150x150.png">
                <img class="cloud" src="../assets/cloud.svg">
                <img class="rombo" src="../assets/rombo.png">
                <img class="linee" src="../assets/lines.png">
            </div>
        </div>
        <div class="guide_text">

        </div>
    </section>
</template>

<script>
export default {
    name: 'TheGuideSection'
}
</script>

<style lang="scss">
    .guide_section{
        width: 100%;
        height: 800px;
        // border: 7px solid red;
        display: flex;
        align-items: center;
        justify-content: center;
        .guide_images{
            width: 50%;
            height: 90%;
            // border: 5px solid green;
            display: flex;
            align-items: center;
            justify-content: center;
            .images_container{
                height: 80%;
                width: 80%;
                // border: 3px solid yellow;
                position: relative;
                .team{
                    top: 0;
                    left: 0;
                    transform: translate(35%, 5%);
                    width: 70%;
                    height: 90%;
                }
                .square{
                    position: absolute;
                    bottom: 0;
                    right: 0;
                    transform: translate(-130%, 30%);
                }
                .cloud{
                    position: absolute;
                    top: 0;
                    left: 0;
                    transform: translate(100%, 60%);
                    max-width: 150px;
                    max-height: 150px;
                    filter: invert(53%) sepia(64%) saturate(405%) hue-rotate(121deg) brightness(93%) contrast(95%);
                }
                .rombo{
                    position: absolute;
                    top: 0;
                    left: 0;
                    transform: translate(50%, 90%);
                }
                .linee{
                    position: absolute;
                    left: 0;
                    bottom: 0;
                    transform: translate(-50%, -90%);
                }
            }
        }
        .guide_text{
            width: 50%;
            height: 90%;
            border: 5px solid green;
        }
    }
</style>