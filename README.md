# back2back_
back server api for post_moderation
Добро пожаловать!
Проект "Модерация постов"
Демо-видео работы приложения можно посмотреть по ссылке: https://www.loom.com/share/9e6dee35a9384f40abc1c6f10f7d894d

Основная информация
Этот readme file содержи пошаговую инструкцию по сборке и запуску приложения.
Данное руководство предполагает наличие установленного IDE и NodeJS (node package manager необходим для запуска и устанавливается вместе с NodeJS) .
Реализация даного техническоо задания выполнени в 2х проектах: серверной и клиентской части.
Серверная часть запускается на порте 5000, и слушает обращения к нему.

Установка
1) Для скачивания серверной части с имитацией API  необходимо пройти на гитхаб по адресу : 
2) Для стягивания приложения на свой IDE необходимо нажать а зеленую кнопку (Code ) и скопировать адрес репозитория, и далее вставить ссылку в соответстующую адресную строку Вашего IDE
(Например, для WebStorm, это будет распологаться во вкладке Git -> Clone -> (Вставляете заранее скопированный в предыдущем шаге URL) -> далее 'Clone"
3) После завершения клонирования репозитория откройте проект, и, с помощью комманды 'npm install' установите пакеты из package.json
4) Для запуска серверной части с коммандной строки введите 'npm start'

5) Для скачивания клиентской части необходимо пройти на гитхаб по адресу : 
2) Для стягивания приложения на свой IDE необходимо так же нажать а зеленую кнопку (Code ) и скопировать адрес репозитория, и далее вставить ссылку в соответстующую адресную строку Вашего IDE
(Например, для WebStorm, это будет распологаться во вкладке Git -> Clone -> (Вставляете заранее скопированный в предыдущем шаге URL) -> далее 'Clone"
3) После завершения клонирования репозитория откройте проект, и, с помощью комманды 'npm install' установите пакеты из package.json
4) Для запуска клиентской части с коммандной строки введите 'npm start'


Работа с приложением:

Сервер и клиент запускаются последовательно. При изначальном запуске клиента, пользователь увидит только заголовок в верхней части экрана с инструкциями. 
При запущеном сервере, во время старта, клиент делает запрос GET на сервер, при нажатии на 'Enter' отображает пакет из первых 10 объектов, подгруженых с http://localhost:5000/cards. 
Схема объектов строго повторяет предложеную в ТЗ. Кнопки принятия решений выбраны основываясь на наименовании принимаемого решения. Таким образом,
 для того чтобы "Одобрить"(approve)- необходимо нажать "А" на английской раскладке, отклонить (disapprove)- "D", передать старшему модератеру(escalate)- "E".

При отоброжении первого пакета 10 "постов", происходит фокусировка на первом "посте", и модератор может начинать принимать решения.
При отработке пакета и нажатии "F7" происходит отправка решений на сервер и последующая загрузка нового пакета.

 Спасибо за просмотр.