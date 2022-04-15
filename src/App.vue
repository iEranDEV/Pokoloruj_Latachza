<script setup>

    function changeBackground() {
        document.querySelector("#color_box").style.backgroundColor = document.querySelector("#kolor").value;
    }

</script>

<template>
    <div id="box">
        <div>
            <div id="color_box"></div>
            <img src="../public/latachz.jpg" alt="LatachZ">
        </div>
        <input type="color" id="kolor" name="kolor">
        <button @click="changeBackground()">Zmień kolor</button>
    </div>
</template>

<style scoped>
@import './assets/base.css';

    #box {
        width: 100%;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
    }

    #color_box {
        width: 300px;
        height: 300px;
        border-radius: 10%;
        position: absolute;
        opacity: 55%;
    }

    img {
        margin-bottom: 5%;
        width: 300px;
        box-shadow: 2px 2px 10px black;
        border-radius: 10%;
    }

    input {
        width: 150px;
        height: 50px;
        border: none;
        background-color: #545454;
    }
    input:hover {
        cursor: pointer;
        box-shadow: 2px 2px 10px black;
    }

    button {
        margin-top: 2%;
        width: 200px;
        height: 50px;
        background-color: #545454;
        border: none;
        color: white;
        font-size: 1.5rem;
        border-radius: 5%;
        box-shadow: 2px 2px 10px black;
    }

    button:hover {
        box-shadow: 2px 2px 20px black;
        background-color: #2b2b2b;
        cursor: pointer;
    }



</style>
