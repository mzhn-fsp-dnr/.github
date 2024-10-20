# Разработка цифрового решения для администрирования очереди потребителей

## Стек
`Python (sqlalchemy, fastapi, sqlmodel)`, `Typescript (NextJs)`, `Go`, `PostgreSQL`, `Docker`.

## Описание доступных демонстраций

- Демонстрация работы терминала обслуживания клиентов - https://client.mzhn.fun/tos
- Демонстрация работы экрана для отображения текущей очереди - https://client.mzhn.fun/screen
- Telegram-bot для удалённой записи (необходимо отсканировать QR-код в терминале) - [@post_donbass_fsp_bot](https://t.me/post_donbass_fsp_bot)
- Демонстрация работы единого рабочего места сотрудника и администратора - https://admin.mzhn.fun/

## Архитектура проекта:
Приложение спроектировано с помощью `микросервисной архитектуры`. 
Микросервисы позволяют разбить приложение на независимые модули, что упрощает масштабирование и улучшает устойчивость системы к сбоям, так как каждая часть работает автономно.
В качестве основного языка для backend был выбран `Python` (fastapi, sqlalchemy), каждый микросервис имеет свою БД (PostgreSQL). 
Frontend приложение было реализовано с помощью `TypeScript` (NextJS).

![image_2024-10-20_15-41-56](https://github.com/user-attachments/assets/e72497ca-1531-46e6-83aa-0fcb00b71f7d)

## Структура проектов
- [Сервис авторизации](https://github.com/mzhn-fsp-dnr/auth)
- [Сервис генерации PDF](https://github.com/mzhn-fsp-dnr/pdf-generator)
- [Telegram бот](https://github.com/mzhn-fsp-dnr/telegram-bot)
- [Сервис предварительной записи](https://github.com/mzhn-fsp-dnr/prereg)
- [Сервис окон отделений](https://github.com/mzhn-fsp-dnr/windows)
- [Сервис услуг](https://github.com/mzhn-fsp-dnr/services)
- [Сервис работы с очередью](https://github.com/mzhn-fsp-dnr/queue)
- [Сервис работы с отделениями](https://github.com/mzhn-fsp-dnr/offices)
- [Сайт для сотрудников и администраторов](https://github.com/mzhn-fsp-dnr/frontend-admin)
- [Сайт системы для записи, терминала управления очередью](https://github.com/mzhn-fsp-dnr/frontend-client)
- [Презентация](https://github.com/mzhn-fsp-dnr/presentation)
