#### GET request to get the object by id

```
GET http://fake-library.com/api/v1/author/0
```

#### Response

```
HTTP 200 (ok)
Content-Type: application/json
```
```json
{
  "data": {
    "id":0,
    "name": "Arthur",
    "secondName": "Klark"
  },
  "meta": {
    "copyright": "Copyright 2015 Fake Library Corp."
  }
}
```

---

НАЗАД <- [Примеры запросов](./examples.md)