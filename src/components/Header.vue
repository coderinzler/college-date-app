<template>
    <div class="header">
        <div class="menu-icon">
            <img src="/basic-gear-setting-svgrepo-com.svg" alt="Menu Icon">
        </div>
        <h1 class="logo">UPDate</h1>
        <button class="button">Log-in</button>
    </div>
</template>

<script>
export default {
    name: 'Header',
}
</script>

<style scoped>
.header {
    background: white;
    grid-column: span 3;
    color: red;
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
    color: red;
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
.button {
  border: none;
  padding: 16px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  transition-duration: 0.4s;
  cursor: pointer;
  background-color: white; 
  color: #f44336; 
  border: 2px solid #f44336;
}
.button:hover {
  background-color: #f44336;
  color: white;
}
</style>
