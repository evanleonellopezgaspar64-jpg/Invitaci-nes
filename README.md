<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>Invitación</title>
<style>
body{
    margin:0;
    background:#1c1c1c;
    color:white;
    font-family:Arial,sans-serif;
    display:flex;
    justify-content:center;
    align-items:center;
    height:100vh;
}
.card{
    width:320px;
    text-align:center;
    padding:30px;
    border-radius:20px;
    background:#2b2b2b;
}
h1{color:#00E5FF;}
button{
    width:220px;
    padding:12px;
    margin:10px;
    border:none;
    border-radius:10px;
    color:white;
    font-size:16px;
    cursor:pointer;
}
.si{background:green;}
.no{background:red;}
#respuesta{
    margin-top:20px;
    font-weight:bold;
}
</style>
</head>
<body>

<div class="card">
<h1>🎉 ¡Estás invitado! 🎉</h1>

<p>
📅 Miércoles<br><br>
Te invitamos cordialmente a nuestra exposición.<br><br>
¿Podrás acompañarnos?
</p>

<button class="si" onclick="asistir()">✅ Asistiré</button><br>
<button class="no" onclick="noAsistire()">❌ No asistiré</button>

<p id="respuesta"></p>
</div>

<script>
function asistir(){
    document.getElementById("respuesta").innerHTML="✅ ¡Gracias por confirmar tu asistencia!";
    document.getElementById("respuesta").style.color="lime";
}

function noAsistire(){
    document.getElementById("respuesta").innerHTML="😢 Gracias por avisarnos.<br>¡Será en otra ocasión!";
    document.getElementById("respuesta").style.color="red";
}
</script>

</body>
</html>
