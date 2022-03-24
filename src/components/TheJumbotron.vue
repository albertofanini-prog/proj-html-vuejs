<template>
    <div class="jumbotron">
        <div class="jumbotron_content">
            <h5>Commence Business</h5>
            <p>Distant Mentoring Program</p>
            <button>Download free guidebook <img src="../assets/Icons/right-long-solid.svg"></button>
        </div>
            <div class="right_banner">
                <button>
                    <img src="../assets/Icons/stairs-solid.svg">
                </button>
                <button>
                    <img src="../assets/Icons/globe-solid.svg">
                </button>
                    
                <button>
                    <img src="../assets/Icons/book-solid.svg">
                </button>
                <button>
                    <img src="../assets/Icons/cart-shopping-solid.svg">
                </button>
            </div>
    </div>
</template>

<script>
export default {
    name: 'TheJumbotron'
}
</script>

<style lang="scss">
    .jumbotron{
        width: 100%;
        height: 700px;
        background-image: url('~@/assets/jumbotron.jpg');
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
        display: flex;
        align-items: center;
        justify-content: center;
        position: relative;
        .jumbotron_content{
            // border: 2px solid yellow;
            width: 60%;
            height: 40%;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            gap: 5px;
            color: #ffffff;
            h5{
                font-size: 26px;
            }
            p{
                font-size: 48px;
            }
            button{
                width: 30%;
                padding: 12px;
                border: none;
                background-color: #ffffff;
                color: #1fad95;
                font-weight: 600;
                font-size: 14px;
                border-radius: 10px;
                cursor: pointer;
                img{
                    width: 10px;
                    height: 10px;
                    filter: invert(53%) sepia(82%) saturate(418%) hue-rotate(120deg) brightness(91%) contrast(86%);
                }
            }
            button:hover{
                color: white;
                background-color: #1fad95;
                img{
                    filter: invert(100%) sepia(100%) saturate(7%) hue-rotate(144deg) brightness(104%) contrast(102%);
                }
            }
        }
        .right_banner{
            display: flex;
            flex-direction: column;
            background-color: white;
            position: absolute;
            top: 40%;
            right: 0;
            height: 150px;
            border-radius: 0px 0px 5px 5px;
            .right_banner:first-child{
                border-radius: 0px 0px 5px 5px;
            }
            button{
                width: 100%;
                height: calc(100% / 4);
                border: none;
                padding: 5px;
                cursor: pointer;
                img{
                    width: 70%;
                    height: 70%;
                }
            }
        }
    }
</style>