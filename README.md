<!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Basbosa Birthday 🎂</title>

<style>
body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: linear-gradient(135deg, #ff758c, #ff7eb3);
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    text-align: center;
}

.card {
    background: white;
    padding: 30px;
    border-radius: 25px;
    box-shadow: 0 15px 40px rgba(0,0,0,0.2);
    width: 90%;
    max-width: 400px;
    animation: fadeIn 1s ease-in-out;
}

@keyframes fadeIn {
    from {opacity:0; transform:translateY(20px);}
    to {opacity:1; transform:translateY(0);}
}

h1 {
    color: #ff4d6d;
}

input {
    padding: 12px;
    width: 85%;
    border-radius: 15px;
    border: 1px solid #ddd;
    margin: 10px 0;
}

button {
    padding: 10px 20px;
    border: none;
    border-radius: 25px;
    background: #ff4d6d;
    color: white;
    cursor: pointer;
    margin: 5px;
    transition: 0.3s;
}

button:hover {
    background: #e63950;
}

#gift {
    display: none;
}

#message {
    margin-top: 15px;
    font-size: 18px;
    color: #444;
}
</style>
</head>

<body>

<div class="card">

<h2>ادخلي الباسورد يا بسبوسة 🎀</h2>

<input type="password" id="pass">
<br>
<button onclick="check()">دخول</button>

<div id="gift">
    <h1>🎉 Happy Birthday 🎉</h1>
    <button onclick="showMessage()">افتحي الرسالة 💌</button>
    <p id="message"></p>
</div>

</div>

<script>
function check() {
    if (document.getElementById("pass").value == "1234") {
        document.getElementById("gift").style.display = "block";
    } else {
        alert("الباسورد غلط 😅");
    }
}

function showMessage() {
    document.getElementById("message").innerText =
    "كل سنة وانتي طيبة يا أحلى بسبوسة في الدنيا ❤️ وجودك في حياتي نعمة كبيرة.";
}
</script>

</body>
</html>
