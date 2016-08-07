# План

* Основы компьютерных сетей
  * Уровни OSI
    
    |Уровень|Тип данных|Пример|   |   |
    |---|---|---|---|---|
    |Прикладной (Application)|   |HTTP|   |   |
    |Представления (Presentation)|   |   |   |   |
    |Сеансовый (Session)|   |   |   |   |
    |Транспортный (transport)|Сегменты|TCP|
    |Сетевой (network)|Пакеты|IP|
    |Канальный (data link)|Кадры|Ethernet|
    |Физический (physical)|Биты|Витая пара|

  * Full-stack пример - от HTTP до Ethernet

    ### HTTP

    ```
    <html>
    <head>
    <title>Заголовок документа</title>
    </head>
    <body>
    Текст на странице
    </body>
    </html>
    ```

    ```
    GET /example.html HTTP/1.1
    Host: example.org
    User-Agent: Mozilla/5.0 (X11; U; Linux i686; ru; rv:1.9b5) Gecko/2008050509 Firefox/3.0b5
    Accept: text/html
    Connection: close
    (пустая строка)  
    ```

    ```
    HTTP/1.1 200 OK
    Date: Wed, 11 Feb 2009 11:20:59 GMT
    Server: Apache
    X-Powered-By: PHP/5.2.4-2ubuntu5wm1
    Last-Modified: Wed, 11 Feb 2009 11:20:59 GMT
    Content-Language: ru
    Content-Type: text/html; charset=utf-8
    Content-Length: 1234
    Connection: close
    (пустая строка)
    (далее следует запрошенная страница в HTML)
    ```

    ### TCP

    Порядок пакетов

    Номера портов

    Например, получится 42 пакета с порта 80 сервера example.org на порт 10000 
    нашего локального компьютера Михаил-ПК

    Имена преобразуются в IP с помощью DNS.

    ### IP

    ```
    example.org: 93.184.216.32

    Михаил-ПК:   84.23.55.75
    ```

    ### Ethernet

    MAC-адреса:

    ```
    example.org: 00-e0-4c-81-86-86

    Михаил-ПК:   01-eb-5e-12-31-16
    ```

* Основы командной строки
  * `ping`, `tracert`

* DNS-регистраторы