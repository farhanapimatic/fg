# Getting started

Testing various
 api 
features

## How to Build

The generated code has dependencies over external libraries like UniRest. These dependencies are defined in the ```composer.json``` file that comes with the SDK. 
To resolve these dependencies, we use the Composer package manager which requires PHP greater than 5.3.2 installed in your system. 
Visit [https://getcomposer.org/download/](https://getcomposer.org/download/) to download the installer file for Composer and run it in your system. 
Open command prompt and type ```composer --version```. This should display the current version of the Composer installed if the installation was successful.

* Using command line, navigate to the directory containing the generated files (including ```composer.json```) for the SDK. 
* Run the command ```composer install```. This should install all the required dependencies and create the ```vendor``` directory in your project directory.

![Building SDK - Step 1](https://apidocs.io/illustration/php?step=installDependencies&workspaceFolder=Tester-PHP)

### [For Windows Users Only] Configuring CURL Certificate Path in php.ini

CURL used to include a list of accepted CAs, but no longer bundles ANY CA certs. So by default it will reject all SSL certificates as unverifiable. You will have to get your CA's cert and point curl at it. The steps are as follows:

1. Download the certificate bundle (.pem file) from [https://curl.haxx.se/docs/caextract.html](https://curl.haxx.se/docs/caextract.html) on to your system.
2. Add curl.cainfo = "PATH_TO/cacert.pem" to your php.ini file located in your php installation. “PATH_TO” must be an absolute path containing the .pem file.

```ini
[curl]
; A default value for the CURLOPT_CAINFO option. This is required to be an
; absolute path.
;curl.cainfo =
```

## How to Use

The following section explains how to use the Tester library in a new project.

### 1. Open Project in an IDE

Open an IDE for PHP like PhpStorm. The basic workflow presented here is also applicable if you prefer using a different editor or IDE.

![Open project in PHPStorm - Step 1](https://apidocs.io/illustration/php?step=openIDE&workspaceFolder=Tester-PHP)

Click on ```Open``` in PhpStorm to browse to your generated SDK directory and then click ```OK```.

![Open project in PHPStorm - Step 2](https://apidocs.io/illustration/php?step=openProject0&workspaceFolder=Tester-PHP)     

### 2. Add a new Test Project

Create a new directory by right clicking on the solution name as shown below:

![Add a new project in PHPStorm - Step 1](https://apidocs.io/illustration/php?step=createDirectory&workspaceFolder=Tester-PHP)

Name the directory as "test"

![Add a new project in PHPStorm - Step 2](https://apidocs.io/illustration/php?step=nameDirectory&workspaceFolder=Tester-PHP)
   
Add a PHP file to this project

![Add a new project in PHPStorm - Step 3](https://apidocs.io/illustration/php?step=createFile&workspaceFolder=Tester-PHP)

Name it "testSDK"

![Add a new project in PHPStorm - Step 4](https://apidocs.io/illustration/php?step=nameFile&workspaceFolder=Tester-PHP)

Depending on your project setup, you might need to include composer's autoloader in your PHP code to enable auto loading of classes.

```PHP
require_once "../vendor/autoload.php";
```

It is important that the path inside require_once correctly points to the file ```autoload.php``` inside the vendor directory created during dependency installations.

![Add a new project in PHPStorm - Step 4](https://apidocs.io/illustration/php?step=projectFiles&workspaceFolder=Tester-PHP)

After this you can add code to initialize the client library and acquire the instance of a Controller class. Sample code to initialize the client library and using controller methods is given in the subsequent sections.

### 3. Run the Test Project

To run your project you must set the Interpreter for your project. Interpreter is the PHP engine installed on your computer.

Open ```Settings``` from ```File``` menu.

![Run Test Project - Step 1](https://apidocs.io/illustration/php?step=openSettings&workspaceFolder=Tester-PHP)

Select ```PHP``` from within ```Languages & Frameworks```

![Run Test Project - Step 2](https://apidocs.io/illustration/php?step=setInterpreter0&workspaceFolder=Tester-PHP)

Browse for Interpreters near the ```Interpreter``` option and choose your interpreter.

![Run Test Project - Step 3](https://apidocs.io/illustration/php?step=setInterpreter1&workspaceFolder=Tester-PHP)

Once the interpreter is selected, click ```OK```

![Run Test Project - Step 4](https://apidocs.io/illustration/php?step=setInterpreter2&workspaceFolder=Tester-PHP)

To run your project, right click on your PHP file inside your Test project and click on ```Run```

![Run Test Project - Step 5](https://apidocs.io/illustration/php?step=runProject&workspaceFolder=Tester-PHP)

## How to Test

Unit tests in this SDK can be run using PHPUnit. 

1. First install the dependencies using composer including the `require-dev` dependencies.
2. Run `vendor\bin\phpunit --verbose` from commandline to execute tests. If you have 
   installed PHPUnit globally, run tests using `phpunit --verbose` instead.

You can change the PHPUnit test configuration in the `phpunit.xml` file.

## Initialization

### 

API client can be initialized as following.

```php

$client = new TesterLib\TesterClient();
```


# Class Reference

## <a name="list_of_controllers"></a>List of Controllers

* [ResponseTypesController](#response_types_controller)
* [BodyParamsController](#body_params_controller)
* [FormParamsController](#form_params_controller)
* [QueryParamController](#query_param_controller)
* [ErrorCodesController](#error_codes_controller)
* [MEchoController](#m_echo_controller)
* [HeaderController](#header_controller)
* [TemplateParamsController](#template_params_controller)

## <a name="response_types_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ResponseTypesController") ResponseTypesController

### Get singleton instance

The singleton instance of the ``` ResponseTypesController ``` class can be accessed from the API Client.

```php
$responseTypes = $client->getResponseTypes();
```

### <a name="get_date_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getDateArray") getDateArray

> TODO: Add a method description


```php
function getDateArray()
```

#### Example Usage

```php

$result = $responseTypes->getDateArray();

```


### <a name="get_date"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getDate") getDate

> TODO: Add a method description


```php
function getDate()
```

#### Example Usage

```php

$result = $responseTypes->getDate();

```


### <a name="get_long"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getLong") getLong

> TODO: Add a method description


```php
function getLong()
```

#### Example Usage

```php

$result = $responseTypes->getLong();

```


### <a name="get_model"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getModel") getModel

> TODO: Add a method description


```php
function getModel()
```

#### Example Usage

```php

$result = $responseTypes->getModel();

```


### <a name="get_string_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getStringEnumArray") getStringEnumArray

> TODO: Add a method description


```php
function getStringEnumArray()
```

#### Example Usage

```php

$result = $responseTypes->getStringEnumArray();

```


### <a name="get_string_enum"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getStringEnum") getStringEnum

> TODO: Add a method description


```php
function getStringEnum()
```

#### Example Usage

```php

$result = $responseTypes->getStringEnum();

```


### <a name="get_model_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getModelArray") getModelArray

> TODO: Add a method description


```php
function getModelArray()
```

#### Example Usage

```php

$result = $responseTypes->getModelArray();

```


### <a name="get_int_enum"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getIntEnum") getIntEnum

> TODO: Add a method description


```php
function getIntEnum()
```

#### Example Usage

```php

$result = $responseTypes->getIntEnum();

```


### <a name="get_int_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getIntEnumArray") getIntEnumArray

> TODO: Add a method description


```php
function getIntEnumArray()
```

#### Example Usage

```php

$result = $responseTypes->getIntEnumArray();

```


### <a name="get_precision"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getPrecision") getPrecision

> TODO: Add a method description


```php
function getPrecision()
```

#### Example Usage

```php

$result = $responseTypes->getPrecision();

```


### <a name="get_binary"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getBinary") getBinary

> gets a binary object


```php
function getBinary()
```

#### Example Usage

```php

$result = $responseTypes->getBinary();

```


### <a name="get_integer"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getInteger") getInteger

> Gets a integer response


```php
function getInteger()
```

#### Example Usage

```php

$result = $responseTypes->getInteger();

```


### <a name="get_integer_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getIntegerArray") getIntegerArray

> Get an array of integers.


```php
function getIntegerArray()
```

#### Example Usage

```php

$result = $responseTypes->getIntegerArray();

```


### <a name="get_dynamic"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getDynamic") getDynamic

> TODO: Add a method description


```php
function getDynamic()
```

#### Example Usage

```php

$result = $responseTypes->getDynamic();

```


### <a name="get_dynamic_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getDynamicArray") getDynamicArray

> TODO: Add a method description


```php
function getDynamicArray()
```

#### Example Usage

```php

$result = $responseTypes->getDynamicArray();

```


### <a name="get3339_datetime"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get3339Datetime") get3339Datetime

> TODO: Add a method description


```php
function get3339Datetime()
```

#### Example Usage

```php

$result = $responseTypes->get3339Datetime();

```


### <a name="get3339_datetime_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get3339DatetimeArray") get3339DatetimeArray

> TODO: Add a method description


```php
function get3339DatetimeArray()
```

#### Example Usage

```php

$result = $responseTypes->get3339DatetimeArray();

```


### <a name="get_boolean"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getBoolean") getBoolean

> TODO: Add a method description


```php
function getBoolean()
```

#### Example Usage

```php

$result = $responseTypes->getBoolean();

```


### <a name="get_boolean_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getBooleanArray") getBooleanArray

> TODO: Add a method description


```php
function getBooleanArray()
```

#### Example Usage

```php

$result = $responseTypes->getBooleanArray();

```


### <a name="get_headers"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getHeaders") getHeaders

> TODO: Add a method description


```php
function getHeaders()
```

#### Example Usage

```php

$responseTypes->getHeaders();

```


### <a name="get1123_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get1123DateTime") get1123DateTime

> TODO: Add a method description


```php
function get1123DateTime()
```

#### Example Usage

```php

$result = $responseTypes->get1123DateTime();

```


### <a name="get_unix_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getUnixDateTime") getUnixDateTime

> TODO: Add a method description


```php
function getUnixDateTime()
```

#### Example Usage

```php

$result = $responseTypes->getUnixDateTime();

```


### <a name="get1123_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get1123DateTimeArray") get1123DateTimeArray

> TODO: Add a method description


```php
function get1123DateTimeArray()
```

#### Example Usage

```php

$result = $responseTypes->get1123DateTimeArray();

```


### <a name="get_unix_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getUnixDateTimeArray") getUnixDateTimeArray

> TODO: Add a method description


```php
function getUnixDateTimeArray()
```

#### Example Usage

```php

$result = $responseTypes->getUnixDateTimeArray();

```


[Back to List of Controllers](#list_of_controllers)

## <a name="body_params_controller"></a>![Class: ](https://apidocs.io/img/class.png ".BodyParamsController") BodyParamsController

### Get singleton instance

The singleton instance of the ``` BodyParamsController ``` class can be accessed from the API Client.

```php
$bodyParams = $client->getBodyParams();
```

### <a name="send_date_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendDateArray") sendDateArray

> TODO: Add a method description


```php
function sendDateArray($dates)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dates |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$datesValue = "["1994-02-13", "1994-02-13"]";
$dates = APIHelper::deserialize($datesValue);

$result = $bodyParams->sendDateArray($dates);

```


### <a name="send_date"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendDate") sendDate

> TODO: Add a method description


```php
function sendDate($date)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| date |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$date = 1994-02-13;

$result = $bodyParams->sendDate($date);

```


### <a name="send_unix_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendUnixDateTime") sendUnixDateTime

> TODO: Add a method description


```php
function sendUnixDateTime($datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$datetime = 1484719381;

$result = $bodyParams->sendUnixDateTime($datetime);

```


### <a name="send_rfc1123_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendRfc1123DateTime") sendRfc1123DateTime

> TODO: Add a method description


```php
function sendRfc1123DateTime($datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$datetime = Sun, 06 Nov 1994 08:49:37 GMT;

$result = $bodyParams->sendRfc1123DateTime($datetime);

```


### <a name="send_rfc3339_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendRfc3339DateTime") sendRfc3339DateTime

> TODO: Add a method description


```php
function sendRfc3339DateTime($datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$datetime = 1994-02-13T14:01:54.9571247Z;

$result = $bodyParams->sendRfc3339DateTime($datetime);

```


### <a name="send_unix_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendUnixDateTimeArray") sendUnixDateTimeArray

> TODO: Add a method description


```php
function sendUnixDateTimeArray($datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$datetimesValue = "[1484719381,1484719381]";
$datetimes = APIHelper::deserialize($datetimesValue);

$result = $bodyParams->sendUnixDateTimeArray($datetimes);

```


### <a name="send_rfc1123_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendRfc1123DateTimeArray") sendRfc1123DateTimeArray

> TODO: Add a method description


```php
function sendRfc1123DateTimeArray($datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$datetimesValue = "["Sun, 06 Nov 1994 08:49:37 GMT","Sun, 06 Nov 1994 08:49:37 GMT"]";
$datetimes = APIHelper::deserialize($datetimesValue);

$result = $bodyParams->sendRfc1123DateTimeArray($datetimes);

```


### <a name="send_rfc3339_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendRfc3339DateTimeArray") sendRfc3339DateTimeArray

> TODO: Add a method description


```php
function sendRfc3339DateTimeArray($datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$datetimesValue = "["1994-02-13T14:01:54.9571247Z","1994-02-13T14:01:54.9571247Z"]";
$datetimes = APIHelper::deserialize($datetimesValue);

$result = $bodyParams->sendRfc3339DateTimeArray($datetimes);

```


### <a name="send_string_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendStringArray") sendStringArray

> sends a string body param


```php
function sendStringArray($sarray)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| sarray |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$sarrayValue = "["abc", "def"]";
$sarray = APIHelper::deserialize($sarrayValue);

$result = $bodyParams->sendStringArray($sarray);

```


### <a name="send_integer_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendIntegerArray") sendIntegerArray

> TODO: Add a method description


```php
function sendIntegerArray($integers)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$integersValue = "[1,2,3,4,5]";
$integers = APIHelper::deserialize($integersValue);

$result = $bodyParams->sendIntegerArray($integers);

```


### <a name="send_model"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendModel") sendModel

> TODO: Add a method description


```php
function sendModel($model)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| model |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$modelValue = "{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}";
$model = APIHelper::deserialize($modelValue);

$result = $bodyParams->sendModel($model);

```


### <a name="send_model_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendModelArray") sendModelArray

> TODO: Add a method description


```php
function sendModelArray($models)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| models |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$modelsValue = "[{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"},{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}]";
$models = APIHelper::deserialize($modelsValue);

$result = $bodyParams->sendModelArray($models);

```


### <a name="send_dynamic"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendDynamic") sendDynamic

> TODO: Add a method description


```php
function sendDynamic($dynamic)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dynamic |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$dynamic = APIHelper::deserialize("{\"uid\": \"1123213\", \"name\": \"Shahid\"}");

$result = $bodyParams->sendDynamic($dynamic);

```


### <a name="send_string"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendString") sendString

> TODO: Add a method description


```php
function sendString($value)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| value |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$value = 'TestString';

$result = $bodyParams->sendString($value);

```


### <a name="send_string_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendStringEnumArray") sendStringEnumArray

> TODO: Add a method description


```php
function sendStringEnumArray($days)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| days |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$days = array(Days::TUESDAY,Days::SATURDAY,Days::MONDAY,Days::SUNDAY);

$result = $bodyParams->sendStringEnumArray($days);

```


### <a name="send_integer_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendIntegerEnumArray") sendIntegerEnumArray

> TODO: Add a method description


```php
function sendIntegerEnumArray($suites)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| suites |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$suites = array(SuiteCode::HEARTS,SuiteCode::CLUBS,SuiteCode::DIAMONDS,SuiteCode::SPADES,SuiteCode::CLUBS);

$result = $bodyParams->sendIntegerEnumArray($suites);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="form_params_controller"></a>![Class: ](https://apidocs.io/img/class.png ".FormParamsController") FormParamsController

### Get singleton instance

The singleton instance of the ``` FormParamsController ``` class can be accessed from the API Client.

```php
$formParams = $client->getFormParams();
```

### <a name="send_date_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendDateArray") sendDateArray

> TODO: Add a method description


```php
function sendDateArray($dates)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dates |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$datesValue = "["1994-02-13","1994-02-13"]";
$dates = APIHelper::deserialize($datesValue);

$result = $formParams->sendDateArray($dates);

```


### <a name="send_date"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendDate") sendDate

> TODO: Add a method description


```php
function sendDate($date)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| date |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$date = 1994-02-13;

$result = $formParams->sendDate($date);

```


### <a name="send_unix_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendUnixDateTime") sendUnixDateTime

> TODO: Add a method description


```php
function sendUnixDateTime($datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$datetime = 1484719381;

$result = $formParams->sendUnixDateTime($datetime);

```


### <a name="send_rfc1123_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendRfc1123DateTime") sendRfc1123DateTime

> TODO: Add a method description


```php
function sendRfc1123DateTime($datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$datetime = Sun, 06 Nov 1994 08:49:37 GMT;

$result = $formParams->sendRfc1123DateTime($datetime);

```


### <a name="send_rfc3339_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendRfc3339DateTime") sendRfc3339DateTime

> TODO: Add a method description


```php
function sendRfc3339DateTime($datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$datetime = 1994-02-13T14:01:54.9571247Z;

$result = $formParams->sendRfc3339DateTime($datetime);

```


### <a name="send_unix_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendUnixDateTimeArray") sendUnixDateTimeArray

> TODO: Add a method description


```php
function sendUnixDateTimeArray($datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$datetimesValue = "[1484719381,1484719381]";
$datetimes = APIHelper::deserialize($datetimesValue);

$result = $formParams->sendUnixDateTimeArray($datetimes);

```


### <a name="send_rfc1123_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendRfc1123DateTimeArray") sendRfc1123DateTimeArray

> TODO: Add a method description


```php
function sendRfc1123DateTimeArray($datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$datetimesValue = "["Sun, 06 Nov 1994 08:49:37 GMT","Sun, 06 Nov 1994 08:49:37 GMT"]";
$datetimes = APIHelper::deserialize($datetimesValue);

$result = $formParams->sendRfc1123DateTimeArray($datetimes);

```


### <a name="send_long"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendLong") sendLong

> TODO: Add a method description


```php
function sendLong($value)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| value |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$value = 5147483647;

$result = $formParams->sendLong($value);

```


### <a name="send_integer_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendIntegerArray") sendIntegerArray

> TODO: Add a method description


```php
function sendIntegerArray($integers)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$integersValue = "[1,2,3,4,5]";
$integers = APIHelper::deserialize($integersValue);

$result = $formParams->sendIntegerArray($integers);

```


### <a name="send_string_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendStringArray") sendStringArray

> TODO: Add a method description


```php
function sendStringArray($strings)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$stringsValue = "["abc", "def"]";
$strings = APIHelper::deserialize($stringsValue);

$result = $formParams->sendStringArray($strings);

```


### <a name="send_model"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendModel") sendModel

> TODO: Add a method description


```php
function sendModel($model)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| model |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$modelValue = "{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}";
$model = APIHelper::deserialize($modelValue);

$result = $formParams->sendModel($model);

```


### <a name="send_model_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendModelArray") sendModelArray

> TODO: Add a method description


```php
function sendModelArray($models)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| models |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$modelsValue = "[{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"},{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}]";
$models = APIHelper::deserialize($modelsValue);

$result = $formParams->sendModelArray($models);

```


### <a name="send_file"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendFile") sendFile

> TODO: Add a method description


```php
function sendFile($file)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$file = "PathToFile";

$result = $formParams->sendFile($file);

```


### <a name="send_string"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendString") sendString

> TODO: Add a method description


```php
function sendString($value)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| value |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$value = 'TestString';

$result = $formParams->sendString($value);

```


### <a name="send_rfc3339_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendRfc3339DateTimeArray") sendRfc3339DateTimeArray

> TODO: Add a method description


```php
function sendRfc3339DateTimeArray($datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$datetimesValue = "["1994-02-13T14:01:54.9571247Z","1994-02-13T14:01:54.9571247Z"]";
$datetimes = APIHelper::deserialize($datetimesValue);

$result = $formParams->sendRfc3339DateTimeArray($datetimes);

```


### <a name="send_mixed_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendMixedArray") sendMixedArray

> Send a variety for form params. Returns file count and body params


```php
function sendMixedArray($options)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | TODO: Add a parameter description |
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |
| models |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$file = "PathToFile";
$collect['file'] = $file;

$integersValue = "[1,2,3,4,5]";
$integers = APIHelper::deserialize($integersValue);
$collect['integers'] = $integers;

$modelsValue = "[{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"},{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}]";
$models = APIHelper::deserialize($modelsValue);
$collect['models'] = $models;

$stringsValue = "["abc", "def"]";
$strings = APIHelper::deserialize($stringsValue);
$collect['strings'] = $strings;


$result = $formParams->sendMixedArray($collect);

```


### <a name="send_integer_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendIntegerEnumArray") sendIntegerEnumArray

> TODO: Add a method description


```php
function sendIntegerEnumArray($suites)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| suites |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$suites = array(SuiteCode::HEARTS,SuiteCode::CLUBS,SuiteCode::DIAMONDS,SuiteCode::SPADES,SuiteCode::CLUBS);

$result = $formParams->sendIntegerEnumArray($suites);

```


### <a name="send_string_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendStringEnumArray") sendStringEnumArray

> TODO: Add a method description


```php
function sendStringEnumArray($days)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| days |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$days = array(Days::TUESDAY,Days::SATURDAY,Days::MONDAY,Days::SUNDAY);

$result = $formParams->sendStringEnumArray($days);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="query_param_controller"></a>![Class: ](https://apidocs.io/img/class.png ".QueryParamController") QueryParamController

### Get singleton instance

The singleton instance of the ``` QueryParamController ``` class can be accessed from the API Client.

```php
$queryParam = $client->getQueryParam();
```

### <a name="date_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.dateArray") dateArray

> TODO: Add a method description


```php
function dateArray($dates)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dates |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$datesValue = "["1994-02-13","1994-02-13"]";
$dates = APIHelper::deserialize($datesValue);

$result = $queryParam->dateArray($dates);

```


### <a name="date"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.date") date

> TODO: Add a method description


```php
function date($date)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| date |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$date = 1994-02-13;

$result = $queryParam->date($date);

```


### <a name="unix_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.unixDateTimeArray") unixDateTimeArray

> TODO: Add a method description


```php
function unixDateTimeArray($datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$datetimesValue = "[1484719381,1484719381]";
$datetimes = APIHelper::deserialize($datetimesValue);

$result = $queryParam->unixDateTimeArray($datetimes);

```


### <a name="unix_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.unixDateTime") unixDateTime

> TODO: Add a method description


```php
function unixDateTime($datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$datetime = 1484719381;

$result = $queryParam->unixDateTime($datetime);

```


### <a name="rfc1123_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.rfc1123DateTime") rfc1123DateTime

> TODO: Add a method description


```php
function rfc1123DateTime($datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$datetime = Sun, 06 Nov 1994 08:49:37 GMT;

$result = $queryParam->rfc1123DateTime($datetime);

```


### <a name="rfc1123_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.rfc1123DateTimeArray") rfc1123DateTimeArray

> TODO: Add a method description


```php
function rfc1123DateTimeArray($datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$datetimesValue = "["Sun, 06 Nov 1994 08:49:37 GMT","Sun, 06 Nov 1994 08:49:37 GMT"]";
$datetimes = APIHelper::deserialize($datetimesValue);

$result = $queryParam->rfc1123DateTimeArray($datetimes);

```


### <a name="rfc3339_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.rfc3339DateTimeArray") rfc3339DateTimeArray

> TODO: Add a method description


```php
function rfc3339DateTimeArray($datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$datetimesValue = "["1994-02-13T14:01:54.9571247Z","1994-02-13T14:01:54.9571247Z"]";
$datetimes = APIHelper::deserialize($datetimesValue);

$result = $queryParam->rfc3339DateTimeArray($datetimes);

```


### <a name="rfc3339_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.rfc3339DateTime") rfc3339DateTime

> TODO: Add a method description


```php
function rfc3339DateTime($datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$datetime = 1994-02-13T14:01:54.9571247Z;

$result = $queryParam->rfc3339DateTime($datetime);

```


### <a name="no_params"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.noParams") noParams

> TODO: Add a method description


```php
function noParams()
```

#### Example Usage

```php

$result = $queryParam->noParams();

```


### <a name="string_param"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.stringParam") stringParam

> TODO: Add a method description


```php
function stringParam($string)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| string |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$string = 'l;asd;asdwe[2304&&;\'.d??\\a\\\\\\;sd//';

$result = $queryParam->stringParam($string);

```


### <a name="url_param"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.urlParam") urlParam

> TODO: Add a method description


```php
function urlParam($url)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| url |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$url = 'https://www.shahidisawesome.com/and/also/a/narcissist?thisis=aparameter&another=one';

$result = $queryParam->urlParam($url);

```


### <a name="number_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.numberArray") numberArray

> TODO: Add a method description


```php
function numberArray($integers)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$integersValue = "[1,2,3,4,5]";
$integers = APIHelper::deserialize($integersValue);

$result = $queryParam->numberArray($integers);

```


### <a name="string_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.stringArray") stringArray

> TODO: Add a method description


```php
function stringArray($strings)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$stringsValue = "["abc", "def"]";
$strings = APIHelper::deserialize($stringsValue);

$result = $queryParam->stringArray($strings);

```


### <a name="simple_query"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.simpleQuery") simpleQuery

> TODO: Add a method description


```php
function simpleQuery(
        $boolean,
        $number,
        $string,
        $queryParameters = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| boolean |  ``` Required ```  | TODO: Add a parameter description |
| number |  ``` Required ```  | TODO: Add a parameter description |
| string |  ``` Required ```  | TODO: Add a parameter description |
| queryParameters | ``` Optional ``` | Additional optional query parameters are supported by this method |



#### Example Usage

```php
$boolean = true;
$number = 4;
$string = 'TestString';
// key-value map for optional query parameters
$queryParams = array('key' => 'value');


$result = $queryParam->simpleQuery($boolean, $number, $string, $queryParams);

```


### <a name="string_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.stringEnumArray") stringEnumArray

> TODO: Add a method description


```php
function stringEnumArray($days)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| days |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$days = array(Days::TUESDAY,Days::SATURDAY,Days::MONDAY,Days::SUNDAY);

$result = $queryParam->stringEnumArray($days);

```


### <a name="multiple_params"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.multipleParams") multipleParams

> TODO: Add a method description


```php
function multipleParams(
        $number,
        $precision,
        $string,
        $url)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| number |  ``` Required ```  | TODO: Add a parameter description |
| precision |  ``` Required ```  | TODO: Add a parameter description |
| string |  ``` Required ```  | TODO: Add a parameter description |
| url |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$number = 123412312;
$precision = 1112.34;
$string = '""test./;";12&&3asl"";"qw1&34"///..//.';
$url = 'http://www.abc.com/test?a=b&c="http://lolol.com?param=no&another=lol"';

$result = $queryParam->multipleParams($number, $precision, $string, $url);

```


### <a name="integer_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.integerEnumArray") integerEnumArray

> TODO: Add a method description


```php
function integerEnumArray($suites)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| suites |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$suites = array(SuiteCode::HEARTS,SuiteCode::CLUBS,SuiteCode::DIAMONDS,SuiteCode::SPADES,SuiteCode::CLUBS);

$result = $queryParam->integerEnumArray($suites);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="error_codes_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ErrorCodesController") ErrorCodesController

### Get singleton instance

The singleton instance of the ``` ErrorCodesController ``` class can be accessed from the API Client.

```php
$errorCodes = $client->getErrorCodes();
```

### <a name="get400"></a>![Method: ](https://apidocs.io/img/method.png ".ErrorCodesController.get400") get400

> TODO: Add a method description


```php
function get400()
```

#### Example Usage

```php

$result = $errorCodes->get400();

```


### <a name="get500"></a>![Method: ](https://apidocs.io/img/method.png ".ErrorCodesController.get500") get500

> TODO: Add a method description


```php
function get500()
```

#### Example Usage

```php

$result = $errorCodes->get500();

```


### <a name="get401"></a>![Method: ](https://apidocs.io/img/method.png ".ErrorCodesController.get401") get401

> TODO: Add a method description


```php
function get401()
```

#### Example Usage

```php

$result = $errorCodes->get401();

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 401 | 401 Local |
| 421 | Default |
| 431 | Default |
| 432 | Default |
| 441 | Default |
| 0 | Invalid response. |



[Back to List of Controllers](#list_of_controllers)

## <a name="m_echo_controller"></a>![Class: ](https://apidocs.io/img/class.png ".MEchoController") MEchoController

### Get singleton instance

The singleton instance of the ``` MEchoController ``` class can be accessed from the API Client.

```php
$mEcho = $client->getMEcho();
```

### <a name="json_echo"></a>![Method: ](https://apidocs.io/img/method.png ".MEchoController.jsonEcho") jsonEcho

> Echo's back the request


```php
function jsonEcho($input)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| input |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$input = APIHelper::deserialize("{\"uid\": \"1123213\", \"name\": \"Shahid\"}");

$result = $mEcho->jsonEcho($input);

```


### <a name="form_echo"></a>![Method: ](https://apidocs.io/img/method.png ".MEchoController.formEcho") formEcho

> Sends the request including any form params as JSON


```php
function formEcho($input)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| input |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```php
$input = APIHelper::deserialize("{\"uid\": \"1123213\", \"name\": \"Shahid\"}");

$result = $mEcho->formEcho($input);

```


### <a name="query_echo"></a>![Method: ](https://apidocs.io/img/method.png ".MEchoController.queryEcho") queryEcho

> TODO: Add a method description


```php
function queryEcho($queryParameters = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| queryParameters | ``` Optional ``` | Additional optional query parameters are supported by this method |



#### Example Usage

```php
// key-value map for optional query parameters
$queryParams = array('key' => 'value');


$result = $mEcho->queryEcho($queryParams);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="header_controller"></a>![Class: ](https://apidocs.io/img/class.png ".HeaderController") HeaderController

### Get singleton instance

The singleton instance of the ``` HeaderController ``` class can be accessed from the API Client.

```php
$header = $client->getHeader();
```

### <a name="send_headers"></a>![Method: ](https://apidocs.io/img/method.png ".HeaderController.sendHeaders") sendHeaders

> Sends a single header params


```php
function sendHeaders(
        $customHeader,
        $value)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| customHeader |  ``` Required ```  | TODO: Add a parameter description |
| value |  ``` Required ```  | Represents the value of the custom header |



#### Example Usage

```php
$customHeader = 'TestString';
$value = 'TestString';

$result = $header->sendHeaders($customHeader, $value);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="template_params_controller"></a>![Class: ](https://apidocs.io/img/class.png ".TemplateParamsController") TemplateParamsController

### Get singleton instance

The singleton instance of the ``` TemplateParamsController ``` class can be accessed from the API Client.

```php
$templateParams = $client->getTemplateParams();
```

### <a name="send_string_array"></a>![Method: ](https://apidocs.io/img/method.png ".TemplateParamsController.sendStringArray") sendStringArray

> TODO: Add a method description


```php
function sendStringArray($strings)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$stringsValue = "["abc", "def"]";
$strings = APIHelper::deserialize($stringsValue);

$result = $templateParams->sendStringArray($strings);

```


### <a name="send_integer_array"></a>![Method: ](https://apidocs.io/img/method.png ".TemplateParamsController.sendIntegerArray") sendIntegerArray

> TODO: Add a method description


```php
function sendIntegerArray($integers)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```php
$integersValue = "[1,2,3,4,5]";
$integers = APIHelper::deserialize($integersValue);

$result = $templateParams->sendIntegerArray($integers);

```


[Back to List of Controllers](#list_of_controllers)



