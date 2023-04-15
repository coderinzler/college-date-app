<template>
  <div class="header">
    <div class="menu-icon">
      <div>
        <img src="src/assets/img/Logo UPC - color.png" alt="Logo UPC" />
      </div>
      <h1 class="logo">UpDate</h1>
    </div>
    <h2 class="language">EN</h2>
    <!--Testline-->
    <div class="profile-pic">
      <button class="button button1">Log-in</button>
      <button class="button button2">Register</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped>
.header {
  background: white;
  grid-column: span 3;
  color: #e30613;
  text-align: center;
  min-height: 100px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-bottom: lightgrey 1px solid;
}

.menu-icon {
  display: flex;
  margin: auto;
  margin-left: 2rem;
}

.menu-icon img {
  height: 48px;
  width: 48px;
}
.language{
    padding-right: 10px;
    margin-right: 30px;
}

.logo {
    color: #e30613;
    font-weight: bold;
    padding-left: 8px;
}

.button {
  border: none;
  padding: 16px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  transition-duration: 0.4s;
  cursor: pointer;
  margin: auto;
  margin-right: 2rem;
  border-radius: 5px;
  font-weight: bold;
  border: 2px solid #f44336;
}
.button1{
  color: #f44336;
  background-color: white;
}
.button1:hover {
  background-color: #f44336;
  color: white;
}
.button2{
  background-color: #f44336;
  color: white;

}
.button2:hover{
  color: #f44336;
  background-color: white;

}
</style>
