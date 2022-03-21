<template>
    <section class="records">
        <div class="main_container">
            <div class="records_text">
                <div class="text-area">
                    <div class="text">
                        <h6>Everything in maxcoach</h6>
                        <h3>Learn about our <span class="water">Work Culture</span> at MaxCoach</h3>
                        <p>
                            Spend some time to visit our website or head office and
                            discover our current courser, enrollment procedure, and
                            registration deadline. We're opening new classes every
                            beginning of each month. 
                        </p>
                        <p>Have questions? <span class="water">Get Free Guide</span></p>
                    </div>
                    <div class="circle-place">
                        <img src="../assets/semi-circle.png">
                    </div>
                </div>
            </div>
            <div class="records_images">
                <div class="image_area">
                    <img class="bottom_one" src="../assets/semi-circle.png">
                    <img class="top_back" src="../assets/grid_150x150.png">
                    <img class="top_front" src="../assets/person_working.jpg">
                </div>
            </div>
        </div>
        <div class="data_container">
            <div class="data_item">
                <h1 class="water">
                    129+
                </h1>
                <p>
                    Enrolled learness
                </p>
            </div>
            <div class="data_item">
                <h1 class="water">
                    80
                </h1>
                <p>
                    finished sessions
                </p>
            </div>
            <div class="data_item">
                <h1 class="water">
                    4%
                </h1>
                <p>
                    satisfaction rate
                </p>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'TheRecordsSection'
}
</script>

<style lang="scss">
    .records{
        width: 100%;
        height: 700px;
        // border: 8px solid yellow;
        display: flex;
        flex-direction: column;
        .main_container{
            // border: 5px solid blue;
            width: 100%;
            height: 80%;
            display: flex;
            align-items: center;
            .records_text{
                // border: 3px dashed green;
                width: 50%;
                height: 100%;
                display: flex;
                align-items: center;
                justify-content: center;
                .text-area{
                    // border: 2px solid purple;
                    width: 60%;
                    height: 70%;
                    display: flex;
                    .text{
                        width: 70%;
                        // border: 1px solid red;
                        padding: 0px 10px;
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
                    }
                    .text > *{
                        padding: 10px 0px;
                    }
                    .circle-place{
                        // border: 2px solid red;
                        width: 30%;
                        display: flex;
                        flex-direction: row;
                        justify-content: flex-end;
                        img{
                            margin-top: 10%;
                            width: 45%;
                            height: 20%;
                        }
                    }
                }
            }
            .records_images{
                // border: 3px dashed green;
                width: 50%;
                height: 100%;
                display: flex;
                align-items: center;
                justify-content: center;
                .image_area{
                    width: 60%;
                    height: 50%;
                    // border: 1px solid red;
                    background-image: url('~@/assets/people-talking.jpg');
                    background-size: cover;
                    background-repeat: no-repeat;
                    background-position: center;
                    position: relative;
                    z-index: 9999;
                    .bottom_one{
                        position: absolute;
                        bottom: 0;
                        right: 0;
                        transform: translate(-50%, 70%);
                        width: 15%;
                    }
                    .top_back{
                        position: absolute;
                        top: 0;
                        right: 0;
                        transform: translate(0%, -30%);
                        width: 25%;
                        z-index: 1;
                    }
                    .top_front{
                        position: absolute;
                        width: 25%;
                        top: 0;
                        right: 0;
                        transform: translate(20%, -30%);
                        z-index: 2;
                    }
                }
            }
        }
        .data_container{
            // border: 5px solid blue;
            width: 100%;
            height: 20%;
            display: flex;
            flex-direction: row;
            align-items: center;
            padding: 0px 15%;
            .data_item{
                width: calc(100% / 3);
                height: 80%;
                // border: 2px solid red;
                display: flex;
                flex-direction: column;
                align-items: center;
                justify-content: center;
                h1{
                    font-size: 48px;
                    font-weight: 700;
                }
                p{
                    text-transform: uppercase;
                    font-size: 16px;
                }
            }
        }
        .water{
            color: #1fad95;
            font-weight: 700;
        }
    }
</style>