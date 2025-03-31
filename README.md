<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Manon, Femme de mes rêves</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #ff9a8b, #ff6a00);
            color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            flex-direction: column;
            text-align: center;
        }

        h1 {
            font-size: 2.5em;
            margin: 0;
            animation: fadeIn 2s ease-in-out;
        }

        p {
            font-size: 1.2em;
            margin: 15px 0;
            line-height: 1.5;
            animation: fadeIn 3s ease-in-out;
        }

        .heart {
            font-size: 4em;
            color: #ff4d4d;
            margin: 20px 0;
            animation: bounce 2s infinite;
        }

        .btn {
            padding: 15px 30px;
            font-size: 1.2em;
            background-color: #fff;
            color: #ff6a00;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            transition: transform 0.3s, background-color 0.3s;
            margin-top: 30px;
        }

        .btn:hover {
            background-color: #ff6a00;
            color: white;
            transform: scale(1.1);
        }

        footer {
            position: absolute;
            bottom: 20px;
            font-size: 1em;
            color: #fff;
            opacity: 0.7;
        }

        .quote {
            font-style: italic;
            font-size: 1.5em;
            margin-top: 30px;
            animation: fadeIn 4s ease-in-out;
        }

        /* Animations */
        @keyframes fadeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }

        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% {
                transform: translateY(0);
            }
            40% {
                transform: translateY(-10px);
            }
            60% {
                transform: translateY(-5px);
            }
        }

        .message-box {
            margin-top: 40px;
            display: none;
            background: rgba(255, 255, 255, 0.9);
            padding: 20px;
            border-radius: 10px;
            text-align: center;
        }

        input[type="text"] {
            padding: 10px;
            font-size: 1em;
            width: 80%;
            border: none;
            border-radius: 5px;
        }

        button[type="submit"] {
            padding: 10px 20px;
            font-size: 1.2em;
            background-color: #ff6a00;
            color: white;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            margin-top: 10px;
        }
    </style>
</head>
<body>
    <h1>Manon, Femme de mes rêves</h1>
    <div class="heart">❤️</div>
    <p>Manon la première fois que je t'ai vu je t'ai aimé et jusqu'a aujourd'hui je t'ai jamais trahi et je pense que tu es d'accord avec moi 
est ce que s'y on y réfléchis vraiment et qu'on pense vraiment l'un pour l'autre est ce que il y aurai vraiment pas un moyen pour qu'on construise une relation qui j'éspère durera étèrnellement Manon le jour ou tu me dira oui je serais le plus hereux du mon Je t'aime 😊</p>
    <p class="quote">"Tu es la personne qui rend chaque journée plus belle. 😊"</p>
    <button class="btn" onclick="showMessage()">Dis Oui à l'Aventure avec Moi</button>

    <div class="message-box" id="message-box">
        <p>Manon, je crois qu'on pourrait vivre une histoire incroyable ensemble. 💖</p>
        <form id="response-form">
            <input type="text" id="user-response" placeholder="Dis-moi ce que tu en penses !" required>
            <button type="submit">Répondre</button>
        </form>
    </div>

    <footer>
        Crée avec beaucoup de sincérité.
    </footer>

    <script>
        function showMessage() {
            document.getElementById('message-box').style.display = 'block';
        }

        document.getElementById('response-form').addEventListener('submit', function(e) {
            e.preventDefault();
            let response = document.getElementById('user-response').value;
            if (response) {
                document.getElementById('message-box').innerHTML = `<p>Ta réponse : "${response}" 💖</p><p>Manon je peux pas voir ce message 
mais si c'est oui sachent que je suis la pour toi</p>`;
            }
        });
    </script>
</body>
</html>
