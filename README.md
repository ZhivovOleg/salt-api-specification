# ActiveBC Json Specification

Спецификация Salt:API для использования в REST сервисах и frontend.
<br/>
Версия 0.5.0

> Внимание!<br/>
> Спецификация в версии Pre-Release<br/>
> В случае обнуружения ошибок, неточностей или необходимости исправлений, просьба создавать ISSUE либо писать на [oazhivov@activebc.ru](mailto:oazhivov@activebc.ru) с темой "ActiveBC Json Specification"

# Формат документации
Чтобы начать работу с Salt:API, ознакомьтесь с [документацией по спецификации](./Spec.md)

# Оглавление
- [Спецификация](./Spec.md)
  - [Соглашения по использованию HTTP методов](./verbs/verbs.md)
    - [POST](./verbs/post.md)
    - [GET](./verbs/get.md)
    - [PUT](./verbs/put.md)
    - [PATCH](./verbs/patch.md)
    - [DELETE](./verbs/delete.md)
  - [Соглашения по телу запроса](./document/document.md)
    - [Первичные данные](./document/primary-data.md)
    - [Ошибки](./document/errors.md)
    - [Ссылки](./document/links.md)
    - [Метаинформация](./document/meta.md)
  - [Соглашения по ограничениям запрашиваемых данных](./data-fetching/data-fetching.md)
    - [Фильтры](./data-fetching/filter.md)
    - [Сортировка](./data-fetching/sort.md)
    - [Pagination](./data-fetching/pagination.md)
    - [Разреженные наборы полей](./data-fetching/fieldset.md)
  - [Примеры](./examples/examples.md)
    - [HTTP GET object](./examples/get-object.md)
    - [HTTP GET collection](./examples/get-collection.md)
    - [HTTP POST create object](./examples/post-add.md)
    - [HTTP POST get collection with filters and pagination](./examples/post-filter.md)
    - [HTTP PUT](./examples/put-object.md)
    - [HTTP PATCH](./examples/patch-object.md)
    - [HTTP DELETE](./examples/delete.md)

# RoadMap

1. Исправления битых ссылок после форматирования
0. Добавить в примеры варианты ошибок
0. swagger

# История изменений

