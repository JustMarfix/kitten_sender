# Информация

Создатели бота: [JustMarfix](https://github.com/JustMarfix/) — написание бота и обслуживание системы, [WiSpace](https://github.com/WiSpace) — config.py

**Краткий экскурс.**
Это — Telegram-бот для рассылки котиков раз в определённое время.
Вы можете запустить его самостоятельно, либо воспользоваться работающим решением — [**\(клик\)**](https://t.me/kittensender_bot).

Таймер рассылки котиков реализован через python библиотеку schedule.

**Пример котика из API:**
![](https://sun9-east.userapi.com/sun9-20/s/v1/ig2/ltYIRBV5RBWoSbkOUiRqkMq-yOcvHsj9iY6iw_spwQQeXijYP1c1iyvu8SN_Sgxilu5POLRHoR1W1U_nk82favI5.jpg?size=800x600&quality=95&type=album)

# Установка:

Сперва, установите [Python 3.10 или выше](https://www.python.org/) на свой ПК.

Затем, откройте командную строку или терминал и выполните следующие команды:
```
pip3 install -r <путь до файла requirements.txt>
```
Переименуйте файл `config.py` в `first_config.py`. **Это важно!**

После чего, разверните сервер [MariaDB](https://mariadb.com/) на своём, либо на удалённом ПК.
Создайте таблицу `users` с четырьмя колонками: uid, cid, name и time с типами данных BigINT, BigINT, TEXT и TEXT соответственно.
Впишите данные для входа в файл `first_config.py`.

Следующим шагом, создайте Telegram-бота с помощью BotFather и впишите его токен в соответствующую графу в конфиге.
Наконец, зарегистрируйтесь на сайте [TheCatAPI](https://thecatapi.com/) и получите токен доступа к API. Его также вставьте в нужную строчку в конфиге.

Последний шаг: запустите бота из командной строки/терминала с помощью команды:
```
python3 <путь до файла main.py>
```

**Готово!**
