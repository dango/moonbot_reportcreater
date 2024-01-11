# moonbot_reportcreater

Группа для обсуждения настроек
https://t.me/moonbot_reports

Описание отчетов, вошедших в релиз
https://korenev.notion.site/moonbot-d2fd78fef58b4759b9f2e8a9bd67317b?pvs=4

Описание дополнительных отчетов
https://korenev.notion.site/f143161db11343cebc082aca89b598c1?pvs=4

Возможно платное обучение и помощь в настройке

## Как запустить отчеты
1. Дать программеру код на проверку на предмет уязвимостей и багов.
2. Запустить ordersaver на серверах с мунботом. Создать БД. Инструкция тут https://github.com/tema2002/moonbot_ordersaver
3. Скачать скрипты на свой сервер. На Винде у меня не получилось запустить Django, делал под Убунтой
4. Установить зависимости, указанные в файле requirements.txt - если какие-то библиотеки забыл указать - просьба сообщить, дополню.
5. Создать в телеграме бота. Полученный токен прописать в файле data/report_bot_settings.py
6. В django_project/django_project/settings_local.py прописать настройки БД
7. Запустить файл report_bot.py
8. Открыть бота в телеграм. Ввести /help . Бот выведет инструкцию по запросам. Начать пользоваться

Периодически телеграм отваливается (так же и соединение с Django) и скрипт надо запускать заново. Я сделал скрипт для автозапуска report_bot_runner.py - его можно запустить вместо report_bot.py, тогда в случае отвала соединения бот перезапустится

Кто проверил код на безопасность - отпишитесь плз в группе https://t.me/moonbot_reports или в любой другой, где есть мунботовцы

## Новичкам
Новичкам советую запускать скрипт следующими способами:

1. Установить десктопную Lubuntu (именно Lubuntu - она меньше ресурсов требует), подключаться через удаленный рабочий стол. Скрипт запускать через консоль или через установленный Visual Studio Code
2. Запуск через консоль Ubuntu. Основные команды: “ls” (посмотреть содержимое текущей папки, без кавычек вводится), “cd ..” - подняться уровнем выше, “cd название_папки” - зайти в папку, “python3 report_bot.py” - запустить скрипт
3. При завершении соединения с сервером бот перестанет работать. Чтобы скрипт работал дальше, нужно в консоли зайти в среду screen и уже в ней запускать скрипт. Тогда можно смело закрывать соединение и все будет работать дальше. 

Я выложил файл со настройками от screen (см .screenrc), так эта среда становится более понятной. Этот файл нужно разместить в корне папки пользователя. Например /home/alex

## Отблагодарить разработчика

Поблагодарить разработчика можно
1. переводом usdt TRC20 TEAiv6gtdqjkxqndEYTG8ZYbQeMvfrtPAw
2. не сильно минусящей (а лучше профитной) стратегией
3. рабочими рекомендациями по торговым идеям

## Для связи

https://t.me/KottAlex
