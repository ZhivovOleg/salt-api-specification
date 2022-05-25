#### GET request to get a coolection of all objects

```
GET http://fake-library.com/api/v1/author
```

#### Response

```
HTTP 200 (ok)
Content-Type: application/json
```
```json
{
  "data": [
    {
      "id": 0,
      "name": "Arthur",
      "secondName": "Klark"
    },
    {
      "id": 1,
      "name": "Frank",
      "secondName": "Herbert"
    },
    {
      "id": 3,
      "name": "Isaac",
      "secondName": "Azimov"
    },
    {
      "id": 4,
      "name": "George",
      "secondName": "Orwell"
    },
    {
      "id": 5,
      "name": "Ray",
      "secondName": "Bradbury"
    },
  ],
  "meta": {
    "copyright": "Copyright 2015 Fake Library Corp."
  }
}
```

---

НАЗАД <- [Примеры запросов](./examples.md)