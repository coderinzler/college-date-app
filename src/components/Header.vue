<template>
    <div class="header">
        <div class="menu-icon">
            <img src="/basic-gear-setting-svgrepo-com.svg" alt="Menu Icon">
        </div>
        <h1 class="logo">{{ appName }}</h1>
        <div class="profile-pic">
            <img src="/ProfilePic.png" alt="Profile Picture">
        </div>
    </div>
</template>

<script>
export default {
    name: 'Header',
    props: {
        appName: {
            type: String,
            required: true
        }
    },
}
</script>

<style scoped>
.header {
    background: #1abc9c;
    grid-column: span 3;
    line-height: 5.5;
    text-align: center;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.menu-icon{
    margin-top: 1rem;
    margin-left: 2rem;
}

.menu-icon img{
    height: 30px;
    width: 30px;
}

.logo {
    display: inline-block;
    margin: 0;
    font-size: 1.5rem;
    color: #fff;
    text-transform: capitalize;
    max-width: 100%;
}

.profile-pic{
    margin-top: 2rem;
    margin-right: 2rem;
}

.profile-pic img{
    width: 50px;
    height: 50px;
    border-radius: 50%;
}
</style>
