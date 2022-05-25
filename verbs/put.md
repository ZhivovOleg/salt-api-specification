# PUT
Изменение одного или нескольких полей существующего объекта

## CRUD:
`Update/Replace`

## Аргументы

- `id` объекта передается в строке URL
- любые другие аргументы **ДОЛЖНЫ(MUST)** передаваться в теле [json документа](./../document/document.md)

## Ответы

### Успешно:

#### Запрос коллекции:

`/customer`:
- `Code`: 200 (Ok)

> метод изменяет *ВСЮ* коллекцию!
аналогично sql `UPDATE` без выражения `WHERE`, поэтому в большинстве случаев метод заблокирован и должен возвращать ошибку `405 (Method Not Allowed)`
      
#### Запрос объекта:

`/customers/{id}`:
- `Code`: 200 (Ok)
- `Body`: [Ссылка на измененный объект](./../document/links.md)

### Ошибки

#### Неверный payload
в частности, переданы неверные атрибуты или типы атрибутов

- `Code`: 400 (Bad Request)
- `Body`: [Объект ошибки](./../document/errors.md)

#### Объект с таким ID не найден
- `Code`: 404 (Not Found)
- `Body`: [Объект ошибки](./../document/errors.md)

## Подробно

**PUT** создаёт новый ресурс или заменяет представление целевого ресурса, данными представленными в теле запроса.
Разница между **PUT** и **POST** в том, что **PUT** является [идемпотентным](https://ru.wikipedia.org/wiki/%D0%98%D0%B4%D0%B5%D0%BC%D0%BF%D0%BE%D1%82%D0%B5%D0%BD%D1%82%D0%BD%D0%BE%D1%81%D1%82%D1%8C).

## Примеры PUT

[Пример изменения объекта](../examples/put-object.md)

---

НАЗАД <- [Соглашения об использовании HTTP методов](./verbs.md)