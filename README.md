# intec-task1
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Personal Info Page</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        .header {
            display: flex;
            align-items: center;
            gap: 20px;
        }
        .header img {
            width: 300px;
            height: 300px;
            border-radius: 10%;
            object-fit: cover;
        }
        .header h1 {
            font-size: 2rem;
            margin: 0;
        }
        .info {
            margin-top: 20px;
        }
        .info p {
            margin: 5px 0;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
        }
        table, th, td {
            border: 1px solid black;
        }
        th, td {
            padding: 10px;
            text-align: center;
        }
        .input-section {
            margin-top: 40px;
            display: flex;
            justify-content: start;
            align-items: center;
            gap: 20px;
        }
        .input-row {
            display: flex;
            flex-direction: column;
            align-items: flex-start;
        }
        .input-row label {
            margin-bottom: 5px;
            font-size: 14px;
        }
        .input-row input {
            padding: 10px;
            width: 400px;
            box-sizing: border-box;
        }
        .toggle-info-container {
            text-align: center;
            margin-top: 20px;
        }
        .toggle-info {
            text-align: center;
            cursor: pointer;
            color: black;
        }
        .extra-info {
            display: none;
            margin-top: 10px;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="header">
        <img src="photo_2024-10-04_20-01-05.jpg" alt="Profile Photo">
        <div>
            <h1>Дидык Анна</h1>
            <p><strong>Адрес:</strong> Челябинск</p>
            <p><strong>Опыт работы:</strong> Нет</p>
            <p><strong>Телефон:</strong> +7 (982) 100-58-22</p>
            <p><strong>О себе:</strong> 19-летняя студентка ЮУрГУ кафедры ИЕТН</p>
        </div>
    </div>
    <h2>Знание языков:</h2>
    <table>
        <tr>
            <th></th>
            <th>HTML</th>
            <th>JavaScript</th>
            <th>C++</th>
            <th>C#</th>
            <th>Python</th>
        </tr>
        <tr>
            <td>Отличное владение</td>
            <td>Нет</td>
            <td>Нет</td>
            <td>Нет</td>
            <td>Нет</td>
            <td>Да</td>
        </tr>
        <tr>
            <td>Хорошие владение</td>
            <td>Нет</td>
            <td>Нет</td>
            <td>Да</td>
            <td>Да</td>
            <td>Да</td>
        </tr>
        <tr>
            <td>Среднее владение</td>
            <td>Да</td>
            <td>Да</td>
            <td>Да</td>
            <td>Да</td>
            <td>Да</td>
        </tr>
        <tr>
            <td>Плохое владение</td>
            <td>Да</td>
            <td>Да</td>
            <td>Да</td>
            <td>Да</td>
            <td>Да</td>
        </tr>
    </table>
    <div class="input-section">
        <div class="input-row">
            <label for="phone">Телефон:</label>
            <input type="tel" id="phone" name="phone" placeholder="+7 (999) 999-99-99">
        </div>
        <div class="input-row">
            <label for="name">Имя:</label>
            <input type="text" id="name" name="name" placeholder="Введите имя">
        </div>
    </div>    
    <h2 class="toggle-info" style="cursor: pointer; color: black; margin-top: 20px;">
        Кликните сюда, чтобы узнать меня подробнее
    </h2>
    <div class="extra-info" style="display: none; margin-top: 20px;">
        <p><strong>Интересы:</strong> Программирование, видеоигры, путешествия.</p>
        <p><strong>Образование:</strong> 2 курс ЮУрГУ кафедры ИЕТН, направление - "Прикладная математика и информатика".</p>
        <p><strong>Интересный факт:</strong> Подрабатывала в онлайн-школе программирования <i>itgen.io</i> составителем обучающего курса Python базового уровня.</p>
    </div>    
    <script>
        const toggleButton = document.querySelector('.toggle-info');
        const extraInfo = document.querySelector('.extra-info');

        toggleButton.addEventListener('click', () => {
            extraInfo.style.display = extraInfo.style.display === 'none' || extraInfo.style.display === '' 
                ? 'block' 
                : 'none';
        });
    </script>
</body>
</html>
