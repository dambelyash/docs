---
editable: false
---

# Метод getFunctionVersion

 

 
## HTTP-запрос {#https-request}
```
GET undefined/functions/v1alpha/versions/{functionVersionId}
```
 
## Path-параметры {#path_params}
 
Параметр | Описание
--- | ---
functionVersionId | Обязательное поле.
 
## Ответ {#responses}
**HTTP Code: 200 - OK**

```json 
{
  "id": "string",
  "functionId": "string",
  "description": "string",
  "createdAt": "string",
  "runtime": "string",
  "entrypoint": "string",
  "resources": {
    "memory": "string"
  },
  "executionTimeout": "string",
  "imageSize": "string",
  "status": "string",
  "tags": [
    "string"
  ]
}
```

 
Поле | Описание
--- | ---
id | **string**<br>
functionId | **string**<br>
description | **string**<br>
createdAt | **string** (date-time)<br><p>Строка в формате <a href="https://www.ietf.org/rfc/rfc3339.txt">RFC3339</a>.</p> 
runtime | **string**<br>
entrypoint | **string**<br>
resources | **object**<br>
resources.<br>memory | **string** (int64)<br><p>Допустимые значения — от 33554432 до 1073741824 включительно.</p> 
executionTimeout | **string**<br>
imageSize | **string** (int64)<br>
status | **string**<br>
tags[] | **string**<br>