#### POST request to create object

```
POST http://fake-library.com/api/v1/author/add
Content-Type: application/json
```
```json
{
  "data": {
    "name": "Arthur",
    "secondName": "Klark"
  }
}
```

#### Response

```
HTTP 201 (created)
Content-Type: application/json
```
```json
{
  "links": {
    "self": "http://fake-library.com/api/v1/author/0"
  },
  "meta": {
    "copyright": "Copyright 2015 Fake Library Corp."
  }
}
```

---

НАЗАД <- [Примеры запросов](./examples.md)