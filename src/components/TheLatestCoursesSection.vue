<template>
    <section class="thelatestcourses_section">
        <div class="title_container">
            <h6>How we work</h6>
            <h3>Latest Online <span class="water">Courses</span></h3>
        </div>
        <div class="slider_container">
            <div class="course-card">
                <div class="card-image">
                    <img class="square" src="../assets/course_1.jpg">
                </div>
                <div class="card-text">
                    <span class="water">
                        $40.<span class="mini">00</span>
                    </span>
                    <h6>Learning to Write as a Professional Author</h6>
                    <div class="info">
                        <div class="lessons">
                            20 Lessons
                        </div>
                        <div class="subscribes">
                            50 Subscribes
                        </div>
                    </div>
                </div>
            </div>
            <div class="course-card">
                <div class="card-image">
                    <img class="square" src="../assets/course_2.jpg">
                </div>
                <div class="card-text">
                    <span class="water">
                        $0.<span class="mini">00</span>
                    </span>
                    <h6>Customer-centric info-Tech Strategies</h6>
                    <div class="info">
                        <div class="lessons">
                            24 Lessons
                        </div>
                        <div class="subscribes">
                            300 Subscribes
                        </div>
                    </div>
                </div>
            </div>
            <div class="course-card">
                <div class="card-image">
                    <img class="square" src="../assets/course_3.jpg">
                </div>
                <div class="card-text">
                    <span class="water">
                        $19.<span class="mini">00</span>
                    </span>
                    <h6>Open Programming Courses for Everyone: Python</h6>
                    <div class="info">
                        <div class="lessons">
                            37 Lessons
                        </div>
                        <div class="subscribes">
                            62 Subscribes
                        </div>
                    </div>
                </div>
            </div>
        </div>
            <div class="points">
                <ul>
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
                </ul>
            </div>
        <div class="view-more_container">
            <p>
                Control your personal settings to get notified about
                appropriate courses. <span>View all courses</span>
            </p>
        </div>
    </section>
</template>

<script>
export default {
    name: 'TheLatestCoursesSection'
}
</script>

<style lang="scss">
    .thelatestcourses_section{
        background-color: #F7F7F7;
        width: 100%;
        height: 800px;
        // border: 7px solid red;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        .title_container{
            width: 50%;
            height: 20%;
            // border: 5px solid yellow;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
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
        }
        .slider_container{
            width: 100%;
            height: 60%;
            // border: 5px solid yellow;
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 0px 10%;
            gap: 10%;
            .course-card{
                width: calc(100% / 3);
                height: 90%;
                // border: 3px solid green;
                box-shadow: 
                    0 1px 1px rgba(0,0,0,0.11),                                 0 2px 2px rgba(0,0,0,0.11), 
                    0 4px 4px rgba(0,0,0,0.11), 
                    0 8px 8px rgba(0,0,0,0.11), 
                    0 16px 16px rgba(0,0,0,0.11), 
                    0 32px 32px rgba(0,0,0,0.11);
                border-radius: 20px;
                .card-image{
                    width: 100%;
                    height: 55%;
                    // border: 2px dashed blue;
                    img{
                        width: 100%;
                        height: 100%;
                        border-radius: 20px 20px 0px 0px;
                    }
                }
                .card-text{
                    width: 100%;
                    height: 45%;
                    // border: 2px dashed blue;
                    padding: 20px;
                    span{
                        font-size: 24px;
                        font-weight: 700;
                        .mini{
                            font-size: 18px;
                        }
                    }
                    h6{
                        font-size: 26px;
                        padding-bottom: 20px;
                    }
                    .info{
                        display: flex;
                        //flex-direction: row;
                        // border: 1px solid red;
                        justify-content: flex-start;
                        color: #6c6c6b;
                        font-size: 14px;
                        > * {
                            width: 50%;
                        }
                    }
                }
            }
        }
        .points{
            height: 5%;
            display: flex;
            align-items: center;
            justify-content: center;
            ul{
                width: 15%;
                display: flex;
                flex-direction: row;
                align-items: center;
                justify-content: center;
                li{
                    width: 1px;
                };
            }
        }
        .view-more_container{
            width: 50%;
            height: 10%;
            // border: 5px solid yellow;
            display: flex;
            align-items: center;
            justify-content: center;
            p{  
                width: 50%;
                color: #6c6c6b;
                font-size: 18px;
                text-align: center;
                span{
                    color: black;
                    font-weight: 700;
                }
            }
        }
        .water{
            color: #1fad95;
            font-weight: 500;
        }
    }
</style>