
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bora se pegar hj?</title>
    <style>
        body {
            background-color: #000;
            color: #fff;
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 20px;
        }
        .opcao {
            position: absolute;
            width: 150px;
            height: 150px;
            background-color: #fff;
            color: #000;
            font-size: 24px;
            line-height: 150px;
            cursor: pointer;
            border: 2px solid transparent;
        }
        .opcao:hover {
            background-color: #ccc;
        }
    </style>
</head>
<body>
    <h1>Bora se pegar hj?</h1>
    
    <a id="sim" class="opcao" href="https://youtu.be/MDmcVLadrmY?si=J8kHHSKdcLNIh5uc" target="_blank">Sim</a>
    <div id="nao" class="opcao nao">Não</div>

    <script>
        var opcaoNao = document.getElementById('nao');

        opcaoNao.addEventListener('click', function() {
            // Muda a posição do botão Não aleatoriamente
            var width = window.innerWidth - 150; // Largura máxima da janela
            var height = window.innerHeight - 150; // Altura máxima da janela
            var newX = Math.floor(Math.random() * width); // Nova posição X
            var newY = Math.floor(Math.random() * height); // Nova posição Y
            opcaoNao.style.left = newX + 'px';
            opcaoNao.style.top = newY + 'px';
        });
    </script>
</body>
</html>
