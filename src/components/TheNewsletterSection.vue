<template>
    <section class="newsletter_section">
        <div class="circle">
            <img class="left_one" src="../assets/semi-circle.png">
        </div>
        <div class="form">
            <div class="form_wrapper">
                <h1>Subscribe <span class="water">Newsletter</span></h1>
                <p>
                    Enter your email address to register to our newsletter subscription
                    delivered on a regular basis!
                </p>
                <div class="inputs">
                    <input type="text" placeholder="Enter your email">
                    <button>Subscribe</button>
                </div>
            </div>
        </div>
        <div class="patches">
            <img class="right_one" src="../assets/semi-circle.png">
            <img class="right_two" src="../assets/ret-obl.png">
        </div>
    </section>
</template>

<script>
export default {
    name: 'TheNewsletterSection'
}
</script>

<style lang="scss">
    .newsletter_section{
        width: 100%;
        height: 350px;
        // border: 7px solid red;
        display: flex;
        align-items: center;
        .circle{
            width: 30%;
            height: 80%;
            // border: 5px solid yellow;
            display: flex;
            align-items: center;
            img{
                width: 17%;
                height: 35%;
            }
        }
        .form{
            width: 40%;
            height: 80%;
            // border: 5px solid yellow;
            display: flex;
            align-items: center;
            .form_wrapper{
                width: 80%;
                height: 80%;
                // border: 3px solid purple;
                display: flex;
                flex-direction: column;
                align-items: center;
                justify-content: center;
                gap: 20px;
                h1{
                    font-size: 46px;
                    .water{
                        color: #1fad95;
                        font-weight: 500;
                    }
                }
                p{
                    text-align: center;
                    font-size: 18px;
                    color: grey;
                }
                .inputs{
                    width: 100%;
                    display: flex;
                    align-items: center;
                    padding: 0px 10px;
                    input{
                        flex-grow: 1;
                        height: 50px;
                        background-color: #f5f5f5;
                        border: none;
                        padding: 0px 10px;
                        font-weight: 600;
                        border-radius: 5px 0px 0px 5px;
                        outline: none;
                    }
                    button{
                        width: 15%;
                        height: 50px;
                        border: none;
                        background-color: #20ad96;
                        color: white;
                        border-radius: 0px 5px 5px 0px;
                        cursor: pointer;
                    }
                }
            }
        }
        .patches{
            width: 30%;
            height: 80%;
            // border: 5px solid yellow;
            position: relative;
            .right_one{
                position: absolute;
                top: 0;
                left: 0;
                transform: translate(80%, 90%);
                z-index: 9;
            }
            .right_two{
                width: 35%;
                position: absolute;
                top: 0;
                left: 0;
                transform: translate(20%, 5%);
                z-index: 8;
            }
        }
    }
</style>