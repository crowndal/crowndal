<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Login Page</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
    }
    form {
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    input {
      margin-bottom: 10px;
      padding: 8px;
    }
  </style>
</head>
<body>
  <form id="loginForm">
    <label for="username">Username:</label>
    <input type="text" id="username" name="username" required>

    <label for="password">Password:</label>
    <input type="password" id="password" name="password" required>

    <button type="button" onclick="login()">Login</button>
  </form>

  <script>
    function login() {
      var username = document.getElementById('username').value;
      var password = document.getElementById('password').value;

      // 이 부분에서 서버로 실제로 로그인 요청을 보내고 결과를 처리해야 합니다.
      // 여기서는 단순히 콘솔에 출력하는 예시를 보여줍니다.
      console.log('Username:', username);
      console.log('Password:', password);
    }
  </script>
</body>
</html>  
