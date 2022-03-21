<template>
    <div class="navbar_container">
        <div class="navbar_item">
            <ul class="pages_list">
                <li>Home </li>
                <li>Pages </li>
                <li>Courses </li>
                <li>Features </li>
                <li>Blog </li>
                <li>Shop </li>
            </ul>
        </div>
        <div class="navbar_item">
            <img src="../assets/dark-logo.png" alt="">
        </div>
        <div class="navbar_item">
            <ul class="buttons_list">
                <li class="cart">
                    cart
                </li>
                <li class="user">
                    user
                </li>
                <li class="input">
                    <form class="searchbar" action="search">
                        <input type="text" placeholder="Search...">
                        <button>lens</button>
                    </form>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'TheHeader',
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
                li{
                    height: 80%;
                    display: flex;
                    align-items: center;
                    justify-content: center;
                    font-size: 14px;
                }
                .cart, .user{
                    width: 25%;
                }
                .input{
                    flex-grow: 1;
                    .searchbar{
                        display: flex;
                        height: 70%;
                        border: none;
                        input, button{
                            background-color: #e2e2e0;
                            padding: 5px;
                            border: none;
                        }
                    }
                }
            }
            img{
                width: 45%;
                height: 50%;
            }
        }
    }
</style>