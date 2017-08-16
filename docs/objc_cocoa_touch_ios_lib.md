# Getting started

Testing various
 api 
features

## How to Build


The generated code has dependencies over external libraries like UniRest. These dependencies are defined in the ```PodFile``` file that comes with the SDK. 
To resolve these dependencies, we use the Cocoapods package manager.
Visit https://guides.cocoapods.org/using/getting-started.html to setup Cocoapods on your system.
Open command prompt and type ```pod --version```. This should display the current version of Cocoapods installed if the installation was successful.

Using command line, navigate to the directory containing the generated files (including ```PodFile```) for the SDK. 
Run the command ```pod install```. This should install all the required dependencies and create the ```pods``` directory in your project directory.

![Installing dependencies using Cocoapods](https://apidocs.io/illustration/objc?step=AddDependencies&workspaceFolder=Tester-ObjC&workspaceName=Tester&projectName=Tester&rootNamespace=Tester)

Open the project workspace using the (Tester.xcworkspace) file. Invoke the build process using `Command(⌘)+B` shortcut key or using the `Build` menu as shown below.

![Building SDK using Xcode](https://apidocs.io/illustration/objc?step=BuildSDK&workspaceFolder=Tester-ObjC&workspaceName=Tester&projectName=Tester&rootNamespace=Tester)


## How to Use

The generated code is a Cocoa Touch Static Library which can be used in any iOS project. The support for these generated libraries go all the way back to iOS 6.

The following section explains how to use the Tester library in a new iOS project.     
### 1. Starting a new project
To start a new project, left-click on the ```Create a new Xcode project```.
![Create Test Project - Step 1](https://apidocs.io/illustration/objc?step=Test1&workspaceFolder=Tester-ObjC&workspaceName=Tester&projectName=Tester&rootNamespace=Tester)

Next, choose **Single View Application** and click ```Next```.
![Create Test Project - Step 2](https://apidocs.io/illustration/objc?step=Test2&workspaceFolder=Tester-ObjC&workspaceName=Tester&projectName=Tester&rootNamespace=Tester)

Provide **Test-Project** as the product name click ```Next```.
![Create Test Project - Step 3](https://apidocs.io/illustration/objc?step=Test3&workspaceFolder=Tester-ObjC&workspaceName=Tester&projectName=Tester&rootNamespace=Tester)

Choose the desired location of your project folder and click ```Create```.
![Create Test Project - Step 4](https://apidocs.io/illustration/objc?step=Test4&workspaceFolder=Tester-ObjC&workspaceName=Tester&projectName=Tester&rootNamespace=Tester)

### 2. Adding the static library dependency
To add this dependency open a terminal and navigate to your project folder. Next, input ```pod init``` and press enter.
![Add dependency - Step 1](https://apidocs.io/illustration/objc?step=Add0&workspaceFolder=Tester-ObjC&workspaceName=Tester&projectName=Tester&rootNamespace=Tester)

Next, open the newly created ```PodFile``` in your favourite text editor. Add the following line : pod 'Tester', :path => 'Vendor/Tester'
![Add dependency - Step 2](https://apidocs.io/illustration/objc?step=Add1&workspaceFolder=Tester-ObjC&workspaceName=Tester&projectName=Tester&rootNamespace=Tester)

Execute `pod install` from terminal to install the dependecy in your project. This would add the dependency to the newly created test project.
![Add dependency - Step 3](https://apidocs.io/illustration/objc?step=Add2&workspaceFolder=Tester-ObjC&workspaceName=Tester&projectName=Tester&rootNamespace=Tester)


## How to Test

Unit tests in this SDK can be run using Xcode. 

First build the SDK as shown in the steps above and naivgate to the project directory and open the Tester.xcworkspace file.

Go to the test explorer in Xcode as shown in the picture below and click on `run tests` from the menu. 
![Run tests](https://apidocs.io/illustration/objc?step=RunTests&workspaceFolder=Tester-ObjC&workspaceName=Tester&projectName=Tester&rootNamespace=Tester)


## Initialization

### 
You need the following information for initializing the API client.

| Parameter | Description |
|-----------|-------------|
| suites | TODO: add a description |



Configuration variables can be set as following.
```Objc
// Configuration parameters
Configuration_Suites = "Configuration_Suites";

```

# Class Reference

## <a name="list_of_controllers"></a>List of Controllers

* [ResponseTypesController](#response_types_controller)
* [BodyParamsController](#body_params_controller)
* [FormParamsController](#form_params_controller)
* [QueryParamController](#query_param_controller)
* [ErrorCodesController](#error_codes_controller)
* [EchoController](#echo_controller)
* [HeaderController](#header_controller)
* [TemplateParamsController](#template_params_controller)

## <a name="response_types_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ResponseTypesController") ResponseTypesController

### Get singleton instance
```objc
ResponseTypes* responseTypes = [[ResponseTypes alloc]init] ;
```

### <a name="get_date_array_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getDateArrayWithCompletionBlock") getDateArrayWithCompletionBlock

> TODO: Add a method description


```objc
function getDateArrayWithCompletionBlock:(CompletedGetDateArray) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes getDateArrayWithCompletionBlock:  ^(BOOL success, HttpContext* context, NSArray* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_date_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getDateWithCompletionBlock") getDateWithCompletionBlock

> TODO: Add a method description


```objc
function getDateWithCompletionBlock:(CompletedGetDate) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes getDateWithCompletionBlock:  ^(BOOL success, HttpContext* context, NSDate* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_long_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getLongWithCompletionBlock") getLongWithCompletionBlock

> TODO: Add a method description


```objc
function getLongWithCompletionBlock:(CompletedGetLong) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes getLongWithCompletionBlock:  ^(BOOL success, HttpContext* context, NSNumber* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_model_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getModelWithCompletionBlock") getModelWithCompletionBlock

> TODO: Add a method description


```objc
function getModelWithCompletionBlock:(CompletedGetModel) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes getModelWithCompletionBlock:  ^(BOOL success, HttpContext* context, Person* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_string_enum_array_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getStringEnumArrayWithCompletionBlock") getStringEnumArrayWithCompletionBlock

> TODO: Add a method description


```objc
function getStringEnumArrayWithCompletionBlock:(CompletedGetStringEnumArray) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes getStringEnumArrayWithCompletionBlock:  ^(BOOL success, HttpContext* context, NSArray<NSNumber*>* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_string_enum_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getStringEnumWithCompletionBlock") getStringEnumWithCompletionBlock

> TODO: Add a method description


```objc
function getStringEnumWithCompletionBlock:(CompletedGetStringEnum) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes getStringEnumWithCompletionBlock:  ^(BOOL success, HttpContext* context, enum Days response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_model_array_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getModelArrayWithCompletionBlock") getModelArrayWithCompletionBlock

> TODO: Add a method description


```objc
function getModelArrayWithCompletionBlock:(CompletedGetModelArray) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes getModelArrayWithCompletionBlock:  ^(BOOL success, HttpContext* context, NSArray<Person> * response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_int_enum_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getIntEnumWithCompletionBlock") getIntEnumWithCompletionBlock

> TODO: Add a method description


```objc
function getIntEnumWithCompletionBlock:(CompletedGetIntEnum) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes getIntEnumWithCompletionBlock:  ^(BOOL success, HttpContext* context, enum SuiteCode response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_int_enum_array_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getIntEnumArrayWithCompletionBlock") getIntEnumArrayWithCompletionBlock

> TODO: Add a method description


```objc
function getIntEnumArrayWithCompletionBlock:(CompletedGetIntEnumArray) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes getIntEnumArrayWithCompletionBlock:  ^(BOOL success, HttpContext* context, NSArray<NSNumber*>* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_precision_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getPrecisionWithCompletionBlock") getPrecisionWithCompletionBlock

> TODO: Add a method description


```objc
function getPrecisionWithCompletionBlock:(CompletedGetPrecision) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes getPrecisionWithCompletionBlock:  ^(BOOL success, HttpContext* context, NSNumber* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_binary_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getBinaryWithCompletionBlock") getBinaryWithCompletionBlock

> gets a binary object


```objc
function getBinaryWithCompletionBlock:(CompletedGetBinary) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes getBinaryWithCompletionBlock:  ^(BOOL success, HttpContext* context, NSData* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_integer_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getIntegerWithCompletionBlock") getIntegerWithCompletionBlock

> Gets a integer response


```objc
function getIntegerWithCompletionBlock:(CompletedGetInteger) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes getIntegerWithCompletionBlock:  ^(BOOL success, HttpContext* context, NSNumber* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_integer_array_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getIntegerArrayWithCompletionBlock") getIntegerArrayWithCompletionBlock

> Get an array of integers.


```objc
function getIntegerArrayWithCompletionBlock:(CompletedGetIntegerArray) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes getIntegerArrayWithCompletionBlock:  ^(BOOL success, HttpContext* context, NSArray* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_dynamic_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getDynamicWithCompletionBlock") getDynamicWithCompletionBlock

> TODO: Add a method description


```objc
function getDynamicWithCompletionBlock:(CompletedGetDynamic) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes getDynamicWithCompletionBlock:  ^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_dynamic_array_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getDynamicArrayWithCompletionBlock") getDynamicArrayWithCompletionBlock

> TODO: Add a method description


```objc
function getDynamicArrayWithCompletionBlock:(CompletedGetDynamicArray) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes getDynamicArrayWithCompletionBlock:  ^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get3339_datetime_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get3339DatetimeWithCompletionBlock") get3339DatetimeWithCompletionBlock

> TODO: Add a method description


```objc
function get3339DatetimeWithCompletionBlock:(CompletedGet3339Datetime) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes get3339DatetimeWithCompletionBlock:  ^(BOOL success, HttpContext* context, NSDate* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get3339_datetime_array_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get3339DatetimeArrayWithCompletionBlock") get3339DatetimeArrayWithCompletionBlock

> TODO: Add a method description


```objc
function get3339DatetimeArrayWithCompletionBlock:(CompletedGet3339DatetimeArray) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes get3339DatetimeArrayWithCompletionBlock:  ^(BOOL success, HttpContext* context, NSArray* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_boolean_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getBooleanWithCompletionBlock") getBooleanWithCompletionBlock

> TODO: Add a method description


```objc
function getBooleanWithCompletionBlock:(CompletedGetBoolean) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes getBooleanWithCompletionBlock:  ^(BOOL success, HttpContext* context, NSNumber* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_boolean_array_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getBooleanArrayWithCompletionBlock") getBooleanArrayWithCompletionBlock

> TODO: Add a method description


```objc
function getBooleanArrayWithCompletionBlock:(CompletedGetBooleanArray) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes getBooleanArrayWithCompletionBlock:  ^(BOOL success, HttpContext* context, NSArray* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_headers_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getHeadersWithCompletionBlock") getHeadersWithCompletionBlock

> TODO: Add a method description


```objc
function getHeadersWithCompletionBlock:(CompletedGetHeaders) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes getHeadersWithCompletionBlock:  ^(BOOL success, HttpContext* context, NSError* error) { 
       //Add code here
    }];
```


### <a name="get1123_date_time_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get1123DateTimeWithCompletionBlock") get1123DateTimeWithCompletionBlock

> TODO: Add a method description


```objc
function get1123DateTimeWithCompletionBlock:(CompletedGet1123DateTime) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes get1123DateTimeWithCompletionBlock:  ^(BOOL success, HttpContext* context, NSDate* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_unix_date_time_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getUnixDateTimeWithCompletionBlock") getUnixDateTimeWithCompletionBlock

> TODO: Add a method description


```objc
function getUnixDateTimeWithCompletionBlock:(CompletedGetUnixDateTime) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes getUnixDateTimeWithCompletionBlock:  ^(BOOL success, HttpContext* context, NSDate* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get1123_date_time_array_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get1123DateTimeArrayWithCompletionBlock") get1123DateTimeArrayWithCompletionBlock

> TODO: Add a method description


```objc
function get1123DateTimeArrayWithCompletionBlock:(CompletedGet1123DateTimeArray) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes get1123DateTimeArrayWithCompletionBlock:  ^(BOOL success, HttpContext* context, NSArray* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get_unix_date_time_array_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.getUnixDateTimeArrayWithCompletionBlock") getUnixDateTimeArrayWithCompletionBlock

> TODO: Add a method description


```objc
function getUnixDateTimeArrayWithCompletionBlock:(CompletedGetUnixDateTimeArray) onCompleted()
```



#### Example Usage

```objc

    [self.responseTypes getUnixDateTimeArrayWithCompletionBlock:  ^(BOOL success, HttpContext* context, NSArray* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="body_params_controller"></a>![Class: ](https://apidocs.io/img/class.png ".BodyParamsController") BodyParamsController

### Get singleton instance
```objc
BodyParams* bodyParams = [[BodyParams alloc]init] ;
```

### <a name="send_date_array_async_with_dates"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendDateArrayAsyncWithDates") sendDateArrayAsyncWithDates

> TODO: Add a method description


```objc
function sendDateArrayAsyncWithDates:(NSArray*) dates
                completionBlock:(CompletedPostSendDateArray) onCompleted(dates)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dates |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* dates = (NSArray*) [APIHelper jsonDeserializeArray: @"[\"1994-02-13\", \"1994-02-13\"]"];

    [self.bodyParams sendDateArrayAsyncWithDates: dates  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_date_async_with_date"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendDateAsyncWithDate") sendDateAsyncWithDate

> TODO: Add a method description


```objc
function sendDateAsyncWithDate:(NSDate*) date
                completionBlock:(CompletedPostSendDate) onCompleted(date)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| date |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSDate* date = [NSDate NSDateFromNSString: @"1994-02-13"];

    [self.bodyParams sendDateAsyncWithDate: date  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_unix_date_time_async_with_datetime"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendUnixDateTimeAsyncWithDatetime") sendUnixDateTimeAsyncWithDatetime

> TODO: Add a method description


```objc
function sendUnixDateTimeAsyncWithDatetime:(NSDate*) datetime
                completionBlock:(CompletedPostSendUnixDateTime) onCompleted(datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSDate* datetime = [NSDate NSDateFromNSString: @"1484719381"];

    [self.bodyParams sendUnixDateTimeAsyncWithDatetime: datetime  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_rfc1123_date_time_async_with_datetime"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendRfc1123DateTimeAsyncWithDatetime") sendRfc1123DateTimeAsyncWithDatetime

> TODO: Add a method description


```objc
function sendRfc1123DateTimeAsyncWithDatetime:(NSDate*) datetime
                completionBlock:(CompletedPostSendRfc1123DateTime) onCompleted(datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSDate* datetime = [NSDate NSDateFromNSString: @"Sun, 06 Nov 1994 08:49:37 GMT"];

    [self.bodyParams sendRfc1123DateTimeAsyncWithDatetime: datetime  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_rfc3339_date_time_async_with_datetime"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendRfc3339DateTimeAsyncWithDatetime") sendRfc3339DateTimeAsyncWithDatetime

> TODO: Add a method description


```objc
function sendRfc3339DateTimeAsyncWithDatetime:(NSDate*) datetime
                completionBlock:(CompletedPostSendRfc3339DateTime) onCompleted(datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSDate* datetime = [NSDate NSDateFromNSString: @"1994-02-13T14:01:54.9571247Z"];

    [self.bodyParams sendRfc3339DateTimeAsyncWithDatetime: datetime  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_unix_date_time_array_async_with_datetimes"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendUnixDateTimeArrayAsyncWithDatetimes") sendUnixDateTimeArrayAsyncWithDatetimes

> TODO: Add a method description


```objc
function sendUnixDateTimeArrayAsyncWithDatetimes:(NSArray*) datetimes
                completionBlock:(CompletedPostSendUnixDateTimeArray) onCompleted(datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* datetimes = (NSArray*) [APIHelper jsonDeserializeArray: @"[1484719381,1484719381]"];

    [self.bodyParams sendUnixDateTimeArrayAsyncWithDatetimes: datetimes  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_rfc1123_date_time_array_async_with_datetimes"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendRfc1123DateTimeArrayAsyncWithDatetimes") sendRfc1123DateTimeArrayAsyncWithDatetimes

> TODO: Add a method description


```objc
function sendRfc1123DateTimeArrayAsyncWithDatetimes:(NSArray*) datetimes
                completionBlock:(CompletedPostSendRfc1123DateTimeArray) onCompleted(datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* datetimes = (NSArray*) [APIHelper jsonDeserializeArray: @"[\"Sun, 06 Nov 1994 08:49:37 GMT\",\"Sun, 06 Nov 1994 08:49:37 GMT\"]"];

    [self.bodyParams sendRfc1123DateTimeArrayAsyncWithDatetimes: datetimes  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_rfc3339_date_time_array_async_with_datetimes"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendRfc3339DateTimeArrayAsyncWithDatetimes") sendRfc3339DateTimeArrayAsyncWithDatetimes

> TODO: Add a method description


```objc
function sendRfc3339DateTimeArrayAsyncWithDatetimes:(NSArray*) datetimes
                completionBlock:(CompletedPostSendRfc3339DateTimeArray) onCompleted(datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* datetimes = (NSArray*) [APIHelper jsonDeserializeArray: @"[\"1994-02-13T14:01:54.9571247Z\",\"1994-02-13T14:01:54.9571247Z\"]"];

    [self.bodyParams sendRfc3339DateTimeArrayAsyncWithDatetimes: datetimes  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_string_array_async_with_sarray"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendStringArrayAsyncWithSarray") sendStringArrayAsyncWithSarray

> sends a string body param


```objc
function sendStringArrayAsyncWithSarray:(NSArray*) sarray
                completionBlock:(CompletedPostSendStringArray) onCompleted(sarray)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| sarray |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* sarray = (NSArray*) [APIHelper jsonDeserializeArray: @"[\"abc\", \"def\"]"];

    [self.bodyParams sendStringArrayAsyncWithSarray: sarray  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_integer_array_async_with_integers"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendIntegerArrayAsyncWithIntegers") sendIntegerArrayAsyncWithIntegers

> TODO: Add a method description


```objc
function sendIntegerArrayAsyncWithIntegers:(NSArray*) integers
                completionBlock:(CompletedPostSendIntegerArray) onCompleted(integers)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* integers = (NSArray*) [APIHelper jsonDeserializeArray: @"[1,2,3,4,5]"];

    [self.bodyParams sendIntegerArrayAsyncWithIntegers: integers  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_model_async_with_model"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendModelAsyncWithModel") sendModelAsyncWithModel

> TODO: Add a method description


```objc
function sendModelAsyncWithModel:(Employee*) model
                completionBlock:(CompletedPostSendModel) onCompleted(model)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| model |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    Employee* model = (Employee*) [APIHelper jsonDeserialize: @"{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}"
                toClass: Employee.class];

    [self.bodyParams sendModelAsyncWithModel: model  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_model_array_async_with_models"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendModelArrayAsyncWithModels") sendModelArrayAsyncWithModels

> TODO: Add a method description


```objc
function sendModelArrayAsyncWithModels:(NSArray<Employee> *) models
                completionBlock:(CompletedPostSendModelArray) onCompleted(models)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| models |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray<Employee> * models = (NSArray<Employee>*) [Employee arrayOfModelsFromDictionaries:
                [APIHelper jsonDeserializeArray: @"[{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"},{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}]"] error: nil];

    [self.bodyParams sendModelArrayAsyncWithModels: models  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_dynamic_async_with_dynamic"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendDynamicAsyncWithDynamic") sendDynamicAsyncWithDynamic

> TODO: Add a method description


```objc
function sendDynamicAsyncWithDynamic:(NSObject*) mdynamic
                completionBlock:(CompletedPostSendDynamic) onCompleted(mdynamic)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mdynamic |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSObject* mdynamic = [NSJSONSerialization
                        JSONObjectWithData: [@"{\"uid\": \"1123213\", \"name\": \"Shahid\"}" dataUsingEncoding: NSUTF8StringEncoding]
                                   options: NSJSONReadingAllowFragments
                                     error: nil];

    [self.bodyParams sendDynamicAsyncWithDynamic: mdynamic  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_string_async_with_value"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendStringAsyncWithValue") sendStringAsyncWithValue

> TODO: Add a method description


```objc
function sendStringAsyncWithValue:(NSString*) value
                completionBlock:(CompletedPostSendString) onCompleted(value)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| value |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* value = @"TestString";

    [self.bodyParams sendStringAsyncWithValue: value  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_string_enum_array_async_with_days"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendStringEnumArrayAsyncWithDays") sendStringEnumArrayAsyncWithDays

> TODO: Add a method description


```objc
function sendStringEnumArrayAsyncWithDays:(NSArray<NSNumber*>*) days
                completionBlock:(CompletedPostSendStringEnumArray) onCompleted(days)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| days |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray<NSNumber*>* days = [DaysHelper daysArrayFromStringArray:
                [APIHelper jsonDeserializeArray: @"[\"Tuesday\", \"Saturday\", \"Wednesday\", \"Monday\", \"Sunday\"]"]];

    [self.bodyParams sendStringEnumArrayAsyncWithDays: days  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_integer_enum_array_async_with_suites"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.sendIntegerEnumArrayAsyncWithSuites") sendIntegerEnumArrayAsyncWithSuites

> TODO: Add a method description


```objc
function sendIntegerEnumArrayAsyncWithSuites:(NSArray<NSNumber*>*) suites
                completionBlock:(CompletedPostSendIntegerEnumArray) onCompleted(suites)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| suites |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray<NSNumber*>* suites =  (NSArray<NSNumber*>*) [APIHelper jsonDeserializeArray: @"[1, 3, 4, 2, 3]"];

    [self.bodyParams sendIntegerEnumArrayAsyncWithSuites: suites  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="form_params_controller"></a>![Class: ](https://apidocs.io/img/class.png ".FormParamsController") FormParamsController

### Get singleton instance
```objc
FormParams* formParams = [[FormParams alloc]init] ;
```

### <a name="send_date_array_async_with_dates"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendDateArrayAsyncWithDates") sendDateArrayAsyncWithDates

> TODO: Add a method description


```objc
function sendDateArrayAsyncWithDates:(NSArray*) dates
                completionBlock:(CompletedPostSendDateArray) onCompleted(dates)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dates |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* dates = (NSArray*) [APIHelper jsonDeserializeArray: @"[\"1994-02-13\",\"1994-02-13\"]"];

    [self.formParams sendDateArrayAsyncWithDates: dates  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_date_async_with_date"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendDateAsyncWithDate") sendDateAsyncWithDate

> TODO: Add a method description


```objc
function sendDateAsyncWithDate:(NSDate*) date
                completionBlock:(CompletedPostSendDate) onCompleted(date)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| date |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSDate* date = [NSDate NSDateFromNSString: @"1994-02-13"];

    [self.formParams sendDateAsyncWithDate: date  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_unix_date_time_async_with_datetime"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendUnixDateTimeAsyncWithDatetime") sendUnixDateTimeAsyncWithDatetime

> TODO: Add a method description


```objc
function sendUnixDateTimeAsyncWithDatetime:(NSDate*) datetime
                completionBlock:(CompletedPostSendUnixDateTime) onCompleted(datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSDate* datetime = [NSDate NSDateFromNSString: @"1484719381"];

    [self.formParams sendUnixDateTimeAsyncWithDatetime: datetime  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_rfc1123_date_time_async_with_datetime"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendRfc1123DateTimeAsyncWithDatetime") sendRfc1123DateTimeAsyncWithDatetime

> TODO: Add a method description


```objc
function sendRfc1123DateTimeAsyncWithDatetime:(NSDate*) datetime
                completionBlock:(CompletedPostSendRfc1123DateTime) onCompleted(datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSDate* datetime = [NSDate NSDateFromNSString: @"Sun, 06 Nov 1994 08:49:37 GMT"];

    [self.formParams sendRfc1123DateTimeAsyncWithDatetime: datetime  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_rfc3339_date_time_async_with_datetime"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendRfc3339DateTimeAsyncWithDatetime") sendRfc3339DateTimeAsyncWithDatetime

> TODO: Add a method description


```objc
function sendRfc3339DateTimeAsyncWithDatetime:(NSDate*) datetime
                completionBlock:(CompletedPostSendRfc3339DateTime) onCompleted(datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSDate* datetime = [NSDate NSDateFromNSString: @"1994-02-13T14:01:54.9571247Z"];

    [self.formParams sendRfc3339DateTimeAsyncWithDatetime: datetime  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_unix_date_time_array_async_with_datetimes"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendUnixDateTimeArrayAsyncWithDatetimes") sendUnixDateTimeArrayAsyncWithDatetimes

> TODO: Add a method description


```objc
function sendUnixDateTimeArrayAsyncWithDatetimes:(NSArray*) datetimes
                completionBlock:(CompletedPostSendUnixDateTimeArray) onCompleted(datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* datetimes = (NSArray*) [APIHelper jsonDeserializeArray: @"[1484719381,1484719381]"];

    [self.formParams sendUnixDateTimeArrayAsyncWithDatetimes: datetimes  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_rfc1123_date_time_array_async_with_datetimes"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendRfc1123DateTimeArrayAsyncWithDatetimes") sendRfc1123DateTimeArrayAsyncWithDatetimes

> TODO: Add a method description


```objc
function sendRfc1123DateTimeArrayAsyncWithDatetimes:(NSArray*) datetimes
                completionBlock:(CompletedPostSendRfc1123DateTimeArray) onCompleted(datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* datetimes = (NSArray*) [APIHelper jsonDeserializeArray: @"[\"Sun, 06 Nov 1994 08:49:37 GMT\",\"Sun, 06 Nov 1994 08:49:37 GMT\"]"];

    [self.formParams sendRfc1123DateTimeArrayAsyncWithDatetimes: datetimes  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_long_async_with_value"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendLongAsyncWithValue") sendLongAsyncWithValue

> TODO: Add a method description


```objc
function sendLongAsyncWithValue:(long) value
                completionBlock:(CompletedPostSendLong) onCompleted(value)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| value |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    long value = [@"5147483647" longLongValue];

    [self.formParams sendLongAsyncWithValue: value  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_integer_array_async_with_integers"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendIntegerArrayAsyncWithIntegers") sendIntegerArrayAsyncWithIntegers

> TODO: Add a method description


```objc
function sendIntegerArrayAsyncWithIntegers:(NSArray*) integers
                completionBlock:(CompletedPostSendIntegerArray) onCompleted(integers)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* integers = (NSArray*) [APIHelper jsonDeserializeArray: @"[1,2,3,4,5]"];

    [self.formParams sendIntegerArrayAsyncWithIntegers: integers  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_string_array_async_with_strings"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendStringArrayAsyncWithStrings") sendStringArrayAsyncWithStrings

> TODO: Add a method description


```objc
function sendStringArrayAsyncWithStrings:(NSArray*) strings
                completionBlock:(CompletedPostSendStringArray) onCompleted(strings)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* strings = (NSArray*) [APIHelper jsonDeserializeArray: @"[\"abc\", \"def\"]"];

    [self.formParams sendStringArrayAsyncWithStrings: strings  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_model_async_with_model"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendModelAsyncWithModel") sendModelAsyncWithModel

> TODO: Add a method description


```objc
function sendModelAsyncWithModel:(Employee*) model
                completionBlock:(CompletedPostSendModel) onCompleted(model)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| model |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    Employee* model = (Employee*) [APIHelper jsonDeserialize: @"{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}"
                toClass: Employee.class];

    [self.formParams sendModelAsyncWithModel: model  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_model_array_async_with_models"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendModelArrayAsyncWithModels") sendModelArrayAsyncWithModels

> TODO: Add a method description


```objc
function sendModelArrayAsyncWithModels:(NSArray<Employee> *) models
                completionBlock:(CompletedPostSendModelArray) onCompleted(models)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| models |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray<Employee> * models = (NSArray<Employee>*) [Employee arrayOfModelsFromDictionaries:
                [APIHelper jsonDeserializeArray: @"[{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"},{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}]"] error: nil];

    [self.formParams sendModelArrayAsyncWithModels: models  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_file_async_with_file"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendFileAsyncWithFile") sendFileAsyncWithFile

> TODO: Add a method description


```objc
function sendFileAsyncWithFile:(NSURL*) file
                completionBlock:(CompletedPostSendFile) onCompleted(file)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSURL* file = [NSURL URLWithString: @"http://localhost:3000/response/image"];

    [self.formParams sendFileAsyncWithFile: file  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_string_async_with_value"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendStringAsyncWithValue") sendStringAsyncWithValue

> TODO: Add a method description


```objc
function sendStringAsyncWithValue:(NSString*) value
                completionBlock:(CompletedPostSendString) onCompleted(value)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| value |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* value = @"TestString";

    [self.formParams sendStringAsyncWithValue: value  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_rfc3339_date_time_array_async_with_datetimes"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendRfc3339DateTimeArrayAsyncWithDatetimes") sendRfc3339DateTimeArrayAsyncWithDatetimes

> TODO: Add a method description


```objc
function sendRfc3339DateTimeArrayAsyncWithDatetimes:(NSArray*) datetimes
                completionBlock:(CompletedPostSendRfc3339DateTimeArray) onCompleted(datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* datetimes = (NSArray*) [APIHelper jsonDeserializeArray: @"[\"1994-02-13T14:01:54.9571247Z\",\"1994-02-13T14:01:54.9571247Z\"]"];

    [self.formParams sendRfc3339DateTimeArrayAsyncWithDatetimes: datetimes  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_mixed_array_async_with_send_mixed_array_input"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendMixedArrayAsyncWithSendMixedArrayInput") sendMixedArrayAsyncWithSendMixedArrayInput

> Send a variety for form params. Returns file count and body params


```objc
function sendMixedArrayAsyncWithSendMixedArrayInput:(SendMixedArrayInput*) input
                completionBlock:(CompletedPostSendMixedArray) onCompleted(input)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | TODO: Add a parameter description |
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |
| models |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    SendMixedArrayInput *input = [[SendMixedArrayInput alloc]init];
    input.file = [NSURL URLWithString: @"http://localhost:3000/response/image"];
    input.integers = (NSArray*) [APIHelper jsonDeserializeArray: @"[1,2,3,4,5]"];
    input.models = (NSArray<Employee>*) [Employee arrayOfModelsFromDictionaries:
                [APIHelper jsonDeserializeArray: @"[{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"},{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}]"] error: nil];
    input.strings = (NSArray*) [APIHelper jsonDeserializeArray: @"[\"abc\", \"def\"]"];

    [self.formParams sendMixedArrayAsyncWithSendMixedArrayInput: input completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_integer_enum_array_async_with_suites"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendIntegerEnumArrayAsyncWithSuites") sendIntegerEnumArrayAsyncWithSuites

> TODO: Add a method description


```objc
function sendIntegerEnumArrayAsyncWithSuites:(NSArray<NSNumber*>*) suites
                completionBlock:(CompletedPostSendIntegerEnumArray) onCompleted(suites)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| suites |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray<NSNumber*>* suites =  (NSArray<NSNumber*>*) [APIHelper jsonDeserializeArray: @"[1, 3, 4, 2, 3]"];

    [self.formParams sendIntegerEnumArrayAsyncWithSuites: suites  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_string_enum_array_async_with_days"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.sendStringEnumArrayAsyncWithDays") sendStringEnumArrayAsyncWithDays

> TODO: Add a method description


```objc
function sendStringEnumArrayAsyncWithDays:(NSArray<NSNumber*>*) days
                completionBlock:(CompletedPostSendStringEnumArray) onCompleted(days)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| days |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray<NSNumber*>* days = [DaysHelper daysArrayFromStringArray:
                [APIHelper jsonDeserializeArray: @"[\"Tuesday\", \"Saturday\", \"Wednesday\", \"Monday\", \"Sunday\"]"]];

    [self.formParams sendStringEnumArrayAsyncWithDays: days  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="query_param_controller"></a>![Class: ](https://apidocs.io/img/class.png ".QueryParamController") QueryParamController

### Get singleton instance
```objc
QueryParam* queryParam = [[QueryParam alloc]init] ;
```

### <a name="date_array_async_with_dates"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.dateArrayAsyncWithDates") dateArrayAsyncWithDates

> TODO: Add a method description


```objc
function dateArrayAsyncWithDates:(NSArray*) dates
                completionBlock:(CompletedGetDateArray) onCompleted(dates)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dates |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* dates = (NSArray*) [APIHelper jsonDeserializeArray: @"[\"1994-02-13\",\"1994-02-13\"]"];

    [self.queryParam dateArrayAsyncWithDates: dates  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="date_async_with_date"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.dateAsyncWithDate") dateAsyncWithDate

> TODO: Add a method description


```objc
function dateAsyncWithDate:(NSDate*) date
                completionBlock:(CompletedGetDate) onCompleted(date)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| date |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSDate* date = [NSDate NSDateFromNSString: @"1994-02-13"];

    [self.queryParam dateAsyncWithDate: date  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="unix_date_time_array_async_with_datetimes"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.unixDateTimeArrayAsyncWithDatetimes") unixDateTimeArrayAsyncWithDatetimes

> TODO: Add a method description


```objc
function unixDateTimeArrayAsyncWithDatetimes:(NSArray*) datetimes
                completionBlock:(CompletedGetUnixDateTimeArray) onCompleted(datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* datetimes = (NSArray*) [APIHelper jsonDeserializeArray: @"[1484719381,1484719381]"];

    [self.queryParam unixDateTimeArrayAsyncWithDatetimes: datetimes  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="unix_date_time_async_with_datetime"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.unixDateTimeAsyncWithDatetime") unixDateTimeAsyncWithDatetime

> TODO: Add a method description


```objc
function unixDateTimeAsyncWithDatetime:(NSDate*) datetime
                completionBlock:(CompletedGetUnixDateTime) onCompleted(datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSDate* datetime = [NSDate NSDateFromNSString: @"1484719381"];

    [self.queryParam unixDateTimeAsyncWithDatetime: datetime  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="rfc1123_date_time_async_with_datetime"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.rfc1123DateTimeAsyncWithDatetime") rfc1123DateTimeAsyncWithDatetime

> TODO: Add a method description


```objc
function rfc1123DateTimeAsyncWithDatetime:(NSDate*) datetime
                completionBlock:(CompletedGetRfc1123DateTime) onCompleted(datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSDate* datetime = [NSDate NSDateFromNSString: @"Sun, 06 Nov 1994 08:49:37 GMT"];

    [self.queryParam rfc1123DateTimeAsyncWithDatetime: datetime  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="rfc1123_date_time_array_async_with_datetimes"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.rfc1123DateTimeArrayAsyncWithDatetimes") rfc1123DateTimeArrayAsyncWithDatetimes

> TODO: Add a method description


```objc
function rfc1123DateTimeArrayAsyncWithDatetimes:(NSArray*) datetimes
                completionBlock:(CompletedGetRfc1123DateTimeArray) onCompleted(datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* datetimes = (NSArray*) [APIHelper jsonDeserializeArray: @"[\"Sun, 06 Nov 1994 08:49:37 GMT\",\"Sun, 06 Nov 1994 08:49:37 GMT\"]"];

    [self.queryParam rfc1123DateTimeArrayAsyncWithDatetimes: datetimes  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="rfc3339_date_time_array_async_with_datetimes"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.rfc3339DateTimeArrayAsyncWithDatetimes") rfc3339DateTimeArrayAsyncWithDatetimes

> TODO: Add a method description


```objc
function rfc3339DateTimeArrayAsyncWithDatetimes:(NSArray*) datetimes
                completionBlock:(CompletedGetRfc3339DateTimeArray) onCompleted(datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* datetimes = (NSArray*) [APIHelper jsonDeserializeArray: @"[\"1994-02-13T14:01:54.9571247Z\",\"1994-02-13T14:01:54.9571247Z\"]"];

    [self.queryParam rfc3339DateTimeArrayAsyncWithDatetimes: datetimes  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="rfc3339_date_time_async_with_datetime"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.rfc3339DateTimeAsyncWithDatetime") rfc3339DateTimeAsyncWithDatetime

> TODO: Add a method description


```objc
function rfc3339DateTimeAsyncWithDatetime:(NSDate*) datetime
                completionBlock:(CompletedGetRfc3339DateTime) onCompleted(datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSDate* datetime = [NSDate NSDateFromNSString: @"1994-02-13T14:01:54.9571247Z"];

    [self.queryParam rfc3339DateTimeAsyncWithDatetime: datetime  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="no_params_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.noParamsWithCompletionBlock") noParamsWithCompletionBlock

> TODO: Add a method description


```objc
function noParamsWithCompletionBlock:(CompletedGetNoParams) onCompleted()
```



#### Example Usage

```objc

    [self.queryParam noParamsWithCompletionBlock:  ^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="string_param_async_with_string"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.stringParamAsyncWithString") stringParamAsyncWithString

> TODO: Add a method description


```objc
function stringParamAsyncWithString:(NSString*) string
                completionBlock:(CompletedGetStringParam) onCompleted(string)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| string |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* string = @"l;asd;asdwe[2304&&;'.d??\\a\\\\\\;sd//";

    [self.queryParam stringParamAsyncWithString: string  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="url_param_async_with_url"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.urlParamAsyncWithUrl") urlParamAsyncWithUrl

> TODO: Add a method description


```objc
function urlParamAsyncWithUrl:(NSString*) url
                completionBlock:(CompletedGetUrlParam) onCompleted(url)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| url |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* url = @"https://www.shahidisawesome.com/and/also/a/narcissist?thisis=aparameter&another=one";

    [self.queryParam urlParamAsyncWithUrl: url  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="number_array_async_with_integers"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.numberArrayAsyncWithIntegers") numberArrayAsyncWithIntegers

> TODO: Add a method description


```objc
function numberArrayAsyncWithIntegers:(NSArray*) integers
                completionBlock:(CompletedGetNumberArray) onCompleted(integers)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* integers = (NSArray*) [APIHelper jsonDeserializeArray: @"[1,2,3,4,5]"];

    [self.queryParam numberArrayAsyncWithIntegers: integers  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="string_array_async_with_strings"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.stringArrayAsyncWithStrings") stringArrayAsyncWithStrings

> TODO: Add a method description


```objc
function stringArrayAsyncWithStrings:(NSArray*) strings
                completionBlock:(CompletedGetStringArray) onCompleted(strings)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* strings = (NSArray*) [APIHelper jsonDeserializeArray: @"[\"abc\", \"def\"]"];

    [self.queryParam stringArrayAsyncWithStrings: strings  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="simple_query_async_with_boolean"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.simpleQueryAsyncWithBoolean") simpleQueryAsyncWithBoolean

> TODO: Add a method description


```objc
function simpleQueryAsyncWithBoolean:(BOOL) boolean
                number:(int) number
                string:(NSString*) string
                queryParameters:(NSDictionary*) queryParameters
                completionBlock:(CompletedGetSimpleQuery) onCompleted(boolean number : number string : string  queryParameters : queryParams)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| boolean |  ``` Required ```  | TODO: Add a parameter description |
| number |  ``` Required ```  | TODO: Add a parameter description |
| string |  ``` Required ```  | TODO: Add a parameter description |
| queryParameters | ``` Optional ``` | Additional optional query parameters are supported by this method |





#### Example Usage

```objc
    // Parameters for the API call
    BOOL boolean = [@"true" boolValue];
    int number = [@"4" intValue];
    NSString* string = @"TestString";
    // Dictionary for optional query parameters
    NSMutableDictionary* queryParamsMutable = [[NSMutableDictionary alloc] init];
    NSDictionary *queryParams= [queryParamsMutable copy];

    [self.queryParam simpleQueryAsyncWithBoolean: boolean number : number string : string  queryParameters : queryParams  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="string_enum_array_async_with_days"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.stringEnumArrayAsyncWithDays") stringEnumArrayAsyncWithDays

> TODO: Add a method description


```objc
function stringEnumArrayAsyncWithDays:(NSArray<NSNumber*>*) days
                completionBlock:(CompletedGetStringEnumArray) onCompleted(days)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| days |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray<NSNumber*>* days = [DaysHelper daysArrayFromStringArray:
                [APIHelper jsonDeserializeArray: @"[\"Tuesday\", \"Saturday\", \"Wednesday\", \"Monday\", \"Sunday\"]"]];

    [self.queryParam stringEnumArrayAsyncWithDays: days  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="multiple_params_async_with_number"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.multipleParamsAsyncWithNumber") multipleParamsAsyncWithNumber

> TODO: Add a method description


```objc
function multipleParamsAsyncWithNumber:(int) number
                precision:(double) precision
                string:(NSString*) string
                url:(NSString*) url
                completionBlock:(CompletedGetMultipleParams) onCompleted(number precision : precision string : string url : url)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| number |  ``` Required ```  | TODO: Add a parameter description |
| precision |  ``` Required ```  | TODO: Add a parameter description |
| string |  ``` Required ```  | TODO: Add a parameter description |
| url |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    int number = [@"123412312" intValue];
    double precision = [@"1112.34" doubleValue];
    NSString* string = @"\"\"test./;\";12&&3asl\"\";\"qw1&34\"///..//.";
    NSString* url = @"http://www.abc.com/test?a=b&c=\"http://lolol.com?param=no&another=lol\"";

    [self.queryParam multipleParamsAsyncWithNumber: number precision : precision string : string url : url  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="integer_enum_array_async_with_suites"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.integerEnumArrayAsyncWithSuites") integerEnumArrayAsyncWithSuites

> TODO: Add a method description


```objc
function integerEnumArrayAsyncWithSuites:(NSArray<NSNumber*>*) suites
                completionBlock:(CompletedGetIntegerEnumArray) onCompleted(suites)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| suites |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray<NSNumber*>* suites =  (NSArray<NSNumber*>*) [APIHelper jsonDeserializeArray: @"[1, 3, 4, 2, 3]"];

    [self.queryParam integerEnumArrayAsyncWithSuites: suites  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="error_codes_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ErrorCodesController") ErrorCodesController

### Get singleton instance
```objc
ErrorCodes* errorCodes = [[ErrorCodes alloc]init] ;
```

### <a name="get400_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ErrorCodesController.get400WithCompletionBlock") get400WithCompletionBlock

> TODO: Add a method description


```objc
function get400WithCompletionBlock:(CompletedGet400) onCompleted()
```



#### Example Usage

```objc

    [self.errorCodes get400WithCompletionBlock:  ^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get500_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ErrorCodesController.get500WithCompletionBlock") get500WithCompletionBlock

> TODO: Add a method description


```objc
function get500WithCompletionBlock:(CompletedGet500) onCompleted()
```



#### Example Usage

```objc

    [self.errorCodes get500WithCompletionBlock:  ^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```


### <a name="get401_with_completion_block"></a>![Method: ](https://apidocs.io/img/method.png ".ErrorCodesController.get401WithCompletionBlock") get401WithCompletionBlock

> TODO: Add a method description


```objc
function get401WithCompletionBlock:(CompletedGet401) onCompleted()
```



#### Example Usage

```objc

    [self.errorCodes get401WithCompletionBlock:  ^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
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

## <a name="echo_controller"></a>![Class: ](https://apidocs.io/img/class.png ".EchoController") EchoController

### Get singleton instance
```objc
Echo* echo = [[Echo alloc]init] ;
```

### <a name="json_echo_async_with_input"></a>![Method: ](https://apidocs.io/img/method.png ".EchoController.jsonEchoAsyncWithInput") jsonEchoAsyncWithInput

> Echo's back the request


```objc
function jsonEchoAsyncWithInput:(NSObject*) input
                completionBlock:(CompletedPostJsonEcho) onCompleted(input)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| input |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSObject* input = [NSJSONSerialization
                        JSONObjectWithData: [@"{\"uid\": \"1123213\", \"name\": \"Shahid\"}" dataUsingEncoding: NSUTF8StringEncoding]
                                   options: NSJSONReadingAllowFragments
                                     error: nil];

    [self.echo jsonEchoAsyncWithInput: input  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```


### <a name="form_echo_async_with_input"></a>![Method: ](https://apidocs.io/img/method.png ".EchoController.formEchoAsyncWithInput") formEchoAsyncWithInput

> Sends the request including any form params as JSON


```objc
function formEchoAsyncWithInput:(NSObject*) input
                completionBlock:(CompletedPostFormEcho) onCompleted(input)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| input |  ``` Required ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSObject* input = [NSJSONSerialization
                        JSONObjectWithData: [@"{\"uid\": \"1123213\", \"name\": \"Shahid\"}" dataUsingEncoding: NSUTF8StringEncoding]
                                   options: NSJSONReadingAllowFragments
                                     error: nil];

    [self.echo formEchoAsyncWithInput: input  completionBlock:^(BOOL success, HttpContext* context, id response, NSError* error) { 
       //Add code here
    }];
```


### <a name="query_echo_with_query_parameters"></a>![Method: ](https://apidocs.io/img/method.png ".EchoController.queryEchoWithQueryParameters") queryEchoWithQueryParameters

> TODO: Add a method description


```objc
function queryEchoWithQueryParameters:(NSDictionary*) queryParameters
                completionBlock:(CompletedGetQueryEcho) onCompleted(queryParams)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| queryParameters | ``` Optional ``` | Additional optional query parameters are supported by this method |





#### Example Usage

```objc
    // Dictionary for optional query parameters
    NSMutableDictionary* queryParamsMutable = [[NSMutableDictionary alloc] init];
    [queryParamsMutable setObject:@"world" forKey:@"hello"];
    NSDictionary *queryParams= [queryParamsMutable copy];

    [self.echo queryEchoWithQueryParameters: queryParams completionBlock:^(BOOL success, HttpContext* context, EchoResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="header_controller"></a>![Class: ](https://apidocs.io/img/class.png ".HeaderController") HeaderController

### Get singleton instance
```objc
Header* header = [[Header alloc]init] ;
```

### <a name="send_headers_async_with_custom_header"></a>![Method: ](https://apidocs.io/img/method.png ".HeaderController.sendHeadersAsyncWithCustomHeader") sendHeadersAsyncWithCustomHeader

> Sends a single header params


```objc
function sendHeadersAsyncWithCustomHeader:(NSString*) customHeader
                value:(NSString*) value
                completionBlock:(CompletedPostSendHeaders) onCompleted(customHeader value : value)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| customHeader |  ``` Required ```  | TODO: Add a parameter description |
| value |  ``` Required ```  | Represents the value of the custom header |





#### Example Usage

```objc
    // Parameters for the API call
    NSString* customHeader = @"TestString";
    NSString* value = @"TestString";

    [self.header sendHeadersAsyncWithCustomHeader: customHeader value : value  completionBlock:^(BOOL success, HttpContext* context, ServerResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)

## <a name="template_params_controller"></a>![Class: ](https://apidocs.io/img/class.png ".TemplateParamsController") TemplateParamsController

### Get singleton instance
```objc
TemplateParams* templateParams = [[TemplateParams alloc]init] ;
```

### <a name="send_string_array_async_with_strings"></a>![Method: ](https://apidocs.io/img/method.png ".TemplateParamsController.sendStringArrayAsyncWithStrings") sendStringArrayAsyncWithStrings

> TODO: Add a method description


```objc
function sendStringArrayAsyncWithStrings:(NSArray*) strings
                completionBlock:(CompletedGetSendStringArray) onCompleted(strings)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* strings = (NSArray*) [APIHelper jsonDeserializeArray: @"[\"abc\", \"def\"]"];

    [self.templateParams sendStringArrayAsyncWithStrings: strings  completionBlock:^(BOOL success, HttpContext* context, EchoResponse* response, NSError* error) { 
       //Add code here
    }];
```


### <a name="send_integer_array_async_with_integers"></a>![Method: ](https://apidocs.io/img/method.png ".TemplateParamsController.sendIntegerArrayAsyncWithIntegers") sendIntegerArrayAsyncWithIntegers

> TODO: Add a method description


```objc
function sendIntegerArrayAsyncWithIntegers:(NSArray*) integers
                completionBlock:(CompletedGetSendIntegerArray) onCompleted(integers)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |





#### Example Usage

```objc
    // Parameters for the API call
    NSArray* integers = (NSArray*) [APIHelper jsonDeserializeArray: @"[1,2,3,4,5]"];

    [self.templateParams sendIntegerArrayAsyncWithIntegers: integers  completionBlock:^(BOOL success, HttpContext* context, EchoResponse* response, NSError* error) { 
       //Add code here
    }];
```


[Back to List of Controllers](#list_of_controllers)



