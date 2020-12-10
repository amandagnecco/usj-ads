<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calcular Média</title>
</head>
<body>
    <h1>Calcule a sua média aqui</h1>
    <div>
        <label>Digite a N1:</label>
        <input type="text" name="nota 1" id="nota 1"/>
    </div>
    
    <div>
        <label>Digite a N2:</label>
        <input type="text" name="nota 2" id="nota 2"/>
    </div>
    
    <div>
        <label>Digite a N3:</label>
        <input type="text" name="nota 3" id="nota 3"/>
    </div>
    
    <div>
        <button onclick="media()">Calcular média</button>
    </div>
    
    <div>
        <label>Sua média é: </label>
        <input type="text" name="resultado" id="resultado" />
    </div>

    <div id="mensagem">

    <script>
        function media (){
            var n1 = document.getElementById('nota 1').value;
            console.log('nota 1', n1);

            var n2 = document.getElementById('nota 2').value;
            console.log('nota 2', n2);

            var n3 = document.getElementById('nota 3').value;
            console.log('nota 3', n3);

            var somarNotas = (+ n1) + (+ n2) + (+ n3);
            var calcularMedia = (somarNotas)/3;
            console.log('calcularMedia', calcularMedia);

            var resultado = document.getElementById('resultado');
            resultado.value = calcularMedia;

            if (calcularMedia >= 6) {
                alert("Aprovado");
            }else{
                alert("Reprovado")
            }
        }


    </script>
</body>
</html>
