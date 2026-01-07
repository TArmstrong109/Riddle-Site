<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Party Riddle Challenge</title>
<style>
    body {
        font-family: Arial, sans-serif;
        background: #f4f4f4;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        height: 100vh;
        margin: 0;
    }
    .container {
        background: white;
        padding: 20px;
        border-radius: 10px;
        box-shadow: 0 4px 8px rgba(0,0,0,0.2);
        text-align: center;
        max-width: 500px;
    }
    h2 {
        color: #2c3e50;
    }
    p {
        font-size: 16px;
        line-height: 1.6;
        color: #333;
    }
    input {
        padding: 10px;
        width: 80%;
        margin-top: 10px;
        font-size: 16px;
    }
    button {
        padding: 10px 20px;
        margin-top: 10px;
        font-size: 16px;
        background: #007BFF;
        color: white;
        border: none;
        border-radius: 5px;
        cursor: pointer;
    }
    button:hover {
        background: #0056b3;
    }
    #secret {
        display: none;
        margin-top: 20px;
        font-weight: bold;
        color: #2c3e50;
    }
</style>
<script>
function checkPassword() {
    var password = document.getElementById("password").value.trim().toLowerCase();
    if(password === "leonardo dicaprio") {
        document.getElementById("secret").style.display = "block";
    } else {
        alert("Wrong answer! Try again.");
    }
}
</script>
</head>
<body>
<div class="container">
    <h2>Solve the Riddle to Unlock the Party Address</h2>
    <p>
        I’ve chased a light across a bay,<br>
        In gilded halls where secrets sway.<br>
        I’ve frozen deep where lovers weep,<br>
        Beneath the waves where dreams don’t keep.<br><br>
        I’ve wandered lands both harsh and wild,<br>
        With nature’s wrath and fate reviled.<br>
        I’ve built a world inside a dream,<br>
        Where time is fluid, not what it seems.<br><br>
        My name’s a blend of art and lore,<br>
        A painter’s touch, an actor’s core.<br>
        Who am I, whose fame does grow,<br>
        From roaring twenties to icy snow?
    </p>
    <input type="text" id="password" placeholder="Enter your answer">
    <button onclick="checkPassword()">Submit</button>
    <div id="secret">
        🎉 <strong>Party Address:</strong> 123 Celebration Street, Perth 🎉
    </div>
</div>
</body>
</html>
