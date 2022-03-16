<template>
    <div class="page-main">
        <div :class="main_left_class">
            <h1 style="font-weight: 300">Healthy Food,</h1>
            <h1>Healthy Life.</h1>
            <h5>{{ main_msg }}</h5>
        </div>
        <div :class="main_right_class">
            <img src="./../assets/vegfoodplate.png" alt="veg food">
        </div>
    </div>
    <div class="scroll">

    </div>
</template>

<script>
export default {
    data(){
        return{
            main_msg : "Order food according to nutritions values and get food recommendations based on your health conditions",
            main_left_class : "main-left",
            main_right_class : "main-right"
        }
    }
}
</script>

<style scoped>
    .page-main{
        margin-top: 40px;
        display: flex;
    }

    .main-left{
        max-width: 50%;
        display: flex;
        align-items: center;
        flex-direction: column;
        justify-content: center;
    }

    .main-left h1{
        font-size: 72px;
        margin: 4px;
        text-align: left;
        color: black;
    }
    .main-left h5{
        font-size: 20px;
        margin: 4px;
        font-weight: 500;
        text-align: left;
        margin-left: 50px;
        color: rgb(95, 95, 95);
    }
    .main-right img{
        max-height: 500px;
        max-width: 500px;
        height: auto;
        width: auto;
        margin-left: 100px;
    }

    .scroll{
        height: 1px;
        width: 200px;
        background-color: #a5a5a5;
        transform: rotateZ(90deg);
        position: absolute;
        left: 0%;
    }

    .scroll::before{
        content: 'SCROLL';
        color: #a5a5a5;
        transform: rotateZ(180deg);
        position: absolute;
        right: -36%;
        font-weight: 600;
    }

</style>