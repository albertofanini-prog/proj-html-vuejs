<template>
    <section class="testimonial_section">
        <div class="testimonial_container">
            <div class="testimonial_title">
                <div class="title">                        
                    <h6>testimonials</h6>
                    <h3>Why do people <span class="water">*Hearts*</span> Us?</h3>
                    <p>
                        Seeking for verbals of our service quality? Find them here.
                        Everything is transparent and straightforward for your sense
                        of justification.
                    </p>
                    <p>View all</p>
                </div>
            </div>
            <div class="testimonial_text">
                <div class="under">
                    <h5 class="testimoniance">
                        The MaxCoach team works really hard to enuser hight level
                        of quality
                    </h5>
                    <p>
                        I am happy with the arrangement of lessons and subjects. They
                        are special.
                    </p>
                    <div class="user">
                        <img class="user_id" src="../assets/mina.jpg" alt="">
                        <div class="infos">
                            <h3>mina hollace</h3>
                            <h5>/ Freelancer</h5>
                        </div>
                    </div>
                </div>
                <div class="over">
                    <h5 class="testimoniance">
                        Professional team of specialists and passionate mentors at reach
                    </h5>
                    <p>
                        I need to get a certification for English proficiency and MaxCoach is
                        my best choice. Their tutors are smart and professional when dealing
                        with students.
                    </p>
                    <div class="user">
                        <img class="user_id" src="../assets/madley.jpg" alt="">
                        <div class="infos">
                            <h3>madley pondor</h3>
                            <h6>/ IT Specialist</h6>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>


<script>
export default {
    
}
</script>


<style lang="scss">
    .testimonial_section{
        width: 100%;
        height: 700px;
        // border: 7px solid red;
        display: flex;
        align-items: center;
        .testimonial_container{
            width: 80%;
            height: 90%;
            // border: 5px solid yellow;
            display: flex;
            align-items: center;
            justify-content: center ;
            .testimonial_title{
                width: 50%;
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
                    h6{
                        text-transform: uppercase;
                        font-size: 14px;
                        color: #6c6c6b;
                    }
                    h3{
                        font-size: 44px;
                        font-weight: 700;
                        .water{
                            color: #1fad95;
                            font-weight: 500;
                        }
                    }
                    p{
                        font-size: 16px;
                        color: #6c6c6b;
                    }
                }
                .text > *{
                    padding: 10px 0px;
                }
            }
            .testimonial_text{
                width: 50%;
                height: 100%;
                // border: 3px solid green;
                position: relative;
                .under{
                    width: 50%;
                    height: 95%;
                    // border: 3px solid purple;
                    position: absolute;
                    top: 0;
                    left: 0;
                    transform: translate(50%, 3%);
                    // background-color: yellow;
                    display: flex;
                    flex-direction: column;
                    justify-content: space-between;
                    padding: 10px;
                    opacity: 0.3;
                    box-shadow: 0 1px 1px rgba(0,0,0,0.11), 
                                0 2px 2px rgba(0,0,0,0.11), 
                                0 4px 4px rgba(0,0,0,0.11), 
                                0 8px 8px rgba(0,0,0,0.11), 
                                0 16px 16px rgba(0,0,0,0.11), 
                                0 32px 32px rgba(0,0,0,0.11);
                    border-radius: 20px;
                    .testimoniance{
                        font-weight: 700;
                        height: 5%;
                        font-size: 18px;
                        margin-bottom: 35px;
                    }
                    p{
                        height: 70%;
                        font-size: 14px;
                    }
                    .user{
                        height: 15%;
                        // border: 1px solid green;
                        width: 100%;
                        display: flex;
                        align-items: center;
                        gap: 20px;
                        img{
                            width: 20%;
                            height: 90%;
                            border-radius: 999px;
                        }
                        .infos{
                            width: 80%;
                            h3{
                                text-transform: uppercase;
                                font-size: 16px;
                            }
                            h5{
                                color: #6c6c6b;
                            }
                        }
                    }
                }
                .over{
                    width: 80%;
                    height: 50%;
                    // border: 3px solid purple;
                    top: 0;
                    left: 0;
                    transform: translate(0%, 50%);
                    // background-color: red;
                    display: flex;
                    flex-direction: column;
                    justify-content: flex-start;
                    gap: 15px;
                    padding: 20px;
                    box-shadow: 0 1px 1px rgba(0,0,0,0.11), 
                                0 2px 2px rgba(0,0,0,0.11), 
                                0 4px 4px rgba(0,0,0,0.11), 
                                0 8px 8px rgba(0,0,0,0.11), 
                                0 16px 16px rgba(0,0,0,0.11), 
                                0 32px 32px rgba(0,0,0,0.11);
                    border-radius: 20px;
                    h5{
                        height: 20%;
                        font-size: 22px;
                    }
                    p{
                        height: 40%;
                        font-size: 16px;
                    }
                    .user{
                        height: 40%;
                        width: 100%;
                        display: flex;
                        align-items: center;
                        gap: 20px;
                        img{
                            width: 20%;
                            height: 100%;
                            border-radius: 999px;
                        }
                        .infos{
                            width: 80%;
                            h3{
                                text-transform: uppercase;
                                font-size: 16px;
                            }
                            h6{
                                color: #6c6c6b;
                                font-size: 14px;
                            }
                        }
                    }
                }
            }
        }
    }
</style>