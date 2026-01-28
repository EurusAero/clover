# Доступ по SSH к Raspberry Pi

На [образе для OPi](image.md) преднастроен доступ по SSH для редактирования файлов, загрузки данных и запуска программ.

Для доступа по SSH необходимо [подключиться к Orange Pi по Wi-Fi](wifi.md) (также возможно подключение через Ethernet-кабель).

В GNU/Linux или macOS необходимо запустить Терминал и выполнить команду:

```bash
ssh orangepi@10.42.0.1
```

Пароль: `orangepi`.

Для доступа по SSH из Windows можно использовать [PuTTY](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html) или веб-доступ (см. далее). Также можно получить доступ по SSH со смартфона с помощью приложения [Termius](https://www.termius.com).

> **Hint** Для того, чтобы не вводить пароль при каждом подключении по SSH, см. [статью об использовании SSH-ключей](ssh_keys.md).

Подробнее: https://www.raspberrypi.org/documentation/remote-access/ssh/README.md.

## Веб-доступ

Начиная с версии 0.11.4 [образа](image.md) доступ к шеллу также доступен через веб-браузер (с использованием [Butterfly](https://github.com/paradoxxxzero/butterfly)). Для доступа откройте страницу http://10.42.0.1 и выберите на ней ссылку _Open web terminal_:

<img src="../assets/butterfly.png">

**Далее**: [Командная строка](cli.md).
