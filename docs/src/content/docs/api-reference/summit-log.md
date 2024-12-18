---
title: summit-log
---

## GET show

GET /summit-log/{id}

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|path|string| yes |none|

> Response Examples

> 200 Response

```json
{
  "collectionId": "string",
  "collectionName": "string",
  "created": "2019-08-24T14:15:22Z",
  "date": "2019-08-24",
  "id": "string",
  "text": "string",
  "updated": "2019-08-24T14:15:22Z"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|none|Inline|

### Responses Data Schema

HTTP Status Code **200**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» collectionId|string|true|none||none|
|» collectionName|string|true|none||none|
|» created|string(date-time)|true|none||none|
|» date|string(date)|true|none||none|
|» id|string|true|none||none|
|» text|string|true|none||none|
|» updated|string(date-time)|true|none||none|

HTTP Status Code **404**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» url|string|true|none||none|
|» status|integer|true|none||none|
|» response|object|true|none||none|
|»» code|integer|true|none||none|
|»» message|string|true|none||none|
|»» data|object|true|none||none|
|» isAbort|boolean|true|none||none|
|» originalError|object|true|none||none|
|»» url|string|true|none||none|
|»» status|integer|true|none||none|
|»» data|object|true|none||none|
|»»» code|integer|true|none||none|
|»»» message|string|true|none||none|
|»»» data|object|true|none||none|
|» name|string|true|none||none|

## POST update

POST /summit-log/{id}

> Body Parameters

```json
{
  "date": "2019-08-24",
  "text": "string"
}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|path|string| yes |none|
|Content-Type|header|string| yes |none|
|body|body|object| no |none|
|» date|body|string(date)| yes |none|
|» text|body|string| no |none|

> Response Examples

> 200 Response

```json
{
  "collectionId": "string",
  "collectionName": "string",
  "created": "2019-08-24T14:15:22Z",
  "date": "2019-08-24",
  "id": "string",
  "text": "string",
  "updated": "2019-08-24T14:15:22Z"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|none|Inline|

### Responses Data Schema

HTTP Status Code **200**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» collectionId|string|true|none||none|
|» collectionName|string|true|none||none|
|» created|string(date-time)|true|none||none|
|» date|string(date)|true|none||none|
|» id|string|true|none||none|
|» text|string|true|none||none|
|» updated|string(date-time)|true|none||none|

HTTP Status Code **404**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» url|string|true|none||none|
|» status|integer|true|none||none|
|» response|object|true|none||none|
|»» code|integer|true|none||none|
|»» message|string|true|none||none|
|»» data|object|true|none||none|
|» isAbort|boolean|true|none||none|
|» originalError|object|true|none||none|
|»» url|string|true|none||none|
|»» status|integer|true|none||none|
|»» data|object|true|none||none|
|»»» code|integer|true|none||none|
|»»» message|string|true|none||none|
|»»» data|object|true|none||none|
|» name|string|true|none||none|

## DELETE delete

DELETE /summit-log/{id}

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|path|string| yes |none|

> Response Examples

> 200 Response

```json
{
  "acknowledged": true
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|none|Inline|

### Responses Data Schema

HTTP Status Code **200**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» acknowledged|boolean|true|none||none|

HTTP Status Code **404**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» url|string|true|none||none|
|» status|integer|true|none||none|
|» response|object|true|none||none|
|»» code|integer|true|none||none|
|»» message|string|true|none||none|
|»» data|object|true|none||none|
|» isAbort|boolean|true|none||none|
|» originalError|object|true|none||none|
|»» url|string|true|none||none|
|»» status|integer|true|none||none|
|»» data|object|true|none||none|
|»»» code|integer|true|none||none|
|»»» message|string|true|none||none|
|»»» data|object|true|none||none|
|» name|string|true|none||none|

## POST file

POST /summit-log/{id}/file

> Body Parameters

```yaml
gpx: ""

```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|path|string| yes |none|
|Content-Type|header|string| yes |none|
|body|body|object| no |none|
|» gpx|body|string(binary)| no |none|

> Response Examples

> 200 Response

```json
{}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

## GET list

GET /summit-log

> Response Examples

> 200 Response

```json
[
  {
    "collectionId": "string",
    "collectionName": "string",
    "created": "string",
    "date": "string",
    "id": "string",
    "text": "string",
    "updated": "string"
  }
]
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

HTTP Status Code **200**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» collectionId|string|false|none||none|
|» collectionName|string|false|none||none|
|» created|string|false|none||none|
|» date|string|false|none||none|
|» id|string|false|none||none|
|» text|string|false|none||none|
|» updated|string|false|none||none|

## PUT create

PUT /summit-log

> Body Parameters

```json
{
  "date": "2019-08-24",
  "text": "string"
}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|
|» date|body|string(date)| yes |none|
|» text|body|string| no |none|

> Response Examples

> 200 Response

```json
{
  "collectionId": "string",
  "collectionName": "string",
  "created": "2019-08-24T14:15:22Z",
  "date": "2019-08-24",
  "id": "string",
  "text": "string",
  "updated": "2019-08-24T14:15:22Z"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|
|400|[Bad Request](https://tools.ietf.org/html/rfc7231#section-6.5.1)|none|Inline|

### Responses Data Schema

HTTP Status Code **200**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» collectionId|string|true|none||none|
|» collectionName|string|true|none||none|
|» created|string(date-time)|true|none||none|
|» date|string(date)|true|none||none|
|» id|string|true|none||none|
|» text|string|true|none||none|
|» updated|string(date-time)|true|none||none|

HTTP Status Code **400**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» url|string|true|none||none|
|» status|integer|true|none||none|
|» response|object|true|none||none|
|»» code|integer|true|none||none|
|»» message|string|true|none||none|
|»» data|object|true|none||none|
|» isAbort|boolean|true|none||none|
|» originalError|object|true|none||none|
|»» url|string|true|none||none|
|»» status|integer|true|none||none|
|»» data|object|true|none||none|
|»»» code|integer|true|none||none|
|»»» message|string|true|none||none|
|»»» data|object|true|none||none|
|» name|string|true|none||none|

# Data Schema

