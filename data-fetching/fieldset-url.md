# Разреженные наборы полей в URL

```
?fields=fieldName1&fields=fieldName2&...
```

где для `fields` в качестве аргументов передаются ожидаемые поля.

В случае указания недопустимого либо несуществующего поля запрашиваемого объекта, сервер **ДОЛЖЕН(MUST)** вернуть ответ `400 Bad Request` с [ошибкой](./../errors.md) в которой будет указан аргумент `fields` со именем недопустимого/несуществующего поля.

---

НАЗАД <- [Ограничениям запрашиваемых данных](./data-fetching.md)