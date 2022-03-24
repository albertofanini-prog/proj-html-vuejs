<template>
    <section class="artists_section">
        <div class="title_container">
            <h6>read for more joyment</h6>
            <h3>Latest From <span class="water">Our Blogs</span></h3>
        </div>
        <div class="slider_container">
            <div class="artist-card">
                <div class="card-image">
                    <img class="square" src="../assets/artist1.jpeg">
                </div>
                <div class="card-text">
                    <span class="card_title">
                        artist
                    </span>
                    <h6>Brush Strokes Energize Trees In Paintings</h6>
                    <div class="info">
                        <div class="lessons">
                            <img src="../assets/Icons/calendar-days-solid.svg" alt=""> May 15, 2020
                        </div>
                        <div class="subscribes">
                            <img src="../assets/Icons/user-solid.svg" alt=""> 688 views
                        </div>
                    </div>
                </div>
            </div>
            <div class="artist-card">
                <div class="card-image">
                    <img class="square" src="../assets/artist2.jpg">
                </div>
                <div class="card-text">
                    <span class="card_title">
                        artist
                    </span>
                    <h6>Pocket-Sized Notebooks Hold Miniature Paintings</h6>
                    <div class="info">
                        <div class="lessons">
                            <img src="../assets/Icons/calendar-days-solid.svg" alt=""> May 15, 2020
                        </div>
                        <div class="subscribes">
                            <img src="../assets/Icons/user-solid.svg" alt=""> 603 views
                        </div>
                    </div>
                </div>
            </div>
            <div class="artist-card">
                <div class="card-image">
                    <img class="square" src="../assets/artist3.jpg">
                </div>
                <div class="card-text">
                    <span class="card_title">
                        artist
                    </span>
                    <h6>Connection Between Self-Potraits and Identity</h6>
                    <div class="info">
                        <div class="lessons">
                            <img src="../assets/Icons/calendar-days-solid.svg" alt=""> May 15, 2020
                        </div>
                        <div class="subscribes">
                            <img src="../assets/Icons/user-solid.svg" alt=""> 397 views
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'TheArtistsSection'
}
</script>

<style lang="scss">
    .artists_section{
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
            .artist-card{
                width: calc(100% / 3);
                height: 100%;
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
                    .card_title{
                        text-transform: uppercase;
                        font-weight: 700;
                        font-size: 14px;
                        color: grey;
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
                        .lessons{
                            img{
                                width: 10px;
                                margin-right: 5px;
                            }
                        }
                    }
                    .subscribes{
                        img{
                            width: 10px;
                            height: 10px;
                                margin-right: 5px;
                        }
                    }
                }
            }
            .artist-card:hover{
                h6{
                    color: #1fad95;
                }
            }
        }
        .water{
            color: #1fad95;
            font-weight: 500;
        }
    }
</style>