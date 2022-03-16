<template>
    <div class="page-header">
        <div :class="head_left_class">
            <div class="head-logo">
                <img src="./../assets/foodbowl.png" alt="foodbowllogo">
            </div>
            <h1><a href="">Diet-Bowl</a></h1>
        </div>
        <div :class="head_right_class">
            <h2><a href="">Feat<span style="color:white">ures</span></a></h2>
            <h2><a style="color:white" href="">Download</a></h2>
            <h2><a style="color:white" href="">About Us</a></h2>
        </div>
    </div>
</template>

<script setup>
    import { ref } from 'vue';

    const head_left_class = ref('head-left');
    const head_right_class = ref('head-right');
</script>

<style scoped>

.page-header{
    display: flex;
}

.head-logo{
    width: 80px;
    height: 80px;
    padding: 5px;
    border-radius: 18px;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #E8F4FA;
    box-shadow: 4px 4px 8px 0px rgba(0,0,0,0.1),-4px -4px 8px 0px rgba(0,0,0,0.1);
    -webkit-box-shadow: 4px 4px 8px 0px rgba(0,0,0,0.1),-4px -4px 8px 0px rgba(0,0,0,0.1);
    -moz-box-shadow: 4px 4px 8px 0px rgba(0,0,0,0.1),-4px -4px 8px 0px rgba(0,0,0,0.1);
}

.head-left{
    display: flex;
    gap: 20px;
    margin-right: auto;
    justify-content: center;
    align-items: center;
}

.head-right{
    display: flex;
    gap: 100px;
    justify-content: center;
    align-items: center;
}

h1{
    font-family: 'Lato';
    font-weight: 700;
}

img{
    max-height: 100px;
    max-width: 100px;
    height: auto;
    width: auto;
}

a{
    color: black;
    text-decoration: none;
}

.head-left a{
    color: #0d8b1e;
}
</style>