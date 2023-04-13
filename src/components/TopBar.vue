<template>
   <div class="box">
    <button>Information</button>
    <button>About us</button>
    <button>Subscription</button>
    </div>
</template>

<script>
export default {
    name: "TopBar"

}
</script>

<style scoped>

.box{
    background-color: white;
    display: flex;
    justify-content: space-evenly;
    font-weight: bold;
    padding: 20px;
}
button{
    color: black;
    border: none;
    background:none;
    width: 140px;
    height: auto;
    float: left;
    transition: .5s linear;
    position: relative;
    display: block;
    overflow: hidden;
    padding: 15px;
    text-align: center;
    margin-bottom: 500%;
    background: transparent;
    font-weight: 700;
    cursor:pointer;
}

button:before{
    position: absolute;
    content: '';
    left: 0;
    bottom: 0;
    height: 4px;
    width: 100%;
    border-bottom: 4px solid transparent;
    border-left: 4px solid transparent;
    box-sizing: border-box;
    transform: translateX(100%);
}

button:after {
    position: absolute;
    content: '';
    top: 0;
    left: 0;
    width: 100%;
    height: 4px;
    border-top: 4px solid transparent;
    border-right: 4px solid transparent;
    box-sizing: border-box;
    transform: translateX(-100%);
}
button:hover {
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
}

button:hover:before {
    border-color: #262626;
    height: 100%;
    transform: translateX(0);
    transition: .3s transform linear, .3s height linear .3s;
}

button:hover:after {
    border-color: #262626;
    height: 100%;
    transform: translateX(0);
    transition: .3s transform linear, .3s height linear .5s;
}
</style>