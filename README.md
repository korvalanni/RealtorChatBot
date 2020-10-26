# RealtorChatBot
Цель проекта
Создать экосистему по поиску жилья через диалоговый интерфейс.
Задача 1
Реализовать бота, с помощью которого по заданными параметрам (цена, район, количество комнат) можно найти квартиру для покупки.


№	Подзадача	Интерес с точки зрения ООП
1	Реализовать два диалоговых интерфейса взаимодействия с ботом: через телеграм и через консоль.	Необходимо создать удобную инфраструктуру для работы одной и той же логики с разными платформами.
2	Реализовать логику поиска подходящих квартир.	Необходимо создать удобный интерфейс взаимодействия логики и отображения. Например, некоторые данные удобно отобразить в телеграме через кнопки, а в консоли - через нумерованные списки. Обе платформы должны использовать одинаковый результат от модуля логики.
3	Использовать кнопки для телеграма.	Дополнительная проверка того, что логика не зависит от представления.


Поскольку основной целью этой задачи является создание удобной для расширения архитектуры, то данные отходят на второй план, поэтому для тестирования возможностей бота будет подготовлена небольшая выборка квартир (например, json-файл).

 
Задача 2
Реализовать сервис, который парсит сайты с объявлениями (ЦИАН и Авито) и сохраняет их в базу данных. Бот должен брать объявления из базы данных.

№	Подзадача	Интерес с точки зрения ООП
1	Реализовать общий интерфейс парсеров.	Реализовать нужно так, чтобы для парсинга нового сайта нужно было дописать только класс парсера, а вся остальная логика оставалась неизменной.
2	Реализовать общий интерфейс для работы с базой данных, чтобы бизнес-логика не зависела от базы данных.	Аналогично подзадаче 1.
