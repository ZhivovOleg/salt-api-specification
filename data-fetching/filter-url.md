# Фильтрация как аргумент URL

```
?filter=field:action:value?filter=field:action:value&...
```

Допустимые значения `action`:
- `eq` - equals
- `ne` - not equals
- `gt` - greater than
- `ge` - greater than or equals to
- `lt` - less than
- `le` - less than or equals to

В случае указания недопустимых значений фильрации, сервер **ДОЛЖЕН(MUST)** вернуть ответ `400 Bad Request` с [ошибкой](./../errors.md) в которой будет указан аргумент `filter` со значением недопустимого фильтра.

---

НАЗАД <- [Ограничениям запрашиваемых данных](./data-fetching.md)