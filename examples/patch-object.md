#### PATCH request

```
PATCH http://fake-library.com/api/v1/author/0
Content-Type: application/json
```
```json
{
  "op": "add",
    "value": {  
      "age": "52" 
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
    "secondName": "Bradbury",
    "age": "52"
  },
  "meta": {
    "copyright": "Copyright 2015 Fake Library Corp."
  }
}
```

---

НАЗАД <- [Примеры запросов](./examples.md)