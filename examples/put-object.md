#### PUT request

```
PUT http://fake-library.com/api/v1/author/5
Content-Type: application/json
```
```json
{
  "data":{
    "name": "Ray Douglas"
  }
}
```

#### Response

```
HTTP 200 (ok)
Content-Type: application/json
```
```json
{
  "data": {
    "id": 5,
    "name": "Ray Douglas",
    "secondName": "Bradbury"
  },
  "meta": {
    "copyright": "Copyright 2015 Fake Library Corp."
  }
}
```

---

НАЗАД <- [Примеры запросов](./examples.md)