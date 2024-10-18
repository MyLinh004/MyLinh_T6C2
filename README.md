Môn học:CNPMNC 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login & Registration</title>
    <link rel="stylesheet" href="../Css/SignUp.css">
</head>
<body>
    <div class="container">
        <div class="form-box">
            <!-- Tabs for Switching between Login and Register -->
            <div class="button-box">
                <button id="loginBtn" class="toggle-btn active" onclick="showLogin()">Đăng nhập</button>
                <button id="registerBtn" class="toggle-btn" onclick="showRegister()">Đăng ký</button>
            </div>
            
            <!-- Login Form -->
            <form id="loginForm" class="input-group">
                <table>
                <div><label for="login-username">Email đăng nhập:</label></div>
                <div><input type="text" id="login-email" placeholder="Email đăng nhập" required></div>
                
                <div><label for="login-password">Nhập mật khẩu:</label></div>
                <div><input type="password" id="login-password" placeholder="Nhập mật khẩu" required></div>
                <!-- Nút quên mật khẩu -->
                <div>
                      <a href="ForgetPassword.html" class="forgot-password-btn">Quên mật khẩu?</a>
                </div>
                
                <div><button type="submit" class="submit-btn">Đăng nhập</button></div>
            </table>
            </form>

            <!-- Registration Form -->
            <form id="registerForm" class="input-group" style="display:none;">
                
                <label for="register-email">Nhập email:</label>
                <input type="email" id="register-email" placeholder="Nhập email" required>
                
                <label for="register-password">Nhập mật khẩu:</label>
                <input type="password" id="register-password" placeholder="Nhập mật khẩu" required>
                
                <label for="register-password-confirm">Nhập lại mật khẩu:</label>
                <input type="password" id="register-password-confirm" placeholder="Nhập lại mật khẩu" required>
                
                <button type="submit"  class="submit-btn">Đăng ký</button>
            </form>
        </div>
        
        <!-- Welcome Text -->
        <div class="welcome-text" id="welcomeMessage">
            Chào mừng bạn đã đến với web đọc truyện của chúng tôi!
        </div>
    </div>

    <script src="../Js/SignUp.js"></script>
    <script type = "module" src="../Js/firebase_auth.js"></script>
</body>
</html>
