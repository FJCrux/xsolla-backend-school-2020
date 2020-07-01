# Xsolla Summer School 2020. Backend
Привет!
Это небольшое тестовое задание, которое не должно занять много времени.
На выбор дается 2 варианта, их сложность сопоставима, а основная разница в том, что одно из заданий более творческое:

# Вариант 1.
Реализовать собственную платёжную систему, которая будет имитировать процесс оплаты банковской картой.

Пусть это будет сервис с JSON API.
- Должен быть метод, принимающий сумму и назначение платежа и возвращающий sessionId - идентификатором платёжной сессии, например, 4e273d86-864c-429d-879a-34579708dd69.
- Должен быть метод, который принимает данные карты (Номер, CVV/CVC, даты) и sessionId
- Номер карты должен проверяться по алгоритму Луна (упрощенному). Валидные номера должны имитировать успешную оплату, невалидные — возвращать ошибку.

Что можно сделать дополнительно:
- Подготовить OpenAPI-спецификацию (и опубликовать её).
- Покрыть реализацию тестами.
- Ограничить время жизни платёжной сессии.
- Сделать Docker-образ, docker-compose файл
- Добавить API-метод, который возвращает список всех платежей за переданный период (должен быть закрыт авторизацией)
- После успешной оплаты асинхронно отправлять HTTP-уведомление на URL магазина (где URL -- параметр метода из п.2).

# Вариант 2

Реализовать собственную ленту новостей, в которой можно оценить новости и куда можно добавлять новые новости.
Оценить новость одним пользователем можно только один раз, оценку можно отменить.
- Пусть это будет сервис с JSON API
- Должен быть метод получения новостей
- Должен быть метод получения самых интересных новостей (с самими высокими оценками)
- Должен быть метод оценки новости
- Должен быть метод снятия оценки новости

Что можно сделать дополнительно:
- Подготовить OpenAPI-спецификацию (и опубликовать её).
- Покрыть реализацию тестами.
- Сделать фильтрацию новостей по категориям
- Сделать Docker-образ, docker-compose файл

Выбранный вариант не влияет на итоговую оценку, они равнозначны.
Мы ждём от тебя ссылку на github с реализацией на PHP, GoLang или C# (можно использовать любой фреймворк).
По всем вопросам можете писать на p.sanachev@xsolla.com или в наш телеграмм канал https://t.me/xsolla_school_be_2020
