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

            </div>
        </div>
        <div class="data_container">

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
        height: 1000px;
        border: 8px solid yellow;
        display: flex;
        flex-direction: column;
        .main_container{
            border: 5px solid blue;
            width: 100%;
            height: 80%;
            display: flex;
            align-items: center;
            .records_text{
                border: 3px dashed green;
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
                        padding: 10px 10px;
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
                            width: 50%;
                            height: 15%;
                        }
                    }
                }
            }
            .records_images{
                border: 3px dashed green;
                width: 50%;
                height: 100%;
            }
        }
        .data_container{
            border: 5px solid blue;
            width: 100%;
            height: 20%;
        }
        .water{
            color: #1fad95;
            font-weight: 700;
        }
    }
</style>