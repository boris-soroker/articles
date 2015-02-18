***

HTTP POST

Hubot

Webhooks

***

В Kato существует возможность создания связок с внешними сервисами и без помощи инструментов вроде [IFTTT](/articles/ru/fun/ifttt-integration) и [Zapier](/articles/ru/power-users/integrations#zapier).

К примеру, с помощью HTTP POST API пользователи могут генерировать сообщения в комнату Kato, если произойдет какое-либо событие во внешнем сервисе (закончит свою работу скрипт и т.д.).

## <a href="#http-post-api" name="http-post-api">HTTP POST API&#8212;to Kato</a>
<br />
![clip.png](https://s3.amazonaws.com/kato-share/c14d5ddcded3988228d8e2449ff963ebb7bcab06eed6bdd3c50ec041ce878b8/clip.png)

Чтобы отправить сообщение в Kato необходимо создать запрос HTTP POST с объектом JSON следующего формата:

    {
      "from": "Имя",
      "color": "Красный",
      "renderer": "markdown",
      "text": "Сообщение"
    }

А URL должен содержать тип `application/json content:

`https://api.kato.im/rooms/`ROOM ID`/simple`

Все параметры сообщения, кроме `text` опциональны; в поле `color` может быть указан любой html-цвет; поле `renderer` может принимать значения `default`, `code` или `markdown`.

Интеграция HTTP POST представлена по ссылке: <a href="https://app.kato.im/#/integrations/http_post" target="_blank">https://app.kato.im/#/integrations/http_post</a>

## <a href="#webhooks-api" name="webhooks-api">Webhooks API&#8212; от Kato</a>
<br />
![clip.png](https://s3.amazonaws.com/kato-share/b1035cac108ae73dbba55c4be1218d34a8d25e64745746ab65096162e7d9390f/clip.png)
