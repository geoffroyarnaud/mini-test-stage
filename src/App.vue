<template>
  <div>
    <div id="wrap">
      <div class="navbar">
          <li>
              <a href="#">Notre concept</a>
          </li>
          <li>
              <a href="#">Nos services</a>
          </li>
          <li>
              <a href="#">Pourquoi nous rejoindre?</a>
          </li>
        <button class="button" type="button">Se connecter</button>
    </div>
    
    <div class="logo">
      logo
    </div>
    <div class="classer">
        <h1>
          La plateforme professionnelles<br>
          et participative<br>
          des jeunes talents
        </h1>
        <h3>
          Talent acquisition | Crowsourcing | Social network
        </h3>
        <div>
          <button on-click="formulaireinscription" class="button1" type="button">Je suis une entreprise</button>
          <button class="button2" type="button">Je suis un jeune talent</button>
        </div>
    </div>
    <FormConnexion>
    </FormConnexion>
  </div>
  </div>
</template>

<script>
 import FormConnexion from './components/FormConnexion.vue'

export default {
  name: 'App',
  components: {
    FormConnexion
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

   color: #2c3e50;  
  margin:0;
  padding: 0;
  width: 100%;
  height: 100vh;
  background-image: url('./assets/img/img1.jpeg');
  background-size: cover;
  
}

.navbar{
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow:hidden; 
  margin-left: 34rem;
}

li{
 float: left;
}

li a{
  display: block;
  color: white;
  padding: 10px 10px;
  margin-left: 1.5rem;
  text-decoration: none;
font-size: 15px;
font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
}

.navbar a{
  margin-top: 3rem;
}

.button{
  display: inline-block;
  width: 9rem;
  border-radius: 5px;
  border: 2px solid #fff;
  font-size: 15px;
  padding: 12px;
  color: white;
  cursor: pointer;
  background: none;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  margin-top:2.8rem;
  margin-left: 80px;
}

.button1{
  display: inline-block;
  border-radius: 8px;
  border: 2px solid #fff;
  font-size: 17px;
  padding: 9px;
  color: white;
  cursor: pointer;
  background: rgb(61, 110, 116);
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  margin-top:2rem;
  margin-right: 9px;
  width: 15rem;
  left: 0;
}
.button2{
  display: inline-block;
  border-radius: 8px;
  border: 2px solid rgb(61, 110, 116);
  font-size: 17px;
  padding: 9px;
  color: rgb(61, 110, 116);
  cursor: pointer;
  background: none;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  margin-top:2rem;
  width: 15rem;
  margin-left: 5px;
  left: 0;
}

.classer{
  margin-left: 100px;
  margin-top: 135px;
  width: 35rem;
  font-size: 19px;
  text-align: center;

}
h1{
  color: rgb(61, 110, 116);
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
}
h3{
  color: rgb(240, 210, 38);
}
.logo{
  font-size: 30px;
  margin-top: -40px;
  margin-left: 200px;
  color: rgb(61, 110, 116);
}


</style>
