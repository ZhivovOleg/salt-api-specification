# Мета информация

Если указано, `meta` элемент может использоваться для включения нестандартной метаинформации. Значение каждого `meta` члена **ДОЛЖНО(MUST)** быть объектом («метаобъект»).

Любые члены **МОГУТ(MAY)** быть указаны внутри metaобъектов.

Например:
```json
{
  "meta": {
    "copyright": "Copyright 2015 Fake Library Corp.",
    "authors": [
      "Yehuda Katz",
      "Steve Klabnik",
      "Dan Gebhardt",
      "Tyler Kellen"
    ]
  },
  // ...
}
```

---

НАЗАД <- [Структура Body документа](./document.md)