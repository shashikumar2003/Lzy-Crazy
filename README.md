<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>LzyCrazy Login Page</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet" />
    <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }

        body {
            background: linear-gradient(135deg, #e0e7ff, #fdf2f8);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 30px;
        }

        .container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            max-width: 1100px;
            width: 100%;
            background: #ffffff;
            border-radius: 20px;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.15);
            overflow: hidden;
        }

        .left-panel {
            background: linear-gradient(135deg, #f0f9ff, #dbeafe);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 50px 30px;
            position: relative;
        }

        .left-panel::before {
            content: '';
            position: absolute;
            top: 20px;
            right: 20px;
            width: 60px;
            height: 60px;
            background: linear-gradient(to top right, #6366f1, #ec4899);
            border-radius: 50%;
            opacity: 0.2;
        }

        .left-panel img {
            height: 100px;
            margin-bottom: 15px;
        }

        .left-panel h1 {
            font-size: 36px;
            font-weight: 700;
            color: #1e293b;
            margin-bottom: 5px;
        }

        .left-panel .subtext {
            font-size: 14px;
            color: #475569;
            margin: 2px 0;
        }

        .search-bar {
            margin: 25px 0;
            width: 100%;
            max-width: 350px;
            position: relative;
        }

        .search-bar input {
            width: 100%;
            padding: 12px 45px 12px 20px;
            border-radius: 30px;
            border: 1px solid #cbd5e1;
            font-size: 14px;
            outline: none;
            transition: 0.3s ease;
        }

        .search-bar input:focus {
            border-color: #6366f1;
        }

        .search-bar i {
            position: absolute;
            right: 15px;
            top: 50%;
            transform: translateY(-50%);
            color: #6366f1;
        }

        .nav-buttons {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 10px;
        }

        .nav-buttons button {
            background: #fff;
            border: 1px solid #cbd5e1;
            border-radius: 25px;
            padding: 8px 20px;
            cursor: pointer;
            font-size: 14px;
            color: #334155;
            transition: all 0.3s ease;
        }

        .nav-buttons button:hover {
            background: #dbeafe;
            color: #1e40af;
        }

        .right-panel {
            padding: 40px 50px;
            display: flex;
            justify-content: center;
            align-items: center;
            background: #ffffff;
        }

        .login-card {
            width: 100%;
            max-width: 400px;
        }

        .login-card input {
            width: 100%;
            padding: 12px 15px;
            margin-bottom: 15px;
            border-radius: 10px;
            border: 1px solid #cbd5e1;
            font-size: 14px;
            transition: 0.3s ease;
        }

        .login-card input:focus {
            border-color: #6366f1;
            box-shadow: 0 0 0 3px rgba(99, 102, 241, 0.1);
            outline: none;
        }

        .forgot-link {
            display: block;
            text-align: right;
            font-size: 13px;
            color: #3b82f6;
            margin-bottom: 20px;
            text-decoration: none;
        }

        .login-btn,
        .create-btn {
            width: 100%;
            padding: 12px;
            border: none;
            border-radius: 10px;
            background: linear-gradient(to right, #8b5cf6, #ec4899);
            color: white;
            font-weight: 600;
            font-size: 15px;
            cursor: pointer;
            transition: 0.3s ease;
        }

        .login-btn:hover,
        .create-btn:hover {
            opacity: 0.9;
        }

        .divider {
            text-align: center;
            font-size: 14px;
            color: #94a3b8;
            margin: 25px 0 15px;
            position: relative;
        }

        .divider::before,
        .divider::after {
            content: '';
            position: absolute;
            height: 1px;
            width: 40%;
            background: #cbd5e1;
            top: 50%;
        }

        .divider::before {
            left: 0;
        }

        .divider::after {
            right: 0;
        }

        .social-buttons {
            display: flex;
            gap: 10px;
            margin-bottom: 20px;
        }

        .social-buttons button {
            flex: 1;
            padding: 10px;
            border: 1px solid #e2e8f0;
            border-radius: 10px;
            background: white;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
            font-size: 14px;
            color: #475569;
            transition: all 0.3s ease;
        }

        .social-buttons button:hover {
            background-color: #f1f5f9;
        }

        @media (max-width: 900px) {
            .container {
                grid-template-columns: 1fr;
            }

            .left-panel {
                padding: 30px 20px;
            }

            .right-panel {
                padding: 30px 20px;
            }
        }
    </style>
</head>

<body>
    <div class="container">
        <div class="left-panel">
            <img src="C:\Users\shas8\Lzy crazy\New folder\lzycrazy.png" alt="LzyCrazy Logo"./>
            <h1>LzyCrazy</h1>
            <p class="subtext">Your Dream, Our Desire</p>
            <p class="subtext">Business &nbsp; Shopping &nbsp; Entertainment</p>
            <div class="search-bar">
                <input type="text" placeholder="Search here..." />
                <i class="fas fa-search"></i>
            </div>

            <div class="nav-buttons">
                <button>About Us</button>
                <button>LzyCrazy Services</button>
                <button>LzyCrazy Marketplace</button>
                <button>We Are Hiring</button>
                <button>LzyCrazy News</button>
            </div>
        </div>

        <div class="right-panel">
            <div class="login-card">
                <input type="email" placeholder="Email Address" />
                <input type="password" placeholder="Password" />
                <a href="#" class="forgot-link">Forgot Password?</a>
                <button class="login-btn">Login</button>

                <div class="divider">or continue with</div>

                <div class="social-buttons">
                    <button><i class="fab fa-google"></i> Google</button>
                    <button><i class="fab fa-facebook-f"></i> Facebook</button>
                </div>


                <button class="create-btn">Create New Account</button>
            </div>
        </div>
    </div>
</body>

</html>
