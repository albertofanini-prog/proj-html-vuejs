<template>
    <footer>
        <div class="info_wrapper">
            <div class="address_wrapper">
                <div class="one">
                    <h6>
                        Address
                    </h6>
                    <ul>
                        <li
                        v-for="(addressItem, i) in addressItems"
                        :key="i"
                        >
                            {{addressItem.content}}
                        </li>
                        <li>
                            <img src="../assets/Icons/facebook-brands.svg" alt="">
                            <img src="../assets/Icons/twitter-brands.svg" alt="">
                            <img src="../assets/Icons/instagram-brands.svg" alt="">
                            <img src="../assets/Icons/linkedin-brands.svg" alt="">
                        </li>
                    </ul>
                </div>
            </div>
            <div class="links_wrapper">
                <div class="first">
                    <h6>Explore</h6>
                    <ul>
                        <li
                        v-for="(exploreItem, i) in exploreItems"
                        :key="i"
                        >
                            {{exploreItem.explore}}
                        </li>
                    </ul>
                </div>
                <ul class="second">
                    <h6>Information</h6>
                    <ul>
                        <li
                        v-for="(informationItem, i) in informationItems"
                        :key="i"
                        >
                            {{informationItem.info}}
                        </li>
                    </ul>
                </ul>
            </div>
        </div>
        <div class="rights_banner">
            <div class="rights_text">
                <h4>2020 Maxcoach. All Rights Reserved</h4>
                <button><img src="../assets/Icons/up-long-solid.svg" alt=""></button>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'TheFooter',
    data(){
        return{
            addressItems:[
                {
                    content: '382 NE 191st St # 87394 Miami, FL 33179-3899'
                },
                {
                    content: '+1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)'
                },
                {
                    content: 'support@maxcoach.com'
                },
            ],
            exploreItems:[
                {
                    explore: 'Start here'
                },
                {
                    explore: 'About us'
                },
                {
                    explore: 'Courses'
                },
                {
                    explore: 'Blog'
                },
                {
                    explore: 'Success story'
                },
                {
                    explore: 'Contact us'
                },
            ],
            informationItems:[
                {
                    info: 'Membership'
                },
                {
                    info: 'Purchase guide'
                },
                {
                    info: 'Privacy policy'
                },
                {
                    info: 'Terms of service'
                },
            ]
        }
    }
}
</script>

<style lang="scss">
    footer{
        width: 100%;
        height: 400px;
        // border: 7px solid red;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        background-color: #171621;
        .info_wrapper{
            width: 70%;
            height: 100%;
            // border: 5px solid yellow;
            display: flex;
            align-items: center;
            color: #8b8b90;
            .address_wrapper{
                width: 50%;
                height: 100%;
                // border: 3px solid green;
                display: flex;
                align-items: center;
                text-align: left;
                .one{
                    width: 100%;
                    height: 60%;
                    display: flex;
                    flex-direction: column;
                    align-items: center;
                    padding: 5px 10px;
                    h6{
                        color: white;
                        font-size: 22px;
                        width: 100%;
                        height: 20%;
                        margin-bottom: 25px;
                    }
                    p{
                        font-size: 16px;
                        width: 100%;
                        height: 20%;
                    }
                    ul{
                        width: 100%;
                        height: 80%;
                        list-style: none;
                        display: flex;
                        flex-direction: column;
                        li{
                            width: 100%;
                            font-size: 16px;
                            height: 25%;
                            img{
                                width: 35px;
                                height: 35px;
                                padding: 0px 5px;
                                filter: invert(54%) sepia(0%) saturate(1581%) hue-rotate(352deg) brightness(102%) contrast(93%);
                                cursor: pointer;
                            }
                        }
                    }
                }
            }
            .links_wrapper{
                width: 50%;
                height: 100%;
                // border: 3px solid green;
                display: flex;
                align-items: center;
                padding: 0px 20px;
                .first{
                    // border: 1px solid red;
                    width: 60%;
                    height: 60%;
                    list-style: none;
                    display: flex;
                    flex-direction: column;
                    align-items: center;
                    padding: 5px 10px;
                    h6{
                        width: 100%;
                        height: 20%;
                        color: white;
                        font-size: 22px;
                        margin-bottom: 15px;
                    }
                    ul{
                        width: 100%;
                        height: 80%;
                        list-style: none;
                        display: flex;
                        align-items: center;
                        flex-wrap: wrap;
                        li{
                            width: 50%;
                            font-size: 16px;
                        }
                    }
                }
                .second{
                    // border: 1px solid red;
                    width: 40%;
                    height: 60%;
                    list-style: none;
                    display: flex;
                    flex-direction: column;
                    align-items: center;
                    padding: 5px 10px;
                    h6{ 
                        width: 100%;
                        height: 20%;
                        color: white;
                        font-size: 22px;
                        margin-bottom: 15px;
                    }
                    ul{
                        width: 100%;
                        height: 80%;
                        list-style: none;
                        display: flex;
                        flex-direction: column;
                        li{
                            width: 100%;
                            font-size: 16px;
                            height: 25%;
                        }
                    }
                }
            }
        }
        .rights_banner{
            width: 70%;
            height: 25%;
            // border: 5px solid yellow;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
            .rights_text{
                display: flex;
                align-items: center;
                justify-content: center;
                color: #8b8b90;
                button{
                    position: absolute;
                    top: 0;
                    right: 0;
                    transform: translate(500%, 0%);
                    height: 50px;
                    width: 50px;
                    border-radius: 999px;
                    border: none;
                    background-color: #1fad95;
                    display: flex;
                    align-items: center;
                    cursor: pointer;
                    img{
                        width: 80%;
                        height: 60%;
                        filter: invert(100%) sepia(100%) saturate(2%) hue-rotate(22deg) brightness(107%) contrast(101%);
                    }
                }
            }
        }
    }
</style>