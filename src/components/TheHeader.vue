<template>
    <div class="navbar_container">
        <div class="navbar_item">
            <ul class="pages_list">
                <li
                v-for="(navbarItem, i) in navbarItems"
                :key="i"
                >
                    {{navbarItem.name}}
                    <img src="../assets/Icons/angle-down-solid.svg" alt="">
                </li>
            </ul>
        </div>
        <div class="navbar_item">
            <img src="../assets/dark-logo.png" alt="">
        </div>
        <div class="navbar_item">
            <ul class="buttons_list">
                <li class="cart">
                    <img src="../assets/Icons/cart-shopping-solid.svg" alt="">
                </li>
                <li class="user">
                    <img src="../assets/Icons/circle-user-solid.svg" alt="">
                </li>
                <li class="input">
                    <form class="searchbar" action="search">
                        <input type="text" placeholder="Search...">
                        <button><img class="len_img" src="../assets/Icons/magnifying-glass-solid.svg" alt=""></button>
                    </form>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'TheHeader',
    data(){
        return{
            navbarItems:[
                {
                    name: 'Home'
                },
                {
                    name: 'Pages'
                },
                {
                    name: 'Courses'
                },
                {
                    name: 'Features'
                },
                {
                    name: 'Blog'
                },
                {
                    name: 'Shop'
                }
            ]
        }
    }
}
</script>

<style lang="scss">
    .navbar_container{
        // border: 5px solid red;
        width: 100%;
        height: 75px;
        display: flex;
        justify-content: space-between;
        gap: 10px;
        padding: 0px 5%;
        .navbar_item{
            // border: 3px solid yellow;
            width: calc((100% / 3) - 10px);
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            .pages_list{
                width: 100%;
                height: 100%;
                // border: 2px solid green;
                list-style: none;
                display: flex;
                align-items: center;
                // justify-content: center;
                gap: 5px;
                li{
                    // border: 1px solid purple;
                    width: calc((100% / 6) - 5px);
                    text-align: center;
                    font-size: 14px;
                    height: 80%;
                    display: flex;
                    align-items: center;
                    justify-content: center;
                    cursor: pointer;
                    img{
                        width: 12px;
                    }
                }
            }
            .buttons_list{
                padding: 0px 10px;
                width: 100%;
                height: 100%;
                // border: 2px solid red;
                list-style: none;
                display: flex;
                align-items: center;
                gap: 5px;
                justify-content: center;
                li{
                    height: 80%;
                    display: flex;
                    align-items: center;
                    font-size: 14px;
                    cursor: pointer;
                }
                .cart, .user{
                    cursor: pointer;
                    img{
                        width: 20px;
                    }
                }
                .input{
                    .searchbar{
                        display: flex;
                        height: 70%;
                        border: none;
                        input, button{
                            background-color: #e2e2e0;
                            padding: 5px;
                            border: none;
                        }
                        input{
                            border-radius: 5px 0px 0px 5px;
                            padding: 0px 10px;
                        }
                        button{
                            border-radius: 0px 5px 5px 0px;
                        }
                        .len_img{
                            width: 70%;
                            height: 70%;
                        }
                    }
                }
            }
            img{
                width: 45%;
                height: 50%;
            }
        }
        .navbar_item:nth-child(1){
            flex-grow: 1;
        }
    }
</style>