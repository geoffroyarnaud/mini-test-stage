<template>
        <div class="modal-bg">
            <div class="modal">
                <h3>logo</h3>
                <div>

                    <div class="talent">Talent</div>

                    <div class="grid-container">
                        <div class="box">
                            <div class="item">
                                <div class="toggle-pill">
                                    <input type="checkbox" id="pill1" name="check">
                                    <label for="pill1"></label>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="client">Client</div>
                    <button class="button2" type="button">Email</button>
                    <button class="button3" type="button">Mot de passe</button>

                    <div class="box">
                        <div class="item">
                            <div class="checkbox-rect">
                                <input type="checkbox" id="checkbox-rect1" name="check">
                                <label class="labels" for="checkbox-rect1">Se souvenir de moi</label>
                            </div>
                        </div>
                    </div>
                    <div> 
                        <div class="navbar">
                            <li>
                                <a href="#">Mot de passe oublié ?</a>
                            </li>
                        </div>
                    </div>

                    <button class="button4" type="button">Se connecter</button>

                </div>
            </div>
        </div>
</template>

<style scoped>

        .modal-bg{
            background: rgb(61, 110, 116);
            width: 19rem;
            border-radius: 9px;
            height: 28rem;
            margin-top: -26rem;
            margin-left: 63rem;
            opacity: 0.8;
            backdrop-filter: blur(12px);
            backdrop-filter: blur(12px);
            backdrop-filter: drop-shadow(4px 4px 10px black);
            box-shadow: 3px 3px 3px rgba(0, 0.5, 0.5, 0.2 ); 
        }
       .modal h3{
            color: white;
            font-size: 24px;
            text-align: center;
            padding-top: 19px;  
        }

        .grid-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, 300px);
  /* minmax(300px, 1fr)*/
  grid-gap: 30px;
  padding: 24px;
  justify-items: center;
  justify-content: center;
  align-items: start;
  margin-top: -85px;
}
.box {
  padding: 2em;
}
.item {
  margin-bottom: 2em;
}
.labels{
    font-size: 15rem;
    color: #fff;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;


}

/* checkbox-rect */
.checkbox-rect input[type="checkbox"] {
  display: none;
}
.checkbox-rect input[type="checkbox"] + label {
  display: block;
  position: relative;
  padding-left: 35px;
  margin-bottom: 20px;
  font: 14px/20px "Open Sans", Arial, sans-serif;
  cursor: pointer;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  margin-left: 3rem;
  margin-top: -1rem;
}

.checkbox-rect input[type="checkbox"] + label:before {
  content: "";
  display: block;
  width: 1.1em;
  height: 1.1em;
  border: 2px solid white;
  border-radius: 0.2em;
  position: absolute;
  left: 0;
  top: 0;
  -webkit-transition: all 0.2s, background 0.2s ease-in-out;
  transition: all 0.2s, background 0.2s ease-in-out;
  background: none;
}
.checkbox-rect input[type="checkbox"]:checked + label:before {
  width: 1.3em;
  height: 1.3em;
  border-radius: 0.2em;
  border: 1px solid blue;
  -webkit-transform: rotate(90deg);
  transform: rotate(90deg);
  background: blue;
  box-shadow: 0 0 0 1px #000;
}
/* checkbox-rect end */

/* lien mot de passe oublié */

.navbar{
  list-style-type: none;
  margin: 0;
  padding: 0;
  margin-top: -55px;
  width: 100%;
  height: 30px;
  overflow:hidden; 
  
}

li a{
  display: block;
  color: white;
  margin-top: -13px;
  margin-left: 4rem;
  text-decoration: none;
font-size: 16px;

}
/*fin lien mot de passe oublié */


.button2{
 display: inline-block;
  border-radius: 8px;
  border: 2px solid white;
  font-size: 17px;
  padding: 9px;
  color: white;
  cursor: pointer;
  background: none;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  margin-top:3rem;
  margin-left: 15px;
  width: 15rem;
  margin-left: 25px;
  left: 0;
}
.button4{
    display: inline-block;
  border-radius: 8px;
  border: 2px solid white;
  font-size: 17px;
  padding: 9px;
  color: rgb(61, 110, 116);
  cursor: pointer;
  background-color: white;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  margin-top:1rem;
  margin-left: 15px;
  width: 15rem;
  margin-left: 25px;
  left: 0;
}
.button3{
 display: inline-block;
  border-radius: 8px;
  border: 2px solid white;
  font-size: 17px;
  padding: 9px;
  color: white;
  cursor: pointer;
  background: none;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  margin-top:1rem;
  margin-left: 15px;
  width: 15rem;
  margin-left: 25px;
  left: 0;
}

        /* toggle-pill */
.toggle-pill input[type="checkbox"] {
  display: none;
}
.toggle-pill input[type="checkbox"] + label {
  display: block;
  position: relative;
  width: 6em;
  height: 1.9em;
  margin-bottom: 20px;
  border-radius: 1em;
  background: none;
  border: 2px solid white;
  box-shadow: inset 0px 0px 3px 1px rgba(0, 0, 0, 0.3);
  cursor: pointer;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  -webkit-transition: background 0.1s ease-in-out;
  transition: background 0.1s ease-in-out;
}
.toggle-pill input[type="checkbox"] + label:before {
  content: "";
  display: block;
  width: 1.3em;
  height: 1.6em;
  border-radius: 1em;
  background: #fff;
  box-shadow: 2px 0px 5px rgba(0, 0, 0, 0.2);
  position: absolute;
  left: 0.2em;
  top: 0.2em;
  -webkit-transition: all 0.2s ease-in-out;
  transition: all 0.2s ease-in-out;
}

.toggle-pill input[type="checkbox"]:checked + label:before {
  box-shadow: -2px 0px 5px rgba(0, 0, 0, 0.2);
  left: 4.6em;
}
/* toggle-pill end */
        
.talent{
    color: #fff;
    margin-top: 70px;
    font-size: 20px;
    margin-left: 25px;
}
.client{
    color: #fff;
    margin-top: -114px;
    font-size: 20px;
    margin-left: 14rem;
}


</style>