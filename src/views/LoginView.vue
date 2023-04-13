<template>
  <div class="login">
    <div class="login-container">
      <h1 class="login-container__welcome">Bem vindo!</h1>       
      <div  class="login-container__register">
        Ainda não possui conta? 
        <router-link style="text-decoration: underline; color: inherit; margin-left: 3px;"
        to="/register">Clique aqui para criar uma </router-link> 
      </div>
       
      <div class="login-container_div">
        <form class="login-container__form">              
          <input class="login-container__input_login" type="text" placeholder="passaporte UFMS"/> 
          <input class="login-container__input_password" type="password" placeholder="senha"/>       
          <div  class="login-container__recoverypass">
            Recuperação de senha  
            <router-link style="text-decoration: underline; color: inherit; margin-left: 3px;"
            to="/#">Passaporte UFMS </router-link> 
          </div>
          <input class="login-button" type="submit" value="entrar">
        </form>
        <img class="login-container_image" src="../assets/logo.png">
      
      </div>
      
      
      <div class="login-container__logo">        

      </div>

    </div>

  </div>
</template>


<script>

</script>


<style scoped>
.login{
  font-family: 'Roboto', sans-serif;
  display: flex;
  position: absolute;
  height: 100vh;
  width: 100vw;   
  background: linear-gradient(180deg, rgba(9,127,168,1) 0%, rgba(255,255,255,1) 100%);
  flex-direction: row;
  justify-content: center;
  align-items: center;
}

.login-container_div{
  display: flex;
}
.login-container{
  background: #ffffff;  
  width: 1220px;
  height: 600px;
  background: red;
  margin: 0;
  background: #fff;
  border-radius: 5px;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25); 
  flex-direction: row;
  align-items: center;
  text-align: center;
   
}

.login-container__welcome{
  text-transform: uppercase;
  font-family: 'Roboto';
  font-style: normal;
  font-weight: 700;
  font-size: 50px;
  line-height: 59px;
  color: #097FA8;
  margin-top: 15px;
}

.login-container__register{
  display: flex;
  margin:113px 0 0 113px;
  color: #097FA8;
  text-decoration: none;
  
}
 
.login-container__input_login{
  display: flex;
  background-repeat: no-repeat;
  background-position: left;
  background-size: 32px;
  background-image: url('../assets/mail.png'); 
  padding-left: 35px;
  font-family: 'Roboto';
  font-weight: 400;
  font-size: 20px;
  border-radius: 5px; 
  border-width:1px;
  margin-left: 112px;
  height:50px ;
  width: 527px;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  margin-top: 17px;
}

.login-container__input_password{
  display: flex;
  background-image: url('../assets/password.png');
  background-repeat: no-repeat;
  background-position: left;
  background-size: 32px;
  padding-left: 35px;
  font-family: 'Roboto';
  font-weight: 400;
  font-size: 20px;
  border-radius: 5px; 
  border-width:1px;
  margin-left: 112px;
  height:50px ;
  width: 527px;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  margin-top: 22px;
}

.login-button{   
  display: flex;
  background: #097FA8;
  border-width:1px ;
  border-radius: 5px;  
  width: 193px;
  height: 58px;
  margin-left: 113px;
  margin-top: 17px;
  font-family: 'Roboto';   
  font-size: 20px;
  color: #FFFFFF;
}

.login-container__recoverypass{   
  display: flex;
  position: absolute;
  color: #097FA8;
  margin-left: 380px;
  margin-top:35px;
  text-decoration: none;  
}

.login-container_image{
  position: absolute;
  right:450px;
  top: 300px;
}
</style>
