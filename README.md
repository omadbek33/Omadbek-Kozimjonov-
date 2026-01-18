# Omadbek-Kozimjonov-
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>Kalkulyator</title>
</head>
<body>

<h2>Kalkulyator</h2>

<input id="a" type="number">
<input id="b" type="number">

<br><br>

<button onclick="hisob('+')">+</button>
<button onclick="hisob('-')">-</button>
<button onclick="hisob('*')">*</button>
<button onclick="hisob('/')">/</button>

<p id="natija"></p>

<script>
function hisob(amal) {
  let a = parseFloat(document.getElementById("a").value);
  let b = parseFloat(document.getElementById("b").value);
  let r = 0;

  if (amal == '+') r = a + b;
  if (amal == '-') r = a - b;
  if (amal == '*') r = a * b;
  if (amal == '/') r = b != 0 ? a / b : "Xato!";

  document.getElementById("natija").innerHTML = "Natija: " + r;
}
</script>

</body>
</html>
