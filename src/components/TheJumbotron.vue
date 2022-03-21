<template>
    <div class="jumbotron">
        <div class="jumbotron_content">
            <h5>Commence Business</h5>
            <p>Distant Mentoring Program</p>
            <button>Download free guidebook</button>
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
        display: flex;
        align-items: center;
        justify-content: center;
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
            }
        }
    }
</style>