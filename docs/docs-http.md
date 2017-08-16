# 

Testing various
 api 
features



## Server Configuration for Base URLs

This section provides details on the environments available and lists down the servers in each of the environment. The default environment for this API is set to `production` while the default server is set to `default`.
### Environments

An environment consists of a set of servers with base URL values. The environment can be changed programatically allowing rapid switching between different environments e.g.the user can specify a Production and Testing Environment.The available environments for this API are: 

#### production
The environment comprises of the following servers: 

| Name | Base URL | 
|-----------|-------------|
| default | http://apimatic.hopto.org:{suites} |
| auth server | http://apimaticauth.hopto.org:3000 |

#### testing
The environment comprises of the following servers: 

| Name | Base URL | 
|-----------|-------------|
| default | http://192.168.0.100:{port} |
| auth server | http://apimaticauth.xhopto.org:3000 |



### Base URL Parameters
Base URL contains the following parameters:

| Name | Type | Tags | Description | Default Value | 
|------|------| ---- | ----------- | ------------- |
| port | [string](#api_types) |  ``` Optional ```  | TODO: Add a parameter description | `"80"` |
| suites | [SuiteCode](#suite_code) |  ``` Optional ```  | TODO: Add a parameter description | `1` |






## Global API Errors
Global API errors are applied across all endpoints.

**400** 
> 400 Global

**402** 
> 402 Global

**403** 
> 403 Global

**404** 
> 404 Global

**500** 
> 500 Global

Body ([GlobalTestException](#global_test_exception)) 
```
{
  "ServerMessage": "ServerMessage",
  "ServerCode": 24
}
```
**Default** 
> Invalid response.

Body ([GlobalTestException](#global_test_exception)) 
```
{
  "ServerMessage": "ServerMessage",
  "ServerCode": 24
}
```



# <a name="api_reference"></a>API Reference

* [ResponseTypes](#response_types)
* [BodyParams](#body_params)
* [FormParams](#form_params)
* [QueryParam](#query_param)
* [ErrorCodes](#error_codes)
* [Echo](#echo)
* [Header](#header)
* [TemplateParams](#template_params)

## <a name="response_types"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "ResponseTypes") ResponseTypes


### <a name="get_date_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Date Array") Get Date Array


**`GET`** `/response/date`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Responses
**200** 


Body ([DateTime](#api_types)) 
```
[
  "1994-02-13",
  "1994-02-13"
]
```


### <a name="get_date"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Date") Get Date


**`GET`** `/response/date`

> TODO: Add a method description




#### Responses
**200** 


Body ([DateTime](#api_types)) 
```
1994-02-13
```


### <a name="get_long"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Long") Get Long


**`GET`** `/response/long`

> TODO: Add a method description


#### Base URL
This endpoint uses server `default`.


#### Responses
**200** 


Body ([Long](#api_types)) 
```
5147483647
```


### <a name="get_model"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Model") Get Model


**`GET`** `/response/model`

> TODO: Add a method description




#### Responses
**200** 


Body ([Person](#person)) 
```
{
  "name": "Shahid Khaliq",
  "age": 5147483645,
  "address": "H # 531, S # 20",
  "uid": "123321",
  "birthday": "1994-02-13",
  "birthtime": "1994-02-13T14:01:54.9571247Z",
  "salary": 20000,
  "department": "Software Development",
  "joiningDay": "Saturday",
  "workingDays": [
    "Monday",
    "Tuesday",
    "Friday"
  ],
  "boss": {
    "personType": "Boss",
    "name": "Zeeshan Ejaz",
    "age": 5147483645,
    "address": "H # 531, S # 20",
    "uid": "123321",
    "birthday": "1994-02-13",
    "birthtime": "1994-02-13T14:01:54.9571247Z",
    "salary": 20000,
    "department": "Software Development",
    "joiningDay": "Saturday",
    "workingDays": [
      "Monday",
      "Tuesday",
      "Friday"
    ],
    "dependents": [
      {
        "name": "Future Wife",
        "age": 5147483649,
        "address": "H # 531, S # 20",
        "uid": "123412",
        "birthday": "1994-02-13",
        "birthtime": "1994-02-13T14:01:54.9571247Z"
      },
      {
        "name": "Future Kid",
        "age": 5147483648,
        "address": "H # 531, S # 20",
        "uid": "312341",
        "birthday": "1994-02-13",
        "birthtime": "1994-02-13T14:01:54.9571247Z"
      }
    ],
    "hiredAt": "Sun, 06 Nov 1994 08:49:37 GMT",
    "promotedAt": 1484719381
  },
  "dependents": [
    {
      "name": "Future Wife",
      "age": 5147483649,
      "address": "H # 531, S # 20",
      "uid": "123412",
      "birthday": "1994-02-13",
      "birthtime": "1994-02-13T14:01:54.9571247Z"
    },
    {
      "name": "Future Kid",
      "age": 5147483648,
      "address": "H # 531, S # 20",
      "uid": "312341",
      "birthday": "1994-02-13",
      "birthtime": "1994-02-13T14:01:54.9571247Z"
    }
  ],
  "hiredAt": "Sun, 06 Nov 1994 08:49:37 GMT"
}
```


### <a name="get_string_enum_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get String Enum Array") Get String Enum Array


**`GET`** `/response/enum`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 
| type | [string](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `"string"` | 

#### Responses
**200** 


Body ([Days](#days)) 
```
[
  "Tuesday",
  "Saturday",
  "Wednesday",
  "Monday",
  "Sunday"
]
```


### <a name="get_string_enum"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get String Enum") Get String Enum


**`GET`** `/response/enum`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| type | [string](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `"string"` | 

#### Responses
**200** 


Body ([Days](#days)) 
```
Monday
```


### <a name="get_model_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Model Array") Get Model Array


**`GET`** `/response/model`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Responses
**200** 


Body ([Person](#person)) 
```
[
  {
    "name": "Shahid Khaliq",
    "age": 5147483645,
    "address": "H # 531, S # 20",
    "uid": "123321",
    "birthday": "1994-02-13",
    "birthtime": "1994-02-13T14:01:54.9571247Z",
    "salary": 20000,
    "department": "Software Development",
    "joiningDay": "Saturday",
    "workingDays": [
      "Monday",
      "Tuesday",
      "Friday"
    ],
    "boss": {
      "personType": "Boss",
      "name": "Zeeshan Ejaz",
      "age": 5147483645,
      "address": "H # 531, S # 20",
      "uid": "123321",
      "birthday": "1994-02-13",
      "birthtime": "1994-02-13T14:01:54.9571247Z",
      "salary": 20000,
      "department": "Software Development",
      "joiningDay": "Saturday",
      "workingDays": [
        "Monday",
        "Tuesday",
        "Friday"
      ],
      "dependents": [
        {
          "name": "Future Wife",
          "age": 5147483649,
          "address": "H # 531, S # 20",
          "uid": "123412",
          "birthday": "1994-02-13",
          "birthtime": "1994-02-13T14:01:54.9571247Z"
        },
        {
          "name": "Future Kid",
          "age": 5147483648,
          "address": "H # 531, S # 20",
          "uid": "312341",
          "birthday": "1994-02-13",
          "birthtime": "1994-02-13T14:01:54.9571247Z"
        }
      ],
      "hiredAt": "Sun, 06 Nov 1994 08:49:37 GMT",
      "promotedAt": 1484719381
    },
    "dependents": [
      {
        "name": "Future Wife",
        "age": 5147483649,
        "address": "H # 531, S # 20",
        "uid": "123412",
        "birthday": "1994-02-13",
        "birthtime": "1994-02-13T14:01:54.9571247Z"
      },
      {
        "name": "Future Kid",
        "age": 5147483648,
        "address": "H # 531, S # 20",
        "uid": "312341",
        "birthday": "1994-02-13",
        "birthtime": "1994-02-13T14:01:54.9571247Z"
      }
    ],
    "hiredAt": "Sun, 06 Nov 1994 08:49:37 GMT"
  },
  {
    "name": "Shahid Khaliq",
    "age": 5147483645,
    "address": "H # 531, S # 20",
    "uid": "123321",
    "birthday": "1994-02-13",
    "birthtime": "1994-02-13T14:01:54.9571247Z",
    "salary": 20000,
    "department": "Software Development",
    "joiningDay": "Saturday",
    "workingDays": [
      "Monday",
      "Tuesday",
      "Friday"
    ],
    "boss": {
      "personType": "Boss",
      "name": "Zeeshan Ejaz",
      "age": 5147483645,
      "address": "H # 531, S # 20",
      "uid": "123321",
      "birthday": "1994-02-13",
      "birthtime": "1994-02-13T14:01:54.9571247Z",
      "salary": 20000,
      "department": "Software Development",
      "joiningDay": "Saturday",
      "workingDays": [
        "Monday",
        "Tuesday",
        "Friday"
      ],
      "dependents": [
        {
          "name": "Future Wife",
          "age": 5147483649,
          "address": "H # 531, S # 20",
          "uid": "123412",
          "birthday": "1994-02-13",
          "birthtime": "1994-02-13T14:01:54.9571247Z"
        },
        {
          "name": "Future Kid",
          "age": 5147483648,
          "address": "H # 531, S # 20",
          "uid": "312341",
          "birthday": "1994-02-13",
          "birthtime": "1994-02-13T14:01:54.9571247Z"
        }
      ],
      "hiredAt": "Sun, 06 Nov 1994 08:49:37 GMT",
      "promotedAt": 1484719381
    },
    "dependents": [
      {
        "name": "Future Wife",
        "age": 5147483649,
        "address": "H # 531, S # 20",
        "uid": "123412",
        "birthday": "1994-02-13",
        "birthtime": "1994-02-13T14:01:54.9571247Z"
      },
      {
        "name": "Future Kid",
        "age": 5147483648,
        "address": "H # 531, S # 20",
        "uid": "312341",
        "birthday": "1994-02-13",
        "birthtime": "1994-02-13T14:01:54.9571247Z"
      }
    ],
    "hiredAt": "Sun, 06 Nov 1994 08:49:37 GMT"
  }
]
```


### <a name="get_int_enum"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Int Enum") Get Int Enum


**`GET`** `/response/enum`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| type | [string](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `"int"` | 

#### Responses
**200** 


Body ([SuiteCode](#suite_code)) 
```
3
```


### <a name="get_int_enum_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Int Enum Array") Get Int Enum Array


**`GET`** `/response/enum`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 
| type | [string](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `"int"` | 

#### Responses
**200** 


Body ([SuiteCode](#suite_code)) 
```
[
  1,
  3,
  4,
  2,
  3
]
```


### <a name="get_precision"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Precision") Get Precision


**`GET`** `/response/precision`

> TODO: Add a method description




#### Responses
**200** 


Body ([Precision](#api_types)) 
```
4.999
```


### <a name="get_binary"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Binary") Get Binary


**`GET`** `/response/binary`

> gets a binary object




#### Responses
**200** 


Body ([Binary](#api_types)) 
```
http://localhost:3000/response/image
```


### <a name="get_integer"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Integer") Get Integer


**`GET`** `/response/integer`

> Gets a integer response




#### Responses
**200** 


Body ([Number](#api_types)) 
```
4
```


### <a name="get_integer_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Integer Array") Get Integer Array


**`GET`** `/response/integer`

> Get an array of integers.




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Responses
**200** 


Body ([Number](#api_types)) 
```
[
  1,
  2,
  3,
  4,
  5
]
```


### <a name="get_dynamic"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Dynamic") Get Dynamic


**`GET`** `/response/dynamic`

> TODO: Add a method description




#### Responses
**200** 


Body 
```
{
  "method": "GET",
  "body": {},
  "uploadCount": 0
}
```


### <a name="get_dynamic_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Dynamic Array") Get Dynamic Array


**`GET`** `/response/dynamic`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Responses
**200** 


Body 
```
{
  "method": "GET",
  "body": {},
  "uploadCount": 0
}
```


### <a name="get_3339_datetime"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get 3339Datetime") Get 3339Datetime


**`GET`** `/response/3339datetime`

> TODO: Add a method description




#### Responses
**200** 


Body ([DateTime](#api_types)) 
```
2016-03-13T12:52:32.123Z
```


### <a name="get_3339_datetime_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get 3339Datetime Array") Get 3339Datetime Array


**`GET`** `/response/3339datetime`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Responses
**200** 


Body ([DateTime](#api_types)) 
```
[
  "2016-03-13T12:52:32.123Z",
  "2016-03-13T12:52:32.123Z",
  "2016-03-13T12:52:32.123Z"
]
```


### <a name="get_boolean"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Boolean") Get Boolean


**`GET`** `/response/boolean`

> TODO: Add a method description




#### Responses
**200** 


Body ([Boolean](#api_types)) 
```
true
```


### <a name="get_boolean_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Boolean Array") Get Boolean Array


**`GET`** `/response/boolean`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Responses
**200** 


Body ([Boolean](#api_types)) 
```
[
  true,
  false,
  true,
  true,
  false
]
```


### <a name="get_headers"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get Headers") Get Headers


**`GET`** `/response/headers`

> TODO: Add a method description




#### Responses
**200**


### <a name="get_1123_date_time"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get 1123DateTime") Get 1123DateTime


**`GET`** `/response/1123datetime`

> TODO: Add a method description




#### Responses
**200** 


Body ([DateTime](#api_types)) 
```
Sun, 06 Nov 1994 08:49:37 GMT
```


### <a name="get_unix_date_time"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get UnixDateTime") Get UnixDateTime


**`GET`** `/response/unixdatetime`

> TODO: Add a method description




#### Responses
**200** 


Body ([DateTime](#api_types)) 
```
1484719381
```


### <a name="get_1123_date_time_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get 1123DateTime Array") Get 1123DateTime Array


**`GET`** `/response/1123datetime`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Responses
**200** 


Body ([DateTime](#api_types)) 
```
[
  "Sun, 06 Nov 1994 08:49:37 GMT",
  "Sun, 06 Nov 1994 08:49:37 GMT"
]
```


### <a name="get_unix_date_time_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get UnixDateTime Array") Get UnixDateTime Array


**`GET`** `/response/unixdatetime`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Responses
**200** 


Body ([DateTime](#api_types)) 
```
[
  1484719381,
  1484719381
]
```


[Back to API Reference](#api_reference)

## <a name="body_params"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "BodyParams") BodyParams


### <a name="send_date_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Date Array") Send Date Array


**`POST`** `/body/date`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [DateTime](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add description | 

 Example 
``` 
[
  "1994-02-13",
  "1994-02-13"
]
``` 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_date"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Date") Send Date


**`POST`** `/body/date`

> TODO: Add a method description




#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [DateTime](#api_types) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
1994-02-13
``` 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_unix_date_time"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send UnixDateTime") Send UnixDateTime


**`POST`** `/body/unixdatetime`

> TODO: Add a method description




#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [DateTime](#api_types) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
1484719381
``` 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_rfc1123_date_time"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Rfc1123 DateTime") Send Rfc1123 DateTime


**`POST`** `/body/rfc1123datetime`

> TODO: Add a method description




#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [DateTime](#api_types) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
Sun, 06 Nov 1994 08:49:37 GMT
``` 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_rfc3339_date_time"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Rfc3339 DateTime") Send Rfc3339 DateTime


**`POST`** `/body/rfc3339datetime`

> TODO: Add a method description




#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [DateTime](#api_types) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
1994-02-13T14:01:54.9571247Z
``` 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_unix_date_time_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send UnixDateTime Array") Send UnixDateTime Array


**`POST`** `/body/unixdatetime`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [DateTime](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add description | 

 Example 
``` 
[
  1484719381,
  1484719381
]
``` 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_rfc1123_date_time_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Rfc1123 DateTime Array") Send Rfc1123 DateTime Array


**`POST`** `/body/rfc1123datetime`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [DateTime](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add description | 

 Example 
``` 
[
  "Sun, 06 Nov 1994 08:49:37 GMT",
  "Sun, 06 Nov 1994 08:49:37 GMT"
]
``` 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_rfc3339_date_time_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Rfc3339 DateTime Array") Send Rfc3339 DateTime Array


**`POST`** `/body/rfc3339datetime`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [DateTime](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add description | 

 Example 
``` 
[
  "1994-02-13T14:01:54.9571247Z",
  "1994-02-13T14:01:54.9571247Z"
]
``` 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_string_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send String Array") Send String Array


**`POST`** `/body/string`

> sends a string body param




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [String](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add description | 

 Example 
``` 
[
  "abc",
  "def"
]
``` 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_integer_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Integer Array") Send Integer Array


**`POST`** `/body/number`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [Number](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add description | 

 Example 
``` 
[
  1,
  2,
  3,
  4,
  5
]
``` 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_model"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Model") Send Model


**`POST`** `/body/model`

> TODO: Add a method description




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [Employee](#employee) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "name": "Shahid Khaliq",
  "age": 5147483645,
  "address": "H # 531, S # 20",
  "uid": "123321",
  "birthday": "1994-02-13",
  "birthtime": "1994-02-13T14:01:54.9571247Z",
  "salary": 20000,
  "department": "Software Development",
  "joiningDay": "Saturday",
  "workingDays": [
    "Monday",
    "Tuesday",
    "Friday"
  ],
  "boss": {
    "personType": "Boss",
    "name": "Zeeshan Ejaz",
    "age": 5147483645,
    "address": "H # 531, S # 20",
    "uid": "123321",
    "birthday": "1994-02-13",
    "birthtime": "1994-02-13T14:01:54.9571247Z",
    "salary": 20000,
    "department": "Software Development",
    "joiningDay": "Saturday",
    "workingDays": [
      "Monday",
      "Tuesday",
      "Friday"
    ],
    "dependents": [
      {
        "name": "Future Wife",
        "age": 5147483649,
        "address": "H # 531, S # 20",
        "uid": "123412",
        "birthday": "1994-02-13",
        "birthtime": "1994-02-13T14:01:54.9571247Z"
      },
      {
        "name": "Future Kid",
        "age": 5147483648,
        "address": "H # 531, S # 20",
        "uid": "312341",
        "birthday": "1994-02-13",
        "birthtime": "1994-02-13T14:01:54.9571247Z"
      }
    ],
    "hiredAt": "Sun, 06 Nov 1994 08:49:37 GMT",
    "promotedAt": 1484719381
  },
  "dependents": [
    {
      "name": "Future Wife",
      "age": 5147483649,
      "address": "H # 531, S # 20",
      "uid": "123412",
      "birthday": "1994-02-13",
      "birthtime": "1994-02-13T14:01:54.9571247Z"
    },
    {
      "name": "Future Kid",
      "age": 5147483648,
      "address": "H # 531, S # 20",
      "uid": "312341",
      "birthday": "1994-02-13",
      "birthtime": "1994-02-13T14:01:54.9571247Z"
    }
  ],
  "hiredAt": "Sun, 06 Nov 1994 08:49:37 GMT"
}
``` 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_model_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Model Array") Send Model Array


**`POST`** `/body/model`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [Employee](#employee) |  ``` Required ```  ``` Collection ```  | TODO: Add description | 

 Example 
``` 
[
  {
    "name": "Shahid Khaliq",
    "age": 5147483645,
    "address": "H # 531, S # 20",
    "uid": "123321",
    "birthday": "1994-02-13",
    "birthtime": "1994-02-13T14:01:54.9571247Z",
    "salary": 20000,
    "department": "Software Development",
    "joiningDay": "Saturday",
    "workingDays": [
      "Monday",
      "Tuesday",
      "Friday"
    ],
    "boss": {
      "personType": "Boss",
      "name": "Zeeshan Ejaz",
      "age": 5147483645,
      "address": "H # 531, S # 20",
      "uid": "123321",
      "birthday": "1994-02-13",
      "birthtime": "1994-02-13T14:01:54.9571247Z",
      "salary": 20000,
      "department": "Software Development",
      "joiningDay": "Saturday",
      "workingDays": [
        "Monday",
        "Tuesday",
        "Friday"
      ],
      "dependents": [
        {
          "name": "Future Wife",
          "age": 5147483649,
          "address": "H # 531, S # 20",
          "uid": "123412",
          "birthday": "1994-02-13",
          "birthtime": "1994-02-13T14:01:54.9571247Z"
        },
        {
          "name": "Future Kid",
          "age": 5147483648,
          "address": "H # 531, S # 20",
          "uid": "312341",
          "birthday": "1994-02-13",
          "birthtime": "1994-02-13T14:01:54.9571247Z"
        }
      ],
      "hiredAt": "Sun, 06 Nov 1994 08:49:37 GMT",
      "promotedAt": 1484719381
    },
    "dependents": [
      {
        "name": "Future Wife",
        "age": 5147483649,
        "address": "H # 531, S # 20",
        "uid": "123412",
        "birthday": "1994-02-13",
        "birthtime": "1994-02-13T14:01:54.9571247Z"
      },
      {
        "name": "Future Kid",
        "age": 5147483648,
        "address": "H # 531, S # 20",
        "uid": "312341",
        "birthday": "1994-02-13",
        "birthtime": "1994-02-13T14:01:54.9571247Z"
      }
    ],
    "hiredAt": "Sun, 06 Nov 1994 08:49:37 GMT"
  },
  {
    "name": "Shahid Khaliq",
    "age": 5147483645,
    "address": "H # 531, S # 20",
    "uid": "123321",
    "birthday": "1994-02-13",
    "birthtime": "1994-02-13T14:01:54.9571247Z",
    "salary": 20000,
    "department": "Software Development",
    "joiningDay": "Saturday",
    "workingDays": [
      "Monday",
      "Tuesday",
      "Friday"
    ],
    "boss": {
      "personType": "Boss",
      "name": "Zeeshan Ejaz",
      "age": 5147483645,
      "address": "H # 531, S # 20",
      "uid": "123321",
      "birthday": "1994-02-13",
      "birthtime": "1994-02-13T14:01:54.9571247Z",
      "salary": 20000,
      "department": "Software Development",
      "joiningDay": "Saturday",
      "workingDays": [
        "Monday",
        "Tuesday",
        "Friday"
      ],
      "dependents": [
        {
          "name": "Future Wife",
          "age": 5147483649,
          "address": "H # 531, S # 20",
          "uid": "123412",
          "birthday": "1994-02-13",
          "birthtime": "1994-02-13T14:01:54.9571247Z"
        },
        {
          "name": "Future Kid",
          "age": 5147483648,
          "address": "H # 531, S # 20",
          "uid": "312341",
          "birthday": "1994-02-13",
          "birthtime": "1994-02-13T14:01:54.9571247Z"
        }
      ],
      "hiredAt": "Sun, 06 Nov 1994 08:49:37 GMT",
      "promotedAt": 1484719381
    },
    "dependents": [
      {
        "name": "Future Wife",
        "age": 5147483649,
        "address": "H # 531, S # 20",
        "uid": "123412",
        "birthday": "1994-02-13",
        "birthtime": "1994-02-13T14:01:54.9571247Z"
      },
      {
        "name": "Future Kid",
        "age": 5147483648,
        "address": "H # 531, S # 20",
        "uid": "312341",
        "birthday": "1994-02-13",
        "birthtime": "1994-02-13T14:01:54.9571247Z"
      }
    ],
    "hiredAt": "Sun, 06 Nov 1994 08:49:37 GMT"
  }
]
``` 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_dynamic"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Dynamic") Send Dynamic


**`POST`** `/body/dynamic`

> TODO: Add a method description




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [Object](#api_types) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "uid": "1123213",
  "name": "Shahid"
}
``` 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_string"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send String") Send String


**`POST`** `/body/string`

> TODO: Add a method description




#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [String](#api_types) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
TestString
``` 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_string_enum_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "SendStringEnumArray") SendStringEnumArray


**`POST`** `/body/stringenum`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [Days](#days) |  ``` Required ```  ``` Collection ```  | TODO: Add description | 

 Example 
``` 
[
  "Tuesday",
  "Saturday",
  "Wednesday",
  "Monday",
  "Sunday"
]
``` 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_integer_enum_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "SendIntegerEnumArray") SendIntegerEnumArray


**`POST`** `/body/integerenum`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [SuiteCode](#suite_code) |  ``` Required ```  ``` Collection ```  | TODO: Add description | 

 Example 
``` 
[
  1,
  3,
  4,
  2,
  3
]
``` 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


[Back to API Reference](#api_reference)

## <a name="form_params"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "FormParams") FormParams


### <a name="send_date_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Date Array") Send Date Array


**`POST`** `/form/date`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Request Headers
>Content-Type=application/x-www-form-urlencoded;

#### Request Body
Url Encoded

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| dates | [datetime](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |  | 

##### Example
```
 dates = ["1994-02-13","1994-02-13"] 
```

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_date"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Date") Send Date


**`POST`** `/form/date`

> TODO: Add a method description




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;

#### Request Body
Url Encoded

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| date | [datetime](#api_types) |  ``` Required ```  | TODO: Add a parameter description |  | 

##### Example
```
 date = 1994-02-13 
```

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_unix_date_time"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send UnixDateTime") Send UnixDateTime


**`POST`** `/form/unixdatetime`

> TODO: Add a method description




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;

#### Request Body
Url Encoded

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| datetime | [datetime](#api_types) |  ``` Required ```  | TODO: Add a parameter description |  | 

##### Example
```
 datetime = 1484719381 
```

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_rfc1123_date_time"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Rfc1123 DateTime") Send Rfc1123 DateTime


**`POST`** `/form/rfc1123datetime`

> TODO: Add a method description




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;

#### Request Body
Url Encoded

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| datetime | [datetime](#api_types) |  ``` Required ```  | TODO: Add a parameter description |  | 

##### Example
```
 datetime = Sun, 06 Nov 1994 08:49:37 GMT 
```

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_rfc3339_date_time"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Rfc3339 DateTime") Send Rfc3339 DateTime


**`POST`** `/form/rfc3339datetime`

> TODO: Add a method description




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;

#### Request Body
Url Encoded

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| datetime | [datetime](#api_types) |  ``` Required ```  | TODO: Add a parameter description |  | 

##### Example
```
 datetime = 1994-02-13T14:01:54.9571247Z 
```

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_unix_date_time_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send UnixDateTime Array") Send UnixDateTime Array


**`POST`** `/form/unixdatetime`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Request Headers
>Content-Type=application/x-www-form-urlencoded;

#### Request Body
Url Encoded

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| datetimes | [datetime](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |  | 

##### Example
```
 datetimes = [1484719381,1484719381] 
```

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_rfc1123_date_time_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Rfc1123 DateTime Array") Send Rfc1123 DateTime Array


**`POST`** `/form/rfc1123datetime`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Request Headers
>Content-Type=application/x-www-form-urlencoded;

#### Request Body
Url Encoded

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| datetimes | [datetime](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |  | 

##### Example
```
 datetimes = ["Sun, 06 Nov 1994 08:49:37 GMT","Sun, 06 Nov 1994 08:49:37 GMT"] 
```

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_long"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Long") Send Long


**`POST`** `/form/number`

> TODO: Add a method description




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;

#### Request Body
Url Encoded

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| value | [long](#api_types) |  ``` Required ```  | TODO: Add a parameter description |  | 

##### Example
```
 value = 5147483647 
```

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_integer_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Integer Array") Send Integer Array


**`POST`** `/form/number`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Request Headers
>Content-Type=application/x-www-form-urlencoded;

#### Request Body
Url Encoded

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| integers | [number](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |  | 

##### Example
```
 integers = [1,2,3,4,5] 
```

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_string_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send String Array") Send String Array


**`POST`** `/form/string`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Request Headers
>Content-Type=application/x-www-form-urlencoded;

#### Request Body
Url Encoded

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| strings | [string](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |  | 

##### Example
```
 strings = ["abc","def"] 
```

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_model"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Model") Send Model


**`POST`** `/form/model`

> TODO: Add a method description




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;

#### Request Body
Url Encoded

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| model | [Employee](#employee) |  ``` Required ```  | TODO: Add a parameter description |  | 

##### Example
```
 model[name] = Shahid Khaliq 
 model[age] = 5147483645 
 model[address] = H # 531, S # 20 
 model[uid] = 123321 
 model[birthday] = 1994-02-13 
 model[birthtime] = 2/13/1994 2:01:54 PM 
 model[salary] = 20000 
 model[department] = Software Development 
 model[joiningDay] = Saturday 
 model[workingDays][0] = Monday 
 model[workingDays][1] = Tuesday 
 model[workingDays][2] = Friday 
 model[boss][personType] = Boss 
 model[boss][name] = Zeeshan Ejaz 
 model[boss][age] = 5147483645 
 model[boss][address] = H # 531, S # 20 
 model[boss][uid] = 123321 
 model[boss][birthday] = 1994-02-13 
 model[boss][birthtime] = 2/13/1994 2:01:54 PM 
 model[boss][salary] = 20000 
 model[boss][department] = Software Development 
 model[boss][joiningDay] = Saturday 
 model[boss][workingDays][0] = Monday 
 model[boss][workingDays][1] = Tuesday 
 model[boss][workingDays][2] = Friday 
 model[boss][dependents][0][name] = Future Wife 
 model[boss][dependents][0][age] = 5147483649 
 model[boss][dependents][0][address] = H # 531, S # 20 
 model[boss][dependents][0][uid] = 123412 
 model[boss][dependents][0][birthday] = 1994-02-13 
 model[boss][dependents][0][birthtime] = 2/13/1994 2:01:54 PM 
 model[boss][dependents][1][name] = Future Kid 
 model[boss][dependents][1][age] = 5147483648 
 model[boss][dependents][1][address] = H # 531, S # 20 
 model[boss][dependents][1][uid] = 312341 
 model[boss][dependents][1][birthday] = 1994-02-13 
 model[boss][dependents][1][birthtime] = 2/13/1994 2:01:54 PM 
 model[boss][hiredAt] = Sun, 06 Nov 1994 08:49:37 GMT 
 model[boss][promotedAt] = 1484719381 
 model[dependents][0][name] = Future Wife 
 model[dependents][0][age] = 5147483649 
 model[dependents][0][address] = H # 531, S # 20 
 model[dependents][0][uid] = 123412 
 model[dependents][0][birthday] = 1994-02-13 
 model[dependents][0][birthtime] = 2/13/1994 2:01:54 PM 
 model[dependents][1][name] = Future Kid 
 model[dependents][1][age] = 5147483648 
 model[dependents][1][address] = H # 531, S # 20 
 model[dependents][1][uid] = 312341 
 model[dependents][1][birthday] = 1994-02-13 
 model[dependents][1][birthtime] = 2/13/1994 2:01:54 PM 
 model[hiredAt] = Sun, 06 Nov 1994 08:49:37 GMT 
```

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_model_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Model Array") Send Model Array


**`POST`** `/form/model`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Request Headers
>Content-Type=application/x-www-form-urlencoded;

#### Request Body
Url Encoded

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| models | [Employee](#employee) |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |  | 

##### Example
```
 models[0][name] = Shahid Khaliq 
 models[0][age] = 5147483645 
 models[0][address] = H # 531, S # 20 
 models[0][uid] = 123321 
 models[0][birthday] = 1994-02-13 
 models[0][birthtime] = 2/13/1994 2:01:54 PM 
 models[0][salary] = 20000 
 models[0][department] = Software Development 
 models[0][joiningDay] = Saturday 
 models[0][workingDays][0] = Monday 
 models[0][workingDays][1] = Tuesday 
 models[0][workingDays][2] = Friday 
 models[0][boss][personType] = Boss 
 models[0][boss][name] = Zeeshan Ejaz 
 models[0][boss][age] = 5147483645 
 models[0][boss][address] = H # 531, S # 20 
 models[0][boss][uid] = 123321 
 models[0][boss][birthday] = 1994-02-13 
 models[0][boss][birthtime] = 2/13/1994 2:01:54 PM 
 models[0][boss][salary] = 20000 
 models[0][boss][department] = Software Development 
 models[0][boss][joiningDay] = Saturday 
 models[0][boss][workingDays][0] = Monday 
 models[0][boss][workingDays][1] = Tuesday 
 models[0][boss][workingDays][2] = Friday 
 models[0][boss][dependents][0][name] = Future Wife 
 models[0][boss][dependents][0][age] = 5147483649 
 models[0][boss][dependents][0][address] = H # 531, S # 20 
 models[0][boss][dependents][0][uid] = 123412 
 models[0][boss][dependents][0][birthday] = 1994-02-13 
 models[0][boss][dependents][0][birthtime] = 2/13/1994 2:01:54 PM 
 models[0][boss][dependents][1][name] = Future Kid 
 models[0][boss][dependents][1][age] = 5147483648 
 models[0][boss][dependents][1][address] = H # 531, S # 20 
 models[0][boss][dependents][1][uid] = 312341 
 models[0][boss][dependents][1][birthday] = 1994-02-13 
 models[0][boss][dependents][1][birthtime] = 2/13/1994 2:01:54 PM 
 models[0][boss][hiredAt] = Sun, 06 Nov 1994 08:49:37 GMT 
 models[0][boss][promotedAt] = 1484719381 
 models[0][dependents][0][name] = Future Wife 
 models[0][dependents][0][age] = 5147483649 
 models[0][dependents][0][address] = H # 531, S # 20 
 models[0][dependents][0][uid] = 123412 
 models[0][dependents][0][birthday] = 1994-02-13 
 models[0][dependents][0][birthtime] = 2/13/1994 2:01:54 PM 
 models[0][dependents][1][name] = Future Kid 
 models[0][dependents][1][age] = 5147483648 
 models[0][dependents][1][address] = H # 531, S # 20 
 models[0][dependents][1][uid] = 312341 
 models[0][dependents][1][birthday] = 1994-02-13 
 models[0][dependents][1][birthtime] = 2/13/1994 2:01:54 PM 
 models[0][hiredAt] = Sun, 06 Nov 1994 08:49:37 GMT 
 models[1][name] = Shahid Khaliq 
 models[1][age] = 5147483645 
 models[1][address] = H # 531, S # 20 
 models[1][uid] = 123321 
 models[1][birthday] = 1994-02-13 
 models[1][birthtime] = 2/13/1994 2:01:54 PM 
 models[1][salary] = 20000 
 models[1][department] = Software Development 
 models[1][joiningDay] = Saturday 
 models[1][workingDays][0] = Monday 
 models[1][workingDays][1] = Tuesday 
 models[1][workingDays][2] = Friday 
 models[1][boss][personType] = Boss 
 models[1][boss][name] = Zeeshan Ejaz 
 models[1][boss][age] = 5147483645 
 models[1][boss][address] = H # 531, S # 20 
 models[1][boss][uid] = 123321 
 models[1][boss][birthday] = 1994-02-13 
 models[1][boss][birthtime] = 2/13/1994 2:01:54 PM 
 models[1][boss][salary] = 20000 
 models[1][boss][department] = Software Development 
 models[1][boss][joiningDay] = Saturday 
 models[1][boss][workingDays][0] = Monday 
 models[1][boss][workingDays][1] = Tuesday 
 models[1][boss][workingDays][2] = Friday 
 models[1][boss][dependents][0][name] = Future Wife 
 models[1][boss][dependents][0][age] = 5147483649 
 models[1][boss][dependents][0][address] = H # 531, S # 20 
 models[1][boss][dependents][0][uid] = 123412 
 models[1][boss][dependents][0][birthday] = 1994-02-13 
 models[1][boss][dependents][0][birthtime] = 2/13/1994 2:01:54 PM 
 models[1][boss][dependents][1][name] = Future Kid 
 models[1][boss][dependents][1][age] = 5147483648 
 models[1][boss][dependents][1][address] = H # 531, S # 20 
 models[1][boss][dependents][1][uid] = 312341 
 models[1][boss][dependents][1][birthday] = 1994-02-13 
 models[1][boss][dependents][1][birthtime] = 2/13/1994 2:01:54 PM 
 models[1][boss][hiredAt] = Sun, 06 Nov 1994 08:49:37 GMT 
 models[1][boss][promotedAt] = 1484719381 
 models[1][dependents][0][name] = Future Wife 
 models[1][dependents][0][age] = 5147483649 
 models[1][dependents][0][address] = H # 531, S # 20 
 models[1][dependents][0][uid] = 123412 
 models[1][dependents][0][birthday] = 1994-02-13 
 models[1][dependents][0][birthtime] = 2/13/1994 2:01:54 PM 
 models[1][dependents][1][name] = Future Kid 
 models[1][dependents][1][age] = 5147483648 
 models[1][dependents][1][address] = H # 531, S # 20 
 models[1][dependents][1][uid] = 312341 
 models[1][dependents][1][birthday] = 1994-02-13 
 models[1][dependents][1][birthtime] = 2/13/1994 2:01:54 PM 
 models[1][hiredAt] = Sun, 06 Nov 1994 08:49:37 GMT 
```

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_file"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send File") Send File


**`POST`** `/form/file`

> TODO: Add a method description




#### Request Headers
>Content-Type=multipart/form-data;

#### Request Body
Multipart Form Data

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| file | [file](#api_types) |  ``` Required ```  | TODO: Add a parameter description |  | 

##### Example
```
 file = http://localhost:3000/response/image 
```

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_string"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send String") Send String


**`POST`** `/form/string`

> TODO: Add a method description




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;

#### Request Body
Url Encoded

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| value | [string](#api_types) |  ``` Required ```  | TODO: Add a parameter description |  | 

##### Example
```
 value = TestString 
```

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_rfc3339_date_time_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Rfc3339 DateTime Array") Send Rfc3339 DateTime Array


**`POST`** `/form/rfc3339datetime`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Request Headers
>Content-Type=application/x-www-form-urlencoded;

#### Request Body
Url Encoded

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| datetimes | [datetime](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |  | 

##### Example
```
 datetimes = ["1994-02-13T14:01:54.9571247Z","1994-02-13T14:01:54.9571247Z"] 
```

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_mixed_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "SendMixedArray") SendMixedArray


**`POST`** `/form/mixed`

> Send a variety for form params. Returns file count and body params




#### Request Headers
>Content-Type=multipart/form-data;

#### Request Body
Multipart Form Data

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| file | [file](#api_types) |  ``` Required ```  | TODO: Add a parameter description |  | 
| integers | [number](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |  | 
| models | [Employee](#employee) |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |  | 
| strings | [string](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |  | 

##### Example
```
 file = http://localhost:3000/response/image 
 integers = [1,2,3,4,5] 
 models[0][name] = Shahid Khaliq 
 models[0][age] = 5147483645 
 models[0][address] = H # 531, S # 20 
 models[0][uid] = 123321 
 models[0][birthday] = 1994-02-13 
 models[0][birthtime] = 2/13/1994 2:01:54 PM 
 models[0][salary] = 20000 
 models[0][department] = Software Development 
 models[0][joiningDay] = Saturday 
 models[0][workingDays][0] = Monday 
 models[0][workingDays][1] = Tuesday 
 models[0][workingDays][2] = Friday 
 models[0][boss][personType] = Boss 
 models[0][boss][name] = Zeeshan Ejaz 
 models[0][boss][age] = 5147483645 
 models[0][boss][address] = H # 531, S # 20 
 models[0][boss][uid] = 123321 
 models[0][boss][birthday] = 1994-02-13 
 models[0][boss][birthtime] = 2/13/1994 2:01:54 PM 
 models[0][boss][salary] = 20000 
 models[0][boss][department] = Software Development 
 models[0][boss][joiningDay] = Saturday 
 models[0][boss][workingDays][0] = Monday 
 models[0][boss][workingDays][1] = Tuesday 
 models[0][boss][workingDays][2] = Friday 
 models[0][boss][dependents][0][name] = Future Wife 
 models[0][boss][dependents][0][age] = 5147483649 
 models[0][boss][dependents][0][address] = H # 531, S # 20 
 models[0][boss][dependents][0][uid] = 123412 
 models[0][boss][dependents][0][birthday] = 1994-02-13 
 models[0][boss][dependents][0][birthtime] = 2/13/1994 2:01:54 PM 
 models[0][boss][dependents][1][name] = Future Kid 
 models[0][boss][dependents][1][age] = 5147483648 
 models[0][boss][dependents][1][address] = H # 531, S # 20 
 models[0][boss][dependents][1][uid] = 312341 
 models[0][boss][dependents][1][birthday] = 1994-02-13 
 models[0][boss][dependents][1][birthtime] = 2/13/1994 2:01:54 PM 
 models[0][boss][hiredAt] = Sun, 06 Nov 1994 08:49:37 GMT 
 models[0][boss][promotedAt] = 1484719381 
 models[0][dependents][0][name] = Future Wife 
 models[0][dependents][0][age] = 5147483649 
 models[0][dependents][0][address] = H # 531, S # 20 
 models[0][dependents][0][uid] = 123412 
 models[0][dependents][0][birthday] = 1994-02-13 
 models[0][dependents][0][birthtime] = 2/13/1994 2:01:54 PM 
 models[0][dependents][1][name] = Future Kid 
 models[0][dependents][1][age] = 5147483648 
 models[0][dependents][1][address] = H # 531, S # 20 
 models[0][dependents][1][uid] = 312341 
 models[0][dependents][1][birthday] = 1994-02-13 
 models[0][dependents][1][birthtime] = 2/13/1994 2:01:54 PM 
 models[0][hiredAt] = Sun, 06 Nov 1994 08:49:37 GMT 
 models[1][name] = Shahid Khaliq 
 models[1][age] = 5147483645 
 models[1][address] = H # 531, S # 20 
 models[1][uid] = 123321 
 models[1][birthday] = 1994-02-13 
 models[1][birthtime] = 2/13/1994 2:01:54 PM 
 models[1][salary] = 20000 
 models[1][department] = Software Development 
 models[1][joiningDay] = Saturday 
 models[1][workingDays][0] = Monday 
 models[1][workingDays][1] = Tuesday 
 models[1][workingDays][2] = Friday 
 models[1][boss][personType] = Boss 
 models[1][boss][name] = Zeeshan Ejaz 
 models[1][boss][age] = 5147483645 
 models[1][boss][address] = H # 531, S # 20 
 models[1][boss][uid] = 123321 
 models[1][boss][birthday] = 1994-02-13 
 models[1][boss][birthtime] = 2/13/1994 2:01:54 PM 
 models[1][boss][salary] = 20000 
 models[1][boss][department] = Software Development 
 models[1][boss][joiningDay] = Saturday 
 models[1][boss][workingDays][0] = Monday 
 models[1][boss][workingDays][1] = Tuesday 
 models[1][boss][workingDays][2] = Friday 
 models[1][boss][dependents][0][name] = Future Wife 
 models[1][boss][dependents][0][age] = 5147483649 
 models[1][boss][dependents][0][address] = H # 531, S # 20 
 models[1][boss][dependents][0][uid] = 123412 
 models[1][boss][dependents][0][birthday] = 1994-02-13 
 models[1][boss][dependents][0][birthtime] = 2/13/1994 2:01:54 PM 
 models[1][boss][dependents][1][name] = Future Kid 
 models[1][boss][dependents][1][age] = 5147483648 
 models[1][boss][dependents][1][address] = H # 531, S # 20 
 models[1][boss][dependents][1][uid] = 312341 
 models[1][boss][dependents][1][birthday] = 1994-02-13 
 models[1][boss][dependents][1][birthtime] = 2/13/1994 2:01:54 PM 
 models[1][boss][hiredAt] = Sun, 06 Nov 1994 08:49:37 GMT 
 models[1][boss][promotedAt] = 1484719381 
 models[1][dependents][0][name] = Future Wife 
 models[1][dependents][0][age] = 5147483649 
 models[1][dependents][0][address] = H # 531, S # 20 
 models[1][dependents][0][uid] = 123412 
 models[1][dependents][0][birthday] = 1994-02-13 
 models[1][dependents][0][birthtime] = 2/13/1994 2:01:54 PM 
 models[1][dependents][1][name] = Future Kid 
 models[1][dependents][1][age] = 5147483648 
 models[1][dependents][1][address] = H # 531, S # 20 
 models[1][dependents][1][uid] = 312341 
 models[1][dependents][1][birthday] = 1994-02-13 
 models[1][dependents][1][birthtime] = 2/13/1994 2:01:54 PM 
 models[1][hiredAt] = Sun, 06 Nov 1994 08:49:37 GMT 
 strings = ["abc","def"] 
```

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_integer_enum_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "SendIntegerEnumArray") SendIntegerEnumArray


**`POST`** `/form/integerenum`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Request Headers
>Content-Type=application/x-www-form-urlencoded;

#### Request Body
Url Encoded

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| suites | [SuiteCode](#suite_code) |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |  | 

##### Example
```
 suites[0] = 1 
 suites[1] = 3 
 suites[2] = 4 
 suites[3] = 2 
 suites[4] = 3 
```

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="send_string_enum_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "SendStringEnumArray") SendStringEnumArray


**`POST`** `/form/stringenum`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example/Default |
|-----------|------| ---- |-------------| -------------------------------- |
| array | [boolean](#api_types) |  ```Constant ```  ``` Required ```  | TODO: Add a parameter description | **Default:** `true` | 

#### Request Headers
>Content-Type=application/x-www-form-urlencoded;

#### Request Body
Url Encoded

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| days | [Days](#days) |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |  | 

##### Example
```
 days = ["Tuesday","Saturday","Wednesday","Monday","Sunday"] 
```

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


[Back to API Reference](#api_reference)

## <a name="query_param"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "QueryParam") QueryParam


### <a name="date_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Date Array") Date Array


**`GET`** `/query/datearray`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| dates | [datetime](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description | `["1994-02-13","1994-02-13"]` | 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="date"></a>![Endpoint: ](https://apidocs.io/img/method.png "Date") Date


**`GET`** `/query/date`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| date | [datetime](#api_types) |  ``` Required ```  | TODO: Add a parameter description | `1994-02-13` | 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="unix_date_time_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Unix DateTime Array") Unix DateTime Array


**`GET`** `/query/unixdatetimearray`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| datetimes | [datetime](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description | `[1484719381,1484719381]` | 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="unix_date_time"></a>![Endpoint: ](https://apidocs.io/img/method.png "Unix DateTime") Unix DateTime


**`GET`** `/query/unixdatetime`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| datetime | [datetime](#api_types) |  ``` Required ```  | TODO: Add a parameter description | `1484719381` | 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="rfc1123_date_time"></a>![Endpoint: ](https://apidocs.io/img/method.png "Rfc1123 DateTime") Rfc1123 DateTime


**`GET`** `/query/rfc1123datetime`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| datetime | [datetime](#api_types) |  ``` Required ```  | TODO: Add a parameter description | `Sun, 06 Nov 1994 08:49:37 GMT` | 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="rfc1123_date_time_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Rfc1123 DateTime Array") Rfc1123 DateTime Array


**`GET`** `/query/rfc1123datetimearray`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| datetimes | [datetime](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description | `["Sun, 06 Nov 1994 08:49:37 GMT","Sun, 06 Nov 1994 08:49:37 GMT"]` | 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="rfc3339_date_time_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Rfc3339 DateTime Array") Rfc3339 DateTime Array


**`GET`** `/query/rfc3339datetimearray`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| datetimes | [datetime](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description | `["1994-02-13T14:01:54.9571247Z","1994-02-13T14:01:54.9571247Z"]` | 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="rfc3339_date_time"></a>![Endpoint: ](https://apidocs.io/img/method.png "Rfc3339 DateTime") Rfc3339 DateTime


**`GET`** `/query/rfc3339datetime`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| datetime | [datetime](#api_types) |  ``` Required ```  | TODO: Add a parameter description | `1994-02-13T14:01:54.9571247Z` | 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="no_params"></a>![Endpoint: ](https://apidocs.io/img/method.png "NoParams") NoParams


**`GET`** `/query/noparams`

> TODO: Add a method description




#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="string_param"></a>![Endpoint: ](https://apidocs.io/img/method.png "StringParam") StringParam


**`GET`** `/query/stringparam`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| string | [string](#api_types) |  ``` Required ```  | TODO: Add a parameter description | `l;asd;asdwe[2304&&;'.d??\a\\\;sd//` | 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="url_param"></a>![Endpoint: ](https://apidocs.io/img/method.png "UrlParam") UrlParam


**`GET`** `/query/urlparam`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| url | [string](#api_types) |  ``` Required ```  | TODO: Add a parameter description | `https://www.shahidisawesome.com/and/also/a/narcissist?thisis=aparameter&another=one` | 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="number_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Number Array") Number Array


**`GET`** `/query/numberarray`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| integers | [number](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description | `[1,2,3,4,5]` | 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="string_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "String Array") String Array


**`GET`** `/query/stringarray`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| strings | [string](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description | `["abc","def"]` | 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="simple_query"></a>![Endpoint: ](https://apidocs.io/img/method.png "SimpleQuery") SimpleQuery


**`GET`** `/query`

> TODO: Add a method description




#### Query Parameters
> Additional optional query parameters are allowed

| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| boolean | [boolean](#api_types) |  ``` Required ```  | TODO: Add a parameter description | `true` | 
| number | [number](#api_types) |  ``` Required ```  | TODO: Add a parameter description | `4` | 
| string | [string](#api_types) |  ``` Required ```  | TODO: Add a parameter description | `TestString` | 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="string_enum_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "String Enum Array") String Enum Array


**`GET`** `/query/stringenumarray`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| days | [Days](#days) |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description | `["Tuesday","Saturday","Wednesday","Monday","Sunday"]` | 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="multiple_params"></a>![Endpoint: ](https://apidocs.io/img/method.png "MultipleParams") MultipleParams


**`GET`** `/query/multipleparams`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| number | [number](#api_types) |  ``` Required ```  | TODO: Add a parameter description | `123412312` | 
| precision | [precision](#api_types) |  ``` Required ```  | TODO: Add a parameter description | `1112.34` | 
| string | [string](#api_types) |  ``` Required ```  | TODO: Add a parameter description | `""test./;";12&&3asl"";"qw1&34"///..//.` | 
| url | [string](#api_types) |  ``` Required ```  | TODO: Add a parameter description | `http://www.abc.com/test?a=b&c="http://lolol.com?param=no&another=lol"` | 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


### <a name="integer_enum_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Integer Enum Array") Integer Enum Array


**`GET`** `/query/integerenumarray`

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| suites | [SuiteCode](#suite_code) |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description | `[1,3,4,2,3]` | 

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


[Back to API Reference](#api_reference)

## <a name="error_codes"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "ErrorCodes") ErrorCodes


### <a name="get400"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get400") Get400


**`GET`** `/error/400`

> TODO: Add a method description




#### Responses
**200** 


Body


### <a name="get500"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get500") Get500


**`GET`** `/error/500`

> TODO: Add a method description




#### Responses
**200** 


Body


### <a name="get401"></a>![Endpoint: ](https://apidocs.io/img/method.png "Get401") Get401


**`GET`** `/error/401`

> TODO: Add a method description




#### Responses
**200** 


Body 


**401** 

> 401 Local

Body ([LocalTestException](#local_test_exception)) 
**421** 

> Default

Body ([LocalTestException](#local_test_exception)) 
```
{
  "SecretMessageForEndpoint": "SecretMessageForEndpoint",
  "ServerMessage": "ServerMessage",
  "ServerCode": 207
}
```
**431** 

> Default

Body ([LocalTestException](#local_test_exception)) 
```
{
  "SecretMessageForEndpoint": "SecretMessageForEndpoint",
  "ServerMessage": "ServerMessage",
  "ServerCode": 207
}
```
**432** 

> Default

Body ([LocalTestException](#local_test_exception)) 
```
{
  "SecretMessageForEndpoint": "SecretMessageForEndpoint",
  "ServerMessage": "ServerMessage",
  "ServerCode": 207
}
```
**441** 

> Default

Body ([LocalTestException](#local_test_exception)) 
```
{
  "SecretMessageForEndpoint": "SecretMessageForEndpoint",
  "ServerMessage": "ServerMessage",
  "ServerCode": 207
}
```
**Default** 

> Invalid response.

Body ([LocalTestException](#local_test_exception)) 
```
{
  "SecretMessageForEndpoint": "SecretMessageForEndpoint",
  "ServerMessage": "ServerMessage",
  "ServerCode": 207
}
```


[Back to API Reference](#api_reference)

## <a name="echo"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Echo") Echo


### <a name="json_echo"></a>![Endpoint: ](https://apidocs.io/img/method.png "Json echo") Json echo


**`POST`** `/`

> Echo's back the request




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [Object](#api_types) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "uid": "1123213",
  "name": "Shahid"
}
``` 

#### Responses
**200** 


Body 
```
{
  "body": {
    "uid": "1123213",
    "name": "Shahid"
  }
}
```


### <a name="form_echo"></a>![Endpoint: ](https://apidocs.io/img/method.png "Form Echo") Form Echo


**`POST`** `/`

> Sends the request including any form params as JSON




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;

#### Request Body
Url Encoded

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| input | [object](#api_types) |  ``` Required ```  | TODO: Add a parameter description |  | 

##### Example
```
 input = {"uid":"1123213","name":"Shahid"} 
```

#### Responses
**200** 


Body 
```
{
  "body": {
    "input": {
      "uid": "1123213",
      "name": "Shahid"
    }
  }
}
```


### <a name="query_echo"></a>![Endpoint: ](https://apidocs.io/img/method.png "QueryEcho") QueryEcho


**`GET`** `/`

> TODO: Add a method description




#### Query Parameters
> Additional optional query parameters are allowed

#### Responses
**200** 


Body ([EchoResponse](#echo_response)) 
```
{
  "query": {
    "hello": "world"
  }
}
```


[Back to API Reference](#api_reference)

## <a name="header"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Header") Header


### <a name="send_headers"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Headers") Send Headers


**`POST`** `/header`

> Sends a single header params




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>custom-header=TestString;

#### Request Body
Url Encoded

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| value | [string](#api_types) |  ``` Required ```  | Represents the value of the custom header |  | 

##### Example
```
 value = TestString 
```

#### Responses
**200** 


Body ([ServerResponse](#server_response)) 
```
{
  "passed": true
}
```


[Back to API Reference](#api_reference)

## <a name="template_params"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "TemplateParams") TemplateParams


### <a name="send_string_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send String Array") Send String Array


**`GET`** `/{strings}`

> TODO: Add a method description




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| strings | [string](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description | `["abc","def"]` | 

#### Responses
**200** 


Body ([EchoResponse](#echo_response)) 
```
{
  "path": "/abc/def"
}
```


### <a name="send_integer_array"></a>![Endpoint: ](https://apidocs.io/img/method.png "Send Integer Array") Send Integer Array


**`GET`** `/{integers}`

> TODO: Add a method description




#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ----------------------------------- |
| integers | [number](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description | `[1,2,3,4,5]` | 

#### Responses
**200** 


Body ([EchoResponse](#echo_response)) 
```
{
  "path": "/1/2/3/4/5"
}
```


[Back to API Reference](#api_reference)

## <a name="api_types"></a>![Models: ](https://apidocs.io/img/class.png "API Types") API Types

This section provides details on the available types. The primitive types available are:

| Type | Example |
| ---- | -------- |
| **string** | `hello world` |
| **boolean** |	`true` |
| **number** | `1` |
| **precision** | `1.5` |
| **datetime** | `2016-03-13T12:52:32.123Z` |
| **date** | `2016-03-13` |
|**void** | |
| **dynamic** | |
| **binary** | |
| **long** | `12345678910` |
| **file** | |
| **uuid** | `0f8fad5b-d9cb-469f-a165-70867728950e` |


In addition to the above types, the following complex types are also available:
### <a name="employee"></a>![Model: ](https://apidocs.io/img/method.png "Employee") Employee



> TODO: Add a method description


#### Base Type
This type inherits from type [Person](#person).


| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| department | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| dependents | [Person](#person) |  ``` Required ```  ``` Collection ```  | TODO: Add a property description | 
| hiredAt | [datetime](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| joiningDay | [Days](#days) |  ``` Required ```  | TODO: Add a property description | 
| salary | [number](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| workingDays | [Days](#days) |  ``` Required ```  ``` Collection ```  | TODO: Add a property description | 
| boss | [Person](#person) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="boss"></a>![Model: ](https://apidocs.io/img/method.png "Boss") Boss



> Testing circular reference.


#### Base Type
This type inherits from type [Employee](#employee).


| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| promotedAt | [datetime](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| assistant | [Employee](#employee) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="days"></a>![Model: ](https://apidocs.io/img/method.png "Days") Days



> A string enum representing days of the week




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `Sunday` | TODO: Add description | 
| `Monday` | TODO: Add description | 
| `Tuesday` | TODO: Add description | 
| `Wednesday` | TODO: Add description | 
| `Thursday` | TODO: Add description | 
| `Friday` | TODO: Add description | 
| `Saturday` | TODO: Add description | 




### <a name="local_test_exception"></a>![Model: ](https://apidocs.io/img/method.png "LocalTestException") LocalTestException



> To test specific local exceptions.


#### Base Type
This type inherits from type [GlobalTestException](#global_test_exception).


| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| SecretMessageForEndpoint | [string](#api_types) |  ``` Required ```  | Represents the specific endpoint info | 




### <a name="global_test_exception"></a>![Model: ](https://apidocs.io/img/method.png "GlobalTestException") GlobalTestException



> To test specific global exceptions.




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| ServerMessage | [string](#api_types) |  ``` Required ```  | Represents the server's exception message | 
| ServerCode | [number](#api_types) |  ``` Required ```  | Represents the server's error code | 




### <a name="echo_response"></a>![Model: ](https://apidocs.io/img/method.png "EchoResponse") EchoResponse



> Raw http Request info




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| body | [object](#api_types) |  ``` Optional ```  ``` Dictionary ```  | TODO: Add a property description | 
| headers | [string](#api_types) |  ``` Optional ```  ``` Dictionary ```  | TODO: Add a property description | 
| method | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| path | [string](#api_types) |  ``` Optional ```  | relativePath | 
| query | [QueryParameter](#query_parameter) |  ``` Optional ```  ``` Dictionary ```  | TODO: Add a property description | 
| uploadCount | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="suite_code"></a>![Model: ](https://apidocs.io/img/method.png "SuiteCode") SuiteCode



> A integer based enum representing a Suite in a game of cards




This type must take a value from the following [number](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `1` | TODO: Add description | 
| `2` | TODO: Add description | 
| `3` | TODO: Add description | 
| `4` | TODO: Add description | 




### <a name="person"></a>![Model: ](https://apidocs.io/img/method.png "Person") Person



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| address | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| age | [long](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| birthday | [datetime](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| birthtime | [datetime](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| name | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| uid | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| personType | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="server_response"></a>![Model: ](https://apidocs.io/img/method.png "ServerResponse") ServerResponse



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| passed | [boolean](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| Message | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| input | [object](#api_types) |  ``` Optional ```  ``` Dictionary ```  | TODO: Add a property description | 




### <a name="query_parameter"></a>![Model: ](https://apidocs.io/img/method.png "QueryParameter") QueryParameter



> Query parameter key value pair echoed back from the server.




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| key | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description |

