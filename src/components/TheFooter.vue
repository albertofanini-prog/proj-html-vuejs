<template>
    <footer>
        <div class="info_wrapper">
            <div class="address_wrapper">
                <h6>
                    Address
                </h6>
                <p>382 NE 191st St # 87394 Miami, FL 33179-3899</p>
                <p>+1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)</p>
                <p>support@maxcoach.com</p>
            </div>
            <div class="links_wrapper">
                <div class="first">
                    <h6>Explore</h6>
                    <ul>
                        <li>Start here</li>
                        <li>Blog</li>
                        <li>About us</li>
                        <li>Success story</li>
                        <li>Courses</li>
                        <li>Contact us</li>
                    </ul>
                </div>
                <ul class="second">
                    <h6>Information</h6>
                    <ul>
                        <li>Membership</li>
                        <li>Purchase guide</li>
                        <li>Privacy policy</li>
                        <li>Terms of service</li>
                    </ul>
                </ul>
            </div>
        </div>
        <div class="rights_banner">

        </div>
    </footer>
</template>

<script>
export default {
    
}
</script>

<style lang="scss">
    footer{
        width: 100%;
        height: 500px;
        border: 7px solid red;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        background-color: #171621;
        .info_wrapper{
            width: 70%;
            height: 100%;
            border: 5px solid yellow;
            display: flex;
            align-items: center;
            color: #8b8b90;
            .address_wrapper{
                width: 50%;
                height: 40%;
                border: 3px solid green;
                display: flex;
                flex-direction: column;
                align-items: flex-start;
                justify-content: center;
                text-align: left;
                h6{
                    color: white;
                    font-size: 22px;
                    width: 100%;
                    height: 40%;
                }
                p{
                    font-size: 16px;
                    width: 100%;
                    height: 20%;
                }
            }
            .links_wrapper{
                width: 50%;
                height: 100%;
                border: 3px solid green;
                display: flex;
                align-items: center;
                padding: 0px 20px;
                .first{
                    border: 1px solid red;
                    width: 60%;
                    height: 40%;
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
                    border: 1px solid red;
                    width: 40%;
                    height: 40%;
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
                        }
                    }
                }
            }
        }
        .rights_banner{
            width: 70%;
            height: 25%;
            border: 5px solid yellow;
        }
    }
</style>