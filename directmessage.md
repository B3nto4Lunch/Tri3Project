<html>
<head>
	<title>User Data Collection Form</title>
	<style>
		body {
			font-family: Arial, sans-serif;
			background-color: #f1f1f1;
		}
		form {
			background-color: #fff;
			padding: 20px;
			border-radius: 5px;
			box-shadow: 0 0 10px rgba(0,0,0,0.1);
			margin: 50px auto;
			width: 500px;
		}
		input[type=text], input[type=email], input[type=password] {
			width: 100%;
			padding: 12px 20px;
			margin: 8px 0;
			box-sizing: border-box;
			border: 2px solid #ccc;
			border-radius: 4px;
			font-size: 16px;
			background-color: #f8f8f8;
		}
		input[type=submit] {
			background-color: #4CAF50;
			color: white;
			padding: 12px 20px;
			border: none;
			border-radius: 4px;
			cursor: pointer;
			font-size: 16px;
			float: right;
		}
		input[type=submit]:hover {
			background-color: #45a049;
		}
		.error {
			color: red;
		}
	</style>
</head>
<body>
	<form>
		<h1>User Data Collection Form</h1>
		<label for="username">Username:</label>
		<input type="text" id="username" name="username" required>
		<label for="email">Email:</label>
		<input type="email" id="email" name="email" required>
		<label for="password">Password:</label>
		<input type="password" id="password" name="password" required>
		<label for="confirmPassword">Confirm Password:</label>
		<input type="password" id="confirmPassword" name="confirmPassword" required>
		<span id="passwordError" class="error"></span>
		<input type="submit" value="Submit">
	</form>

	<script>
		const form = document.querySelector('form');
		const passwordInput = document.querySelector('#password');
		const confirmPasswordInput = document.querySelector('#confirmPassword');
		const passwordError = document.querySelector('#passwordError');

		// Validate password and confirm password match
		confirmPasswordInput.addEventListener('input', () => {
			if (passwordInput.value !== confirmPasswordInput.value) {
				passwordError.textContent = "Passwords do not match";
				confirmPasswordInput.setCustomValidity("Passwords do not match");
			} else {
				passwordError.textContent = "";
				confirmPasswordInput.setCustomValidity("");
			}
		});

		// Submit form
		form.addEventListener('submit', (event) => {
			event.preventDefault();
			console.log('Submitting form...');
			// Add code to send form data to server here
		});
	</script>
</body>
</html>




<html>
  <head>
    <meta charset="UTF-8">
    <title>Collecting User Data</title>
    <style>
      body {
        font-family: Arial, sans-serif;
        background-color: #f2f2f2;
      }

      form {
        background-color: white;
        border-radius: 5px;
        width: 500px;
        margin: 50px auto;
        padding: 20px;
        box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.3);
      }

      input[type="text"],
      input[type="password"],
      input[type="email"],
      input[type="file"] {
        width: 100%;
        padding: 12px 20px;
        margin: 8px 0;
        box-sizing: border-box;
        border: none;
        border-bottom: 2px solid #ccc;
      }

      input[type="submit"] {
        background-color: #4CAF50;
        color: white;
        padding: 12px 20px;
        border: none;
        border-radius: 4px;
        cursor: pointer;
        float: right;
      }

      input[type="submit"]:hover {
        background-color: #45a049;
      }

      label {
        font-weight: bold;
      }

      .error-message {
        color: red;
        font-weight: bold;
        margin-top: 5px;
      }
    </style>
  </head>
  <body>
    <form name="myForm" onsubmit="return validateForm()">
      <label for="username">Username</label>
      <input type="text" id="username" name="username" required>

      <label for="password">Password</label>
      <input type="password" id="password" name="password" required>

      <label for="email">Email</label>
      <input type="email" id="email" name="email" required>

      <label for="photo">Photo</label>
      <input type="file" id="photo" name="photo" accept="image/*">

      <input type="submit" value="Submit">
      <div class="error-message" id="error-message"></div>
    </form>

    <script>
      function validateForm() {
        var username = document.forms["myForm"]["username"].value;
        var password = document.forms["myForm"]["password"].value;
        var email = document.forms["myForm"]["email"].value;
        var photo = document.forms["myForm"]["photo"].value;

        if (username == "") {
          document.getElementById("error-message").innerHTML = "Username is required.";
          return false;
        }

        if (password == "") {
          document.getElementById("error-message").innerHTML = "Password is required.";
          return false;
        }

        if (email == "") {
          document.getElementById("error-message").innerHTML = "Email is required.";
          return false;
        }

        if (photo == "") {
          document.getElementById("error-message").innerHTML = "Photo is required.";
          return false;
        }

        return true;
      }
    </script>
  </body>
</html>




