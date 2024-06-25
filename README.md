<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>login form</title>
    <link rel="stylesheet" href="style.css">
    <script src="https://unpkg.com/boxicons@2.1.4/dist/boxicons.js"></script>
</head>

<body>
    <div class="wrapper">
        <form action="">
            <h1>Login</h1>
            <div class="input-box">
                <input type="text" placeholder="username" required>
                <box-icon type='solid' name='user-pin'></box-icon>
            </div>
            <div class="input-box">
                <input type="password" placeholder="password" required>
                <box-icon type='solid' name='lock-alt'></box-icon>
            </div>
            <div class="remember-forgot">
                <label for=""><input type="checkbox">remember me</label>
                <a href="#">Forgot password</a>
            </div>
            <button type="submit" class="btn">login</button>
            <div class="registration-link">
               <p>Dont have an account? <a href="#">Register</a></p>
            </div>

        </form>
    </div>
</body>
</html>

//css for login form


@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: "poppins",sans-serif;
}
body{
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    color: white;
    background:url(https://wallpapercave.com/wp/wp400110.jpg);
    background-size:cover;
    background-position: center;
}
.wrapper{
    width: 400px;
    height: 45vh;
    border-radius: 10px;
    background:transparent;
    border: 2px solid rgba(255, 255, 255,.2);
    backdrop-filter: blur(10px);
    padding-left: 20px;
    padding-right: 20px;
}

h1{
    padding: 5px;
    font-weight: 500;
    text-align: center;
}
.input-box{ 
   width: auto;
   height: 30px;
   margin: 20px 0;
   border-radius: 18px;
}

.wrapper .remember-forgot{
    padding: 10px;
    display: flex;
    justify-content: space-between;
    font-size: 15px;
    margin: -19px 0px 15px ;
}
.remember-forgot label input{
 accent-color: white;
 margin-right: 5px;
}

.wrapper .input-box input{
    width: 100%;
    height: 100%;
    background-color:transparent;
    border: none;
    outline: none;
    border: 2px solid rgb(255, 255, 255,.2);
    border-radius: 10px;
    padding: 15px;
    color: white;
}

.input-box input::placeholder{
    color: white;
}

.input-box box-icon{
    position: absolute;
    right: 20px;
    transform: translateY(13%) translateX(-50%);
    padding: 2px 2px;
    font-size: 20px;
}

.remember-forgot a{
    color: white;
    text-decoration: none;
}

.remember-forgot a:hover{
    text-decoration: underline;
}

.wrapper .btn{
    width: 100%;
    height: 50%;
    border-radius:15px;
    border: none;
    padding: 3px;
    font-weight: 600;
    font-size: 15px;
}

.wrapper .registration-link {
  text-align: center;
  margin: 12px;
  font-size: 15px;
}

.registration-link p a{
 color: white;
 text-decoration: none;
 font-weight: 600;

}
.registration-link p a:hover{
 text-decoration: underline;
}
