<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para minha princesa ❤️</title>
    <style>
        body { 
            text-align: center; 
            font-family: Arial, sans-serif; 
            margin: 50px; 
            background-color: #ADD8E6; /* Azul bebê */
            color: black; 
        }
        .container { 
            max-width: 600px; 
            margin: auto; 
            font-size: 20px; 
            line-height: 1.5; 
        }
        .hidden { display: none; }
        button { 
            font-size: 18px; 
            padding: 10px 20px; 
            margin-top: 20px; 
            cursor: pointer; 
            background-color: #87CEEB; /* Azul mais forte */
            border: none;
            color: white;
            border-radius: 10px;
        }
        #no { position: absolute; }
        .heart {
            font-size: 30px;
            animation: float 1.5s infinite ease-in-out alternate;
        }
        @keyframes float {
            from { transform: translateY(0px); }
            to { transform: translateY(-10px); }
        }
    </style>
    <script>
        function showProposal() {
            document.getElementById('intro').style.display = 'none';
            document.getElementById('proposal').style.display = 'block';
        }

        function moveButton() {
            let x = Math.random() * window.innerWidth - 100;
            let y = Math.random() * window.innerHeight - 50;
            document.getElementById('no').style.left = `${x}px`;
            document.getElementById('no').style.top = `${y}px`;
        }
    </script>
</head>
<body>

    <div id="intro" class="container">
        <p class="heart">💙💙💙</p>
        <p>Minha linda princesa, sou grato por você ser essa pessoa incrível, maravilhosa, leal, companheira, compreensiva... simplesmente perfeita.</p>
        <p>Todos os dias agradeço a Deus por ter me presenteado com um amor tão precioso como o seu.</p>
        <p>O tempo só reforçou o quanto eu te quero e me fez perceber que você é a pessoa certa para mim.</p>
        <p>Não há dúvidas: quero estar ao seu lado em todos os momentos, como seu namorado, seu marido, seu melhor amigo... seu tudo.</p>
        <p>Com amor, <b>Zirc</b> para <b>Mhiy</b> 💙</p>
        <p class="heart">💙💙💙</p>
        <button onclick="showProposal()">Próximo ➡️</button>
    </div>

    <div id="proposal" class="container hidden">
        <h1>Quer namorar comigo? 💙</h1>
        <button onclick="alert('Eu te amo! 💙')">Sim</button>
        <button id="no" onmouseover="moveButton()">Não</button>
        <p class="heart">💙💙💙</p>
    </div>

</body>
</html>
