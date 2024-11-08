<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>All products - RedStore</title>
    <link rel="stylesheet" href="style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.6.0/css/fontawesome.min.css">
</head>
<body>
    <div class="container">
        <div class="navbar">
            <div class="logo">
                <img src="redstore.png" width="125px">
            </div>
            <nav>
                <ul id="MenuItems">
                    <li><a href="index.html">Home</a></li>
                    <li><a href="product.html">Products</a></li>
                    <li><a href="">About</a></li>
                    <li><a href="">Contact</a></li>
                    <li><a href="account.html">Account</a></li>
                </ul>
            </nav>
            <img src="cart.jpg" width="30px" height="30px">
            <img src="menu.jpeg" width="30px" height="30px" onclick="menutoggle()">
        </div>
    </div>

<!------------ account page------------>

<div class="account-page">
     <div class="container">
          <div class="row">
               <div class="col-2">
                    <img src="Foot.png" width="100%">
               </div>

               <div class="col-2">
                    <div class="form-container">
                         <div class="form-btn">
                              <span onclick="register()">Login</span>
                         </div>

                         <form id="LoginForm">
                              <input type="text" placeholder="Username">
                              <input type="password" placeholder="Password">
                              <button type="submit" class="btn">Login</button>
                              <a href="">Forgot password</a>
                         </form>
                    </div>
               </div>
          </div>
     </div>
</div>

<!---------- footer-------->

    <div class="footer">
        <div class="container">
            <div class="row">
                <div class="footer-col-1">
                    <h3>Download Our App</h3>
                    <p>Download App for Android and ios mobile phone.</p>
                    <div class="app-logo">
                        <img src="app1.png">
                        <img src="app2.png">
                    </div>
                </div>
                <div class="footer-col-2">
                    <img src="redstore.png">
                    <p>welcome to our e-commerce platform first you login than immerse in our website</p>
                </div>
                <div class="footer-col-4">
                    <h3>Follow us</h3>
                    <ul>
                        <li>Facebook</li>
                        <li>Twitter</li>
                        <li>Instagram</li>
                        <li>You Tube</li>
                    </ul>
                </div>
            </div>
            <hr>
            <p class="copyright"></p>Copyright 2020 - Easy Tutorials</p>
        </div>
    </div>
<!---------- js for toggle menu----------->

<script>
    var MenuItem = document.getElementById("MenuItem");

    MenuItem.style.maxHeight = "0px";

    function menutoggle(){
        if(MenuItem.style.maxHeight == "0px")
            {
                MenuItem.style.maxHeight = "200px";
            }
        else
            {
                MenuItem.style.maxHeight = "0px";
            }

    }
</script>

<!---------- js for toggle form----------->

    <script>

     var LoginForm = document.getElementById("LoginForm");

     function login() {
    RegForm.style.transform = "translateX(300px)";
    LoginForm.style.transform = "translateX(0px)";
    Indicator.style.transform = "translateX(0px)";
}
 
    </script>

</body>
</html>
