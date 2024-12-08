# miagoath.github.io
# Regenerar el archivo HTML con animación para "¡sorpresa!" en tonos rosa pastel.

html_content = """
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¡Sorpresa!</title>
    <style>
        body {
            margin: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background-color: #ffe6f2; /* Rosa pastel */
            font-family: 'Arial', sans-serif;
        }
        .container {
            text-align: center;
            animation: fadeIn 2s ease-in-out;
        }
        .container h1 {
            font-size: 3rem;
            color: #ff80aa; /* Rosa más oscuro */
            text-shadow: 2px 2px #ffcce0;
        }
        .container p {
            font-size: 1.5rem;
            color: #ff99c2;
        }
        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: scale(0.5);
            }
            to {
                opacity: 1;
                transform: scale(1);
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>¡Sorpresa!</h1>
        <p>Espero que esto te alegre el día :)</p>
    </div>
</body>
</html>
"""

# Guardar el archivo HTML.
file_path = "/mnt/data/sorpresa.html"

with open(file_path, "w") as file:
    file.write(html_content)

file_path
