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
            <div class="guide_title">
                <div class="title">                        
                    <h6>everything in <span class="bold">maxcoach</span></h6>
                    <h3>We're Here To <span class="water">Transform</span> You!</h3>
                    <p>
                        As leaners, people can enjoy great companionship from
                        MaxCoach mentors and educators. We can help you
                        develop and grow at your best.
                    </p>
                    <button class="get_guide">Get free guide</button>
                </div>
            </div>
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
                width: 90%;
                // border: 3px solid yellow;
                position: relative;
                .team{
                    position: absolute;
                    top: 0;
                    left: 0;
                    transform: translate(35%, 5%);
                    width: 70%;
                    height: 90%;
                    z-index: 10;
                }
                .square{
                    position: absolute;
                    bottom: 5%;
                    right: 10%;
                    transform: translate(-80%, 50%);
                    width: 175px;
                }
                .cloud{
                    position: absolute;
                    top: 10%;
                    left: 10%;
                    transform: translate(100%, 60%);
                    max-width: 150px;
                    max-height: 150px;
                    filter: invert(78%) sepia(46%) saturate(235%) hue-rotate(120deg) brightness(95%) contrast(87%);
                }
                .rombo{
                    position: absolute;
                    top: 15%;
                    left: 5%;
                    transform: translate(50%, 90%);
                    z-index: 9;
                }
                .linee{
                    position: absolute;
                    left: 5%;
                    bottom: 2%;
                    transform: translate(-0%, -90%);
                }
            }
        }
        .guide_text{
            width: 50%;
            height: 90%;
            // border: 5px solid green;
            display: flex;
            .guide_title{
                width: 80%;
                height: 100%;
                // border: 3px solid green;
                display: flex;
                align-items: center;
                justify-content: center;
                flex-direction: column;
                .title{
                    width: 65%;
                    // border: 1px solid red;
                    padding: 0px 10px;
                    .bold{
                        font-weight: 700;
                    }
                    h6{
                        text-transform: uppercase;
                        font-size: 18px;
                        color: #6c6c6b;
                    }
                    h3{
                        font-size: 48px;
                        font-weight: 700;
                        .water{
                            color: #1fad95;
                            font-weight: 500;
                        }
                    }
                    p{
                        font-size: 18px;
                        color: #6c6c6b;
                    }
                    button{
                        width: 50%;
                        height: 45px;
                        margin-top: 20px;
                        padding: 10px;
                        border: none;
                        background-color: #20ad96;
                        color: white;
                        font-size: 12px;
                        border-radius: 5px;
                    }
                }
                .text > *{
                    padding: 10px 0px;
                }
            }
        }
    }
</style>