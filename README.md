<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Fun Surprise Box</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #fafafa;
      margin: 0;
      padding: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }.container {
  width: 350px;
  background: white;
  padding: 25px;
  border-radius: 15px;
  box-shadow: 0 4px 15px rgba(0,0,0,0.1);
  text-align: center;
}

h2 {
  margin-bottom: 20px;
}

input {
  width: 90%;
  padding: 10px;
  border-radius: 7px;
  border: 1px solid #bbb;
  margin-bottom: 15px;
}

button {
  padding: 10px 20px;
  background: #ffbf00;
  border: none;
  border-radius: 7px;
  cursor: pointer;
  font-size: 16px;
}

#box {
  margin-top: 20px;
  width: 150px;
  height: 150px;
  background: #ffdd66;
  border-radius: 10px;
  display: none;
  justify-content: center;
  align-items: center;
  cursor: pointer;
  font-weight: bold;
}

#resultImg {
  width: 180px;
  margin-top: 20px;
  display: none;
}
p{
  color: #555;
  font-size: 14px;
}

  </style>
</head>
<body>
  <div class="container">
    <h2>Welcome 🎁</h2>
    <p>Enter your number and open the magic surprise box!</p><input type="number" id="num" placeholder="Enter your number..." />
<button onclick="showBox()">Continue</button>

<div id="box" onclick="openBox()">📦 Open Box</div>

<img id="resultImg" src="https://i.postimg.cc/QNMP0tr5/cat.png" />

<p id="tag" style="display:none;">Ye aapka samaan niche gir gaya tha 😺🧠</p>

  </div>  <script>
    function showBox() {
      let n = document.getElementById("num").value;
      if(n === ""){
        alert("Please enter number!");
        return;
      }
      document.getElementById("box").style.display = "flex";
    }

    function openBox(){
      document.getElementById("resultImg").style.display = "block";
      document.getElementById("tag").style.display = "block";
    }
  </script></body>
</html>
