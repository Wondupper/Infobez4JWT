Этапы:
  1. Docker должен быть запущен.
  2. Для запуска достаточно скачать только docker-compose.yaml, открыть папку куда он скачался в терминале и ввести команду: "docker compose up".
  3. Вроде должно работать).

Далее открываем браузер и заходим по адресу: localhost:8080/

В проге есть 3 работающих адреса:

  1.  localhost:8080/sign-up
Регистрируем пользователя в бд. Шлем json:

{
  "username":"<здесь имя> длина от 3 до 20",
  "password":"<пароль длина от 6 до 40>"
}

  2.  localhost:8080/auth
Аутентифицируемся. Шлем json:

{
  "username":"<здесь имя>",
  "password":"<пароль>"
}

  3.  localhost:8080/refresh
Из куки получаем новую пару токенов.
