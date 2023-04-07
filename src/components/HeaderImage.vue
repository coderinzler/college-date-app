<template>
  <div class="headerImage">
    <img src="../assets/img/HERO.jpg" alt="HandsTogether" />
    <div class="containerTextHands">
      <h1>Find new people.
        Whenever. Wherever.</h1>
      <h3>Search for college students with your same tastes and begin to expand your social life</h3>
      <button class="button button2">Register ></button>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderImage",
};
</script>

<style scoped>
.headerImage {
  background: white;
  grid-column: span 3;
  color: red;
  text-align: center;
  height: 450px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-bottom: lightgrey 1px solid;
}
.headerImage > img{
  max-width: 100%;
  min-width: 1000px;
  opacity: 0.25;
}
.containerTextHands{
  position:absolute;
  margin-left: 10%;
  text-align: initial;
  color: black;

}
.containerTextHands > h1{
  max-width: 500px;
  font-weight: 500;
  font-size: 3em;
}
.containerTextHands > h3{
  max-width: 600px;
  font-size: 1.7em;
  padding-bottom: 10px;
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
  border-radius: 50px;
  font-weight: bold;
  border: 2px solid #f44336;
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
