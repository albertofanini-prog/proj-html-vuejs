<template>
    <section class="trailer_section">
        <div class="trailer_container">
            <div class="trailer_player">
                <div class="player_area">
                    <img class="youtube_player" src="../assets/youtube-play.png" alt="">
                    <img class="cloud" src="../assets/cloud.svg">
                    <img class="rombo" src="../assets/rombo.png">
                    <img class="square" src="../assets/grid_150x150.png">
                </div>
            </div>
            <div class="trailer_text">
                <div class="player_text_area">
                    <div class="player_text">
                        <h6>How we work</h6>
                        <h3>Upgrade Your Skills <span class="water">Upgrade Your Life</span></h3>
                        <p>
                            Opening up more opportunities in front of you to get the
                            ticketto more enjoyable door in life. Getting equipped width
                            new skills for new sets of insights into your career.
                            MaxCoach accompany learners in every stage of learning.
                        </p>
                        <button>Download free guidebook</button>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'TheTrailerSection'
}
</script>

<style lang="scss">
    .trailer_section{
        width: 100%;
        height: 900px;
        // border: 5px solid green;
        display: flex;
        align-items: center;
        .trailer_container{
            width: 100%;
            height: 80%;
            // border: 3px solid red;
            display: flex;
            align-items: center;
            .trailer_player{
                width: 60%;
                height: 100%;
                // border: 3px solid orange;
                display: flex;
                align-items: center;
                .player_area{
                    width: 70%;
                    height: 75%;
                    // border: 1px solid red;
                    background-image: url('~@/assets/phone_call.jpg');
                    background-size: cover;
                    background-repeat: no-repeat;
                    background-position: center;
                    position: relative;
                    z-index: 9999;
                    .youtube_player{
                        position: absolute;
                        top: 50%;
                        left: 50%;
                        transform: translate(-50%, -50%);
                        cursor: pointer;
                    }
                    .cloud{
                        width: 125px;
                        height: 125px;
                        position: absolute;
                        top: 0;
                        left: 0;
                        transform: translate(-40%, -50%);
                        filter: invert(100%) sepia(0%) saturate(5464%) hue-rotate(158deg) brightness(107%) contrast(77%);
                    }
                    .rombo{
                        width: 125px;
                        height: 125px;
                        position: absolute;
                        top: 0;
                        left: 0;
                        transform: translate(-65%, 20%);
                    }
                    .square{
                        width: 125px;
                        height: 125px;
                        position: absolute;
                        bottom: 0;
                        right: 0;
                        transform: translate(10%, 50%);
                    }
                }
            }
            .trailer_text{
                width: 40%;
                height: 100%;
                // border: 3px solid orange;
                display: flex;
                align-items: center;
                justify-content: center;                
                .player_text_area{
                    width: 50%;
                    height: 65%;
                    // border: 1px solid blue;
                    display: flex;
                    .player_text{
                        // width: 70%;
                        padding: 0px 10px;
                        // border: 1px solid brown;
                        h6{
                            text-transform: uppercase;
                            font-size: 14px;
                            color: #6c6c6b;
                        }
                        h3{
                            font-size: 44px;
                            .water{
                                color: #1fad95;
                                font-weight: 500;
                            }
                        }
                        p{
                            font-size: 16px;
                        }
                        button{
                            margin-top: 10px;
                            background-color: white;
                            padding: 5px;
                            border: 1px solid black;
                            box-shadow: 10px;
                            font-size: 12px;
                        }
                    }
                    .text > *{
                        padding: 10px 0px;
                    }
                }
            }
        }
    }
</style>