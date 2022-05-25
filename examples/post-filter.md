#### POST request to get coolection of objects with filter

```
POST http://fake-library.com/api/v1/author/filter
Content-Type: application/json
```
```json
{
  "filter": [
    {
      "field": "name",
      "operator": "eq",
      "value": "Arthur"
    },
    {
      "field": "secondName",
      "operator": "neq",
      "value": "Turgenev"
    }
  ]
}
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
    }
  ],
  "links": {
    "related": [
      "http://fake-library.com/api/v1/author/0"
    ]
  },
  "meta": {
    "copyright": "Copyright 2015 Fake Library Corp."
  }
}
```

---

НАЗАД <- [Примеры запросов](./examples.md)