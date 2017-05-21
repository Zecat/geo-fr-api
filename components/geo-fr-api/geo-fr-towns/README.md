## &lt;geo-fr-towns&gt;

geo-fr-towns gives you an array of french towns description from the filters you give it.

It requests the [french governmental geo api](https://api.gouv.fr/api/api-geo.html) `/communes` endpoint using an iron-ajax element.

### Filters

Filters are properties  `name`, `code`, `postalCode`, `departementCode`, `regionCode`, `format`, `geometry`, `latitude`, `longitude`
Use and combine them to refine the search.

### Model

After a success request, the `value` property contains an array of town descriptions with the following model:

```json
[
  {
    "code": "string",
    "nom": "string",
    "codesPostaux": [
      "string"
    ],
    "codeDepartement": "string",
    "codeRegion": "string",
    "population": "int",
    "_score": "float"
  }
]
```

You can restrict the fields using `fields` property.

For exemple, with the following restrictions :

```html
<geo-fr-api fields='["code", "nom"]'></geo-fr-api>
```

You will get this model :

```json
[
  {
    "code": "string",
    "nom": "string"
  }
]
```

### Auto

With `auto` set to true, the element performs a new request whenever the `fields` or a "filter property" changes.
