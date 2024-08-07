<!DOCTYPE html>  
<html lang="zh-CN">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>XXXX登录界面</title>  
    <style>  
        * {  
            margin: 0;  
            padding: 0;  
        }  
        body {  
            min-height: 100vh;  
            background: linear-gradient(#141e30, #243b55);  
            background-image: url('background.jpg'); 
            background-size: cover;  
            background-position: center;  
            background-repeat: no-repeat;  
        }  
        .login-box {  
            width: 400px;  
            position: absolute;  
            left: 50%;  
            top: 50%;  
            transform: translate(-50%, -50%);  
            padding: 40px;  
            background: rgba(0, 0, 0, 0.5);  
            box-sizing: border-box;  
            box-shadow: 0 15px 25px rgba(0, 0, 0, 0.6);  
            border-radius: 10px;  
            text-align: center;
        }  
        .login-box h2 {  
            margin: 0 0 40px;  
            padding: 0;  
            color: #fff;  
        }  
        .login-box .user-box {  
            position: relative;  
        }  
        .login-box .user-box input {  
            width: 100%;  
            padding: 10px 0;  
            font-size: 16px;  
            color: #fff;  
            margin-bottom: 30px;  
            border: none;  
            border-bottom: 1px solid #fff;  
            background: transparent;  
            outline: none;  
        }  
        .login-box .user-box label {  
            position: absolute;  
            top: 0;  
            left: 0;  
            padding: 10px 0;  
            color: #fff;  
            font-size: 16px;  
            pointer-events: none;  
            transition: 0.5s;  
        }  
        .login-box .user-box input:focus ~ label,  
        .login-box .user-box input:valid ~ label {  
            top: -20px;  
            left: 0;  
            color: #03e9f4;  
            font-size: 12px;  
        }  
        .login-box form a {  
            position: relative;  
            display: inline-block;  
            padding: 10px 40px;  
            color: #03e9f4;  
            text-decoration: none;  
            font-size: 16px;  
            margin-top: 30px;
            letter-spacing: 4px;  
            text-indent: 4px;  
            transition: 0.5s;  
            overflow: hidden;  
        }  
        .login-box form a:hover {  
            background: #03e9f4;  
            color: #fff;  
            border-radius: 5px;  
            box-shadow: 0 0 5px #03e9f4, 0 0 25px #03e9f4, 0 0 50px #03e9f4, 0 0 100px #03e9f4;  
        }  
        .login-box form a span {  
            position: absolute;  
            display: block;  
        }  
        .login-box form a span:nth-child(1) {  
            top: 0;  
            left: -100%;  
            width: 100%;  
            height: 2px;  
            background: linear-gradient(90deg, transparent, #03e9f4);  
            animation: btn-anim1 1s linear infinite;  
        }  
        @keyframes btn-anim1 {  
            0% { left: -100%; }  
            50%, 100% { left: 100%; }  
        }  
        .login-box form a span:nth-child(2) {  
            top: -100%;  
            right: 0;  
            width: 2px;  
            height: 100%;  
            background: linear-gradient(180deg, transparent, #03e9f4);  
            animation: btn-anim2 1s linear infinite;  
            animation-delay: 0.25s;  
        }  
        @keyframes btn-anim2 {  
            0% { top: -100%; }  
            50%, 100% { top: 100%; }  
        }  
        .login-box form a span:nth-child(3) {  
            bottom: 0;  
            right: -100%;  
            width: 100%;  
            height: 2px;  
            background: linear-gradient(270deg, transparent, #03e9f4);  
            animation: btn-anim3 1s linear infinite;  
            animation-delay: 0.5s;  
        }  
        @keyframes btn-anim3 {  
            0% { bottom: -100%; }  
            50%, 100% { bottom: 100%; }  
        }  
        .login-box form a span:nth-child(4) {  
            bottom: -100%;  
            left: 0;  
            width: 2px;  
            height: 100%;  
            background: linear-gradient(360deg, transparent, #03e9f4);  
            animation: btn-anim4 1s linear infinite;  
            animation-delay: 0.75s;  
        }  
        @keyframes btn-anim4 {  
            0% { bottom: -100%; }  
            50%, 100% { bottom: 100%; }  
        }  
        .forgot-password {  
        position: absolute;  
        bottom: 20px; 
        right: 20px;   
        color: white;
        font-size: 12px;
        text-decoration: none;  
    }  
    .forgot-password:hover {  
        text-decoration: underline;
    }  
</style>  
</head>  
<body>  
    <div class="login-box">  
        <h2>Hi！欢迎进入XXXX平台</h2>  
        <form>  
            <div class="user-box">  
                <input type="text" required>  
                <label>用户名</label>  
            </div>  
            <div class="user-box">  
                <input type="password" required>  
                <label>密码</label>  
            </div>  
            <a href="#">  
                <span></span><span></span><span></span><span></span>  
                登录  
            </a>  
        </form>  
        <a href="#" class="forgot-password">忘记密码？</a>  
    </div>  
</body>  
</html>
