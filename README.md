<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Приветствие</title>
</head>
<body>
    <h1>Добро пожаловать!</h1>
    <p id="greeting"></p>

    <script>
        // Получаем имя пользователя при загрузке страницы
        document.addEventListener("DOMContentLoaded", function() {
            var name = prompt("Пожалуйста, введите ваше имя:");
            if (name != null && name != "") {
                // Отображаем приветствие с именем пользователя
                document.getElementById("greeting").innerHTML = "Привет, " + name + "!";
            } else {
                // Если пользователь не ввел имя, отображаем общее приветствие
                document.getElementById("greeting").innerHTML = "Добро пожаловать!";
            }
        });
    </script>
</body>
</html>
