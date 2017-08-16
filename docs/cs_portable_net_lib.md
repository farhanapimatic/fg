# Getting started

Testing various
 api 
features

## How to Build

The generated code uses the Newtonsoft Json.NET NuGet Package. If the automatic NuGet package restore
is enabled, these dependencies will be installed automatically. Therefore,
you will need internet access for build.

1. Open the solution (Tester.sln) file.
2. Invoke the build process using `Ctrl+Shift+B` shortcut key or using the `Build` menu as shown below.

![Building SDK using Visual Studio](https://apidocs.io/illustration/cs?step=buildSDK&workspaceFolder=Tester-CSharp&workspaceName=Tester&projectName=Tester.Tests)

## How to Use

The build process generates a portable class library, which can be used like a normal class library. The generated library is compatible with Windows Forms, Windows RT, Windows Phone 8,
Silverlight 5, Xamarin iOS, Xamarin Android and Mono. More information on how to use can be found at the [MSDN Portable Class Libraries documentation](http://msdn.microsoft.com/en-us/library/vstudio/gg597391%28v=vs.100%29.aspx).

The following section explains how to use the Tester library in a new console project.

### 1. Starting a new project

For starting a new project, right click on the current solution from the *solution explorer* and choose  ``` Add -> New Project ```.

![Add a new project in the existing solution using Visual Studio](https://apidocs.io/illustration/cs?step=addProject&workspaceFolder=Tester-CSharp&workspaceName=Tester&projectName=Tester.Tests)

Next, choose "Console Application", provide a ``` TestConsoleProject ``` as the project name and click ``` OK ```.

![Create a new console project using Visual Studio](https://apidocs.io/illustration/cs?step=createProject&workspaceFolder=Tester-CSharp&workspaceName=Tester&projectName=Tester.Tests)

### 2. Set as startup project

The new console project is the entry point for the eventual execution. This requires us to set the ``` TestConsoleProject ``` as the start-up project. To do this, right-click on the  ``` TestConsoleProject ``` and choose  ``` Set as StartUp Project ``` form the context menu.

![Set the new cosole project as the start up project](https://apidocs.io/illustration/cs?step=setStartup&workspaceFolder=Tester-CSharp&workspaceName=Tester&projectName=Tester.Tests)

### 3. Add reference of the library project

In order to use the Tester library in the new project, first we must add a projet reference to the ``` TestConsoleProject ```. First, right click on the ``` References ``` node in the *solution explorer* and click ``` Add Reference... ```.

![Open references of the TestConsoleProject](https://apidocs.io/illustration/cs?step=addReference&workspaceFolder=Tester-CSharp&workspaceName=Tester&projectName=Tester.Tests)

Next, a window will be displayed where we must set the ``` checkbox ``` on ``` Tester.Tests ``` and click ``` OK ```. By doing this, we have added a reference of the ```Tester.Tests``` project into the new ``` TestConsoleProject ```.

![Add a reference to the TestConsoleProject](https://apidocs.io/illustration/cs?step=createReference&workspaceFolder=Tester-CSharp&workspaceName=Tester&projectName=Tester.Tests)

### 4. Write sample code

Once the ``` TestConsoleProject ``` is created, a file named ``` Program.cs ``` will be visible in the *solution explorer* with an empty ``` Main ``` method. This is the entry point for the execution of the entire solution.
Here, you can add code to initialize the client library and acquire the instance of a *Controller* class. Sample code to initialize the client library and using controller methods is given in the subsequent sections.

![Add a reference to the TestConsoleProject](https://apidocs.io/illustration/cs?step=addCode&workspaceFolder=Tester-CSharp&workspaceName=Tester&projectName=Tester.Tests)

## How to Test

The generated SDK also contain one or more Tests, which are contained in the Tests project.
In order to invoke these test cases, you will need *NUnit 3.0 Test Adapter Extension for Visual Studio*.
Once the SDK is complied, the test cases should appear in the Test Explorer window.
Here, you can click *Run All* to execute these test cases.

## Initialization

### 

API client can be initialized as following.

```csharp

TesterClient client = new TesterClient();
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

## <a name="response_types_controller"></a>![Class: ](https://apidocs.io/img/class.png "Tester.Tests.Controllers.ResponseTypesController") ResponseTypesController

### Get singleton instance

The singleton instance of the ``` ResponseTypesController ``` class can be accessed from the API Client.

```csharp
IResponseTypesController responseTypes = client.ResponseTypes;
```

### <a name="get_date_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.GetDateArray") GetDateArray

> TODO: Add a method description


```csharp
Task<List<DateTime>> GetDateArray()
```

#### Example Usage

```csharp

List<DateTime> result = await responseTypes.GetDateArray();

```


### <a name="get_date"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.GetDate") GetDate

> TODO: Add a method description


```csharp
Task<DateTime?> GetDate()
```

#### Example Usage

```csharp

DateTime? result = await responseTypes.GetDate();

```


### <a name="get_long"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.GetLong") GetLong

> TODO: Add a method description


```csharp
Task<long?> GetLong()
```

#### Example Usage

```csharp

long? result = await responseTypes.GetLong();

```


### <a name="get_model"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.GetModel") GetModel

> TODO: Add a method description


```csharp
Task<PCL.Models.Person> GetModel()
```

#### Example Usage

```csharp

PCL.Models.Person result = await responseTypes.GetModel();

```


### <a name="get_string_enum_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.GetStringEnumArray") GetStringEnumArray

> TODO: Add a method description


```csharp
Task<List<PCL.Models.Days>> GetStringEnumArray()
```

#### Example Usage

```csharp

List<PCL.Models.Days> result = await responseTypes.GetStringEnumArray();

```


### <a name="get_string_enum"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.GetStringEnum") GetStringEnum

> TODO: Add a method description


```csharp
Task<PCL.Models.Days?> GetStringEnum()
```

#### Example Usage

```csharp

PCL.Models.Days? result = await responseTypes.GetStringEnum();

```


### <a name="get_model_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.GetModelArray") GetModelArray

> TODO: Add a method description


```csharp
Task<List<PCL.Models.Person>> GetModelArray()
```

#### Example Usage

```csharp

List<PCL.Models.Person> result = await responseTypes.GetModelArray();

```


### <a name="get_int_enum"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.GetIntEnum") GetIntEnum

> TODO: Add a method description


```csharp
Task<PCL.Models.SuiteCode?> GetIntEnum()
```

#### Example Usage

```csharp

PCL.Models.SuiteCode? result = await responseTypes.GetIntEnum();

```


### <a name="get_int_enum_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.GetIntEnumArray") GetIntEnumArray

> TODO: Add a method description


```csharp
Task<List<PCL.Models.SuiteCode>> GetIntEnumArray()
```

#### Example Usage

```csharp

List<PCL.Models.SuiteCode> result = await responseTypes.GetIntEnumArray();

```


### <a name="get_precision"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.GetPrecision") GetPrecision

> TODO: Add a method description


```csharp
Task<double?> GetPrecision()
```

#### Example Usage

```csharp

double? result = await responseTypes.GetPrecision();

```


### <a name="get_binary"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.GetBinary") GetBinary

> gets a binary object


```csharp
Task<Stream> GetBinary()
```

#### Example Usage

```csharp

Stream result = await responseTypes.GetBinary();

```


### <a name="get_integer"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.GetInteger") GetInteger

> Gets a integer response


```csharp
Task<int?> GetInteger()
```

#### Example Usage

```csharp

int? result = await responseTypes.GetInteger();

```


### <a name="get_integer_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.GetIntegerArray") GetIntegerArray

> Get an array of integers.


```csharp
Task<List<int>> GetIntegerArray()
```

#### Example Usage

```csharp

List<int> result = await responseTypes.GetIntegerArray();

```


### <a name="get_dynamic"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.GetDynamic") GetDynamic

> TODO: Add a method description


```csharp
Task<dynamic> GetDynamic()
```

#### Example Usage

```csharp

dynamic result = await responseTypes.GetDynamic();

```


### <a name="get_dynamic_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.GetDynamicArray") GetDynamicArray

> TODO: Add a method description


```csharp
Task<dynamic> GetDynamicArray()
```

#### Example Usage

```csharp

dynamic result = await responseTypes.GetDynamicArray();

```


### <a name="get3339_datetime"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.Get3339Datetime") Get3339Datetime

> TODO: Add a method description


```csharp
Task<DateTime?> Get3339Datetime()
```

#### Example Usage

```csharp

DateTime? result = await responseTypes.Get3339Datetime();

```


### <a name="get3339_datetime_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.Get3339DatetimeArray") Get3339DatetimeArray

> TODO: Add a method description


```csharp
Task<List<DateTime>> Get3339DatetimeArray()
```

#### Example Usage

```csharp

List<DateTime> result = await responseTypes.Get3339DatetimeArray();

```


### <a name="get_boolean"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.GetBoolean") GetBoolean

> TODO: Add a method description


```csharp
Task<bool?> GetBoolean()
```

#### Example Usage

```csharp

bool? result = await responseTypes.GetBoolean();

```


### <a name="get_boolean_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.GetBooleanArray") GetBooleanArray

> TODO: Add a method description


```csharp
Task<List<bool>> GetBooleanArray()
```

#### Example Usage

```csharp

List<bool> result = await responseTypes.GetBooleanArray();

```


### <a name="get_headers"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.GetHeaders") GetHeaders

> TODO: Add a method description


```csharp
Task GetHeaders()
```

#### Example Usage

```csharp

await responseTypes.GetHeaders();

```


### <a name="get1123_date_time"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.Get1123DateTime") Get1123DateTime

> TODO: Add a method description


```csharp
Task<DateTime?> Get1123DateTime()
```

#### Example Usage

```csharp

DateTime? result = await responseTypes.Get1123DateTime();

```


### <a name="get_unix_date_time"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.GetUnixDateTime") GetUnixDateTime

> TODO: Add a method description


```csharp
Task<DateTime?> GetUnixDateTime()
```

#### Example Usage

```csharp

DateTime? result = await responseTypes.GetUnixDateTime();

```


### <a name="get1123_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.Get1123DateTimeArray") Get1123DateTimeArray

> TODO: Add a method description


```csharp
Task<List<DateTime>> Get1123DateTimeArray()
```

#### Example Usage

```csharp

List<DateTime> result = await responseTypes.Get1123DateTimeArray();

```


### <a name="get_unix_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ResponseTypesController.GetUnixDateTimeArray") GetUnixDateTimeArray

> TODO: Add a method description


```csharp
Task<List<DateTime>> GetUnixDateTimeArray()
```

#### Example Usage

```csharp

List<DateTime> result = await responseTypes.GetUnixDateTimeArray();

```


[Back to List of Controllers](#list_of_controllers)

## <a name="body_params_controller"></a>![Class: ](https://apidocs.io/img/class.png "Tester.Tests.Controllers.BodyParamsController") BodyParamsController

### Get singleton instance

The singleton instance of the ``` BodyParamsController ``` class can be accessed from the API Client.

```csharp
IBodyParamsController bodyParams = client.BodyParams;
```

### <a name="send_date_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.BodyParamsController.SendDateArray") SendDateArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendDateArray(List<DateTime> dates)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dates |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string datesValue = ["1994-02-13", "1994-02-13"];
var dates = Newtonsoft.Json.JsonConvert.DeserializeObject<List<DateTime>>(datesValue);

PCL.Models.ServerResponse result = await bodyParams.SendDateArray(dates);

```


### <a name="send_date"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.BodyParamsController.SendDate") SendDate

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendDate(DateTime date)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| date |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
DateTime date = 1994-02-13;

PCL.Models.ServerResponse result = await bodyParams.SendDate(date);

```


### <a name="send_unix_date_time"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.BodyParamsController.SendUnixDateTime") SendUnixDateTime

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendUnixDateTime(DateTime datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
DateTime datetime = 1484719381;

PCL.Models.ServerResponse result = await bodyParams.SendUnixDateTime(datetime);

```


### <a name="send_rfc1123_date_time"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.BodyParamsController.SendRfc1123DateTime") SendRfc1123DateTime

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendRfc1123DateTime(DateTime datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
DateTime datetime = Sun, 06 Nov 1994 08:49:37 GMT;

PCL.Models.ServerResponse result = await bodyParams.SendRfc1123DateTime(datetime);

```


### <a name="send_rfc3339_date_time"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.BodyParamsController.SendRfc3339DateTime") SendRfc3339DateTime

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendRfc3339DateTime(DateTime datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
DateTime datetime = 1994-02-13T14:01:54.9571247Z;

PCL.Models.ServerResponse result = await bodyParams.SendRfc3339DateTime(datetime);

```


### <a name="send_unix_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.BodyParamsController.SendUnixDateTimeArray") SendUnixDateTimeArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendUnixDateTimeArray(List<DateTime> datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string datetimesValue = [1484719381,1484719381];
var datetimes = Newtonsoft.Json.JsonConvert.DeserializeObject<List<DateTime>>(datetimesValue);

PCL.Models.ServerResponse result = await bodyParams.SendUnixDateTimeArray(datetimes);

```


### <a name="send_rfc1123_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.BodyParamsController.SendRfc1123DateTimeArray") SendRfc1123DateTimeArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendRfc1123DateTimeArray(List<DateTime> datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string datetimesValue = ["Sun, 06 Nov 1994 08:49:37 GMT","Sun, 06 Nov 1994 08:49:37 GMT"];
var datetimes = Newtonsoft.Json.JsonConvert.DeserializeObject<List<DateTime>>(datetimesValue);

PCL.Models.ServerResponse result = await bodyParams.SendRfc1123DateTimeArray(datetimes);

```


### <a name="send_rfc3339_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.BodyParamsController.SendRfc3339DateTimeArray") SendRfc3339DateTimeArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendRfc3339DateTimeArray(List<DateTime> datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string datetimesValue = ["1994-02-13T14:01:54.9571247Z","1994-02-13T14:01:54.9571247Z"];
var datetimes = Newtonsoft.Json.JsonConvert.DeserializeObject<List<DateTime>>(datetimesValue);

PCL.Models.ServerResponse result = await bodyParams.SendRfc3339DateTimeArray(datetimes);

```


### <a name="send_string_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.BodyParamsController.SendStringArray") SendStringArray

> sends a string body param


```csharp
Task<PCL.Models.ServerResponse> SendStringArray(List<string> sarray)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| sarray |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string sarrayValue = "[\"abc\", \"def\"]";
var sarray = Newtonsoft.Json.JsonConvert.DeserializeObject<List<string>>(sarrayValue);

PCL.Models.ServerResponse result = await bodyParams.SendStringArray(sarray);

```


### <a name="send_integer_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.BodyParamsController.SendIntegerArray") SendIntegerArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendIntegerArray(List<int> integers)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string integersValue = "[1,2,3,4,5]";
var integers = Newtonsoft.Json.JsonConvert.DeserializeObject<List<int>>(integersValue);

PCL.Models.ServerResponse result = await bodyParams.SendIntegerArray(integers);

```


### <a name="send_model"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.BodyParamsController.SendModel") SendModel

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendModel(PCL.Models.Employee model)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| model |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string modelValue = "{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}";
var model = Newtonsoft.Json.JsonConvert.DeserializeObject<PCL.Models.Employee>(modelValue);

PCL.Models.ServerResponse result = await bodyParams.SendModel(model);

```


### <a name="send_model_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.BodyParamsController.SendModelArray") SendModelArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendModelArray(List<PCL.Models.Employee> models)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| models |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string modelsValue = "[{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"},{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}]";
var models = Newtonsoft.Json.JsonConvert.DeserializeObject<List<PCL.Models.Employee>>(modelsValue);

PCL.Models.ServerResponse result = await bodyParams.SendModelArray(models);

```


### <a name="send_dynamic"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.BodyParamsController.SendDynamic") SendDynamic

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendDynamic(object mdynamic)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mdynamic |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string mdynamicValue = "{\"uid\": \"1123213\", \"name\": \"Shahid\"}";
var mdynamic = Newtonsoft.Json.JsonConvert.DeserializeObject(mdynamicValue);

PCL.Models.ServerResponse result = await bodyParams.SendDynamic(mdynamic);

```


### <a name="send_string"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.BodyParamsController.SendString") SendString

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendString(string mvalue)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mvalue |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string mvalue = "TestString";

PCL.Models.ServerResponse result = await bodyParams.SendString(mvalue);

```


### <a name="send_string_enum_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.BodyParamsController.SendStringEnumArray") SendStringEnumArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendStringEnumArray(List<PCL.Models.Days> days)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| days |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string daysValue = "[\"Tuesday\", \"Saturday\", \"Wednesday\", \"Monday\", \"Sunday\"]";
var days = Newtonsoft.Json.JsonConvert.DeserializeObject<List<PCL.Models.Days>>(daysValue);

PCL.Models.ServerResponse result = await bodyParams.SendStringEnumArray(days);

```


### <a name="send_integer_enum_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.BodyParamsController.SendIntegerEnumArray") SendIntegerEnumArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendIntegerEnumArray(List<PCL.Models.SuiteCode> suites)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| suites |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string suitesValue = "[1, 3, 4, 2, 3]";
var suites = Newtonsoft.Json.JsonConvert.DeserializeObject<List<PCL.Models.SuiteCode>>(suitesValue);

PCL.Models.ServerResponse result = await bodyParams.SendIntegerEnumArray(suites);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="form_params_controller"></a>![Class: ](https://apidocs.io/img/class.png "Tester.Tests.Controllers.FormParamsController") FormParamsController

### Get singleton instance

The singleton instance of the ``` FormParamsController ``` class can be accessed from the API Client.

```csharp
IFormParamsController formParams = client.FormParams;
```

### <a name="send_date_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.FormParamsController.SendDateArray") SendDateArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendDateArray(List<DateTime> dates)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dates |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string datesValue = ["1994-02-13","1994-02-13"];
var dates = Newtonsoft.Json.JsonConvert.DeserializeObject<List<DateTime>>(datesValue);

PCL.Models.ServerResponse result = await formParams.SendDateArray(dates);

```


### <a name="send_date"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.FormParamsController.SendDate") SendDate

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendDate(DateTime date)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| date |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
DateTime date = 1994-02-13;

PCL.Models.ServerResponse result = await formParams.SendDate(date);

```


### <a name="send_unix_date_time"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.FormParamsController.SendUnixDateTime") SendUnixDateTime

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendUnixDateTime(DateTime datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
DateTime datetime = 1484719381;

PCL.Models.ServerResponse result = await formParams.SendUnixDateTime(datetime);

```


### <a name="send_rfc1123_date_time"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.FormParamsController.SendRfc1123DateTime") SendRfc1123DateTime

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendRfc1123DateTime(DateTime datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
DateTime datetime = Sun, 06 Nov 1994 08:49:37 GMT;

PCL.Models.ServerResponse result = await formParams.SendRfc1123DateTime(datetime);

```


### <a name="send_rfc3339_date_time"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.FormParamsController.SendRfc3339DateTime") SendRfc3339DateTime

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendRfc3339DateTime(DateTime datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
DateTime datetime = 1994-02-13T14:01:54.9571247Z;

PCL.Models.ServerResponse result = await formParams.SendRfc3339DateTime(datetime);

```


### <a name="send_unix_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.FormParamsController.SendUnixDateTimeArray") SendUnixDateTimeArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendUnixDateTimeArray(List<DateTime> datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string datetimesValue = [1484719381,1484719381];
var datetimes = Newtonsoft.Json.JsonConvert.DeserializeObject<List<DateTime>>(datetimesValue);

PCL.Models.ServerResponse result = await formParams.SendUnixDateTimeArray(datetimes);

```


### <a name="send_rfc1123_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.FormParamsController.SendRfc1123DateTimeArray") SendRfc1123DateTimeArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendRfc1123DateTimeArray(List<DateTime> datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string datetimesValue = ["Sun, 06 Nov 1994 08:49:37 GMT","Sun, 06 Nov 1994 08:49:37 GMT"];
var datetimes = Newtonsoft.Json.JsonConvert.DeserializeObject<List<DateTime>>(datetimesValue);

PCL.Models.ServerResponse result = await formParams.SendRfc1123DateTimeArray(datetimes);

```


### <a name="send_long"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.FormParamsController.SendLong") SendLong

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendLong(long mvalue)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mvalue |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
long mvalue = 5147483647L;

PCL.Models.ServerResponse result = await formParams.SendLong(mvalue);

```


### <a name="send_integer_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.FormParamsController.SendIntegerArray") SendIntegerArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendIntegerArray(List<int> integers)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string integersValue = "[1,2,3,4,5]";
var integers = Newtonsoft.Json.JsonConvert.DeserializeObject<List<int>>(integersValue);

PCL.Models.ServerResponse result = await formParams.SendIntegerArray(integers);

```


### <a name="send_string_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.FormParamsController.SendStringArray") SendStringArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendStringArray(List<string> strings)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string stringsValue = "[\"abc\", \"def\"]";
var strings = Newtonsoft.Json.JsonConvert.DeserializeObject<List<string>>(stringsValue);

PCL.Models.ServerResponse result = await formParams.SendStringArray(strings);

```


### <a name="send_model"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.FormParamsController.SendModel") SendModel

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendModel(PCL.Models.Employee model)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| model |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string modelValue = "{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}";
var model = Newtonsoft.Json.JsonConvert.DeserializeObject<PCL.Models.Employee>(modelValue);

PCL.Models.ServerResponse result = await formParams.SendModel(model);

```


### <a name="send_model_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.FormParamsController.SendModelArray") SendModelArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendModelArray(List<PCL.Models.Employee> models)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| models |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string modelsValue = "[{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"},{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}]";
var models = Newtonsoft.Json.JsonConvert.DeserializeObject<List<PCL.Models.Employee>>(modelsValue);

PCL.Models.ServerResponse result = await formParams.SendModelArray(models);

```


### <a name="send_file"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.FormParamsController.SendFile") SendFile

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendFile(FileStreamInfo file)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
FileStreamInfo file = new FileStreamInfo(new FileStream(@"pathToFile",FileMode.Open));

PCL.Models.ServerResponse result = await formParams.SendFile(file);

```


### <a name="send_string"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.FormParamsController.SendString") SendString

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendString(string mvalue)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mvalue |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string mvalue = "TestString";

PCL.Models.ServerResponse result = await formParams.SendString(mvalue);

```


### <a name="send_rfc3339_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.FormParamsController.SendRfc3339DateTimeArray") SendRfc3339DateTimeArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendRfc3339DateTimeArray(List<DateTime> datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string datetimesValue = ["1994-02-13T14:01:54.9571247Z","1994-02-13T14:01:54.9571247Z"];
var datetimes = Newtonsoft.Json.JsonConvert.DeserializeObject<List<DateTime>>(datetimesValue);

PCL.Models.ServerResponse result = await formParams.SendRfc3339DateTimeArray(datetimes);

```


### <a name="send_mixed_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.FormParamsController.SendMixedArray") SendMixedArray

> Send a variety for form params. Returns file count and body params


```csharp
Task<PCL.Models.ServerResponse> SendMixedArray(PCL.Models.SendMixedArrayInput input)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | TODO: Add a parameter description |
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |
| models |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
SendMixedArrayInput collect = new SendMixedArrayInput();

FileStreamInfo file = new FileStreamInfo(new FileStream(@"pathToFile",FileMode.Open));
collect.File = file;

string integersValue = "[1,2,3,4,5]";
var integers = Newtonsoft.Json.JsonConvert.DeserializeObject<List<int>>(integersValue);
collect.Integers = integers;

string modelsValue = "[{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"},{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}]";
var models = Newtonsoft.Json.JsonConvert.DeserializeObject<List<PCL.Models.Employee>>(modelsValue);
collect.Models = models;

string stringsValue = "[\"abc\", \"def\"]";
var strings = Newtonsoft.Json.JsonConvert.DeserializeObject<List<string>>(stringsValue);
collect.Strings = strings;


PCL.Models.ServerResponse result = await formParams.SendMixedArray(collect);

```


### <a name="send_integer_enum_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.FormParamsController.SendIntegerEnumArray") SendIntegerEnumArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendIntegerEnumArray(List<PCL.Models.SuiteCode> suites)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| suites |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string suitesValue = "[1, 3, 4, 2, 3]";
var suites = Newtonsoft.Json.JsonConvert.DeserializeObject<List<PCL.Models.SuiteCode>>(suitesValue);

PCL.Models.ServerResponse result = await formParams.SendIntegerEnumArray(suites);

```


### <a name="send_string_enum_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.FormParamsController.SendStringEnumArray") SendStringEnumArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SendStringEnumArray(List<PCL.Models.Days> days)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| days |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string daysValue = "[\"Tuesday\", \"Saturday\", \"Wednesday\", \"Monday\", \"Sunday\"]";
var days = Newtonsoft.Json.JsonConvert.DeserializeObject<List<PCL.Models.Days>>(daysValue);

PCL.Models.ServerResponse result = await formParams.SendStringEnumArray(days);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="query_param_controller"></a>![Class: ](https://apidocs.io/img/class.png "Tester.Tests.Controllers.QueryParamController") QueryParamController

### Get singleton instance

The singleton instance of the ``` QueryParamController ``` class can be accessed from the API Client.

```csharp
IQueryParamController queryParam = client.QueryParam;
```

### <a name="date_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.QueryParamController.DateArray") DateArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> DateArray(List<DateTime> dates)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dates |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string datesValue = ["1994-02-13","1994-02-13"];
var dates = Newtonsoft.Json.JsonConvert.DeserializeObject<List<DateTime>>(datesValue);

PCL.Models.ServerResponse result = await queryParam.DateArray(dates);

```


### <a name="date"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.QueryParamController.Date") Date

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> Date(DateTime date)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| date |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
DateTime date = 1994-02-13;

PCL.Models.ServerResponse result = await queryParam.Date(date);

```


### <a name="unix_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.QueryParamController.UnixDateTimeArray") UnixDateTimeArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> UnixDateTimeArray(List<DateTime> datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string datetimesValue = [1484719381,1484719381];
var datetimes = Newtonsoft.Json.JsonConvert.DeserializeObject<List<DateTime>>(datetimesValue);

PCL.Models.ServerResponse result = await queryParam.UnixDateTimeArray(datetimes);

```


### <a name="unix_date_time"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.QueryParamController.UnixDateTime") UnixDateTime

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> UnixDateTime(DateTime datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
DateTime datetime = 1484719381;

PCL.Models.ServerResponse result = await queryParam.UnixDateTime(datetime);

```


### <a name="rfc1123_date_time"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.QueryParamController.Rfc1123DateTime") Rfc1123DateTime

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> Rfc1123DateTime(DateTime datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
DateTime datetime = Sun, 06 Nov 1994 08:49:37 GMT;

PCL.Models.ServerResponse result = await queryParam.Rfc1123DateTime(datetime);

```


### <a name="rfc1123_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.QueryParamController.Rfc1123DateTimeArray") Rfc1123DateTimeArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> Rfc1123DateTimeArray(List<DateTime> datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string datetimesValue = ["Sun, 06 Nov 1994 08:49:37 GMT","Sun, 06 Nov 1994 08:49:37 GMT"];
var datetimes = Newtonsoft.Json.JsonConvert.DeserializeObject<List<DateTime>>(datetimesValue);

PCL.Models.ServerResponse result = await queryParam.Rfc1123DateTimeArray(datetimes);

```


### <a name="rfc3339_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.QueryParamController.Rfc3339DateTimeArray") Rfc3339DateTimeArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> Rfc3339DateTimeArray(List<DateTime> datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string datetimesValue = ["1994-02-13T14:01:54.9571247Z","1994-02-13T14:01:54.9571247Z"];
var datetimes = Newtonsoft.Json.JsonConvert.DeserializeObject<List<DateTime>>(datetimesValue);

PCL.Models.ServerResponse result = await queryParam.Rfc3339DateTimeArray(datetimes);

```


### <a name="rfc3339_date_time"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.QueryParamController.Rfc3339DateTime") Rfc3339DateTime

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> Rfc3339DateTime(DateTime datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
DateTime datetime = 1994-02-13T14:01:54.9571247Z;

PCL.Models.ServerResponse result = await queryParam.Rfc3339DateTime(datetime);

```


### <a name="no_params"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.QueryParamController.NoParams") NoParams

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> NoParams()
```

#### Example Usage

```csharp

PCL.Models.ServerResponse result = await queryParam.NoParams();

```


### <a name="string_param"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.QueryParamController.StringParam") StringParam

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> StringParam(string mstring)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mstring |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string mstring = "l;asd;asdwe[2304&&;'.d??\\a\\\\\\;sd//";

PCL.Models.ServerResponse result = await queryParam.StringParam(mstring);

```


### <a name="url_param"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.QueryParamController.UrlParam") UrlParam

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> UrlParam(string url)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| url |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string url = "https://www.shahidisawesome.com/and/also/a/narcissist?thisis=aparameter&another=one";

PCL.Models.ServerResponse result = await queryParam.UrlParam(url);

```


### <a name="number_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.QueryParamController.NumberArray") NumberArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> NumberArray(List<int> integers)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string integersValue = "[1,2,3,4,5]";
var integers = Newtonsoft.Json.JsonConvert.DeserializeObject<List<int>>(integersValue);

PCL.Models.ServerResponse result = await queryParam.NumberArray(integers);

```


### <a name="string_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.QueryParamController.StringArray") StringArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> StringArray(List<string> strings)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string stringsValue = "[\"abc\", \"def\"]";
var strings = Newtonsoft.Json.JsonConvert.DeserializeObject<List<string>>(stringsValue);

PCL.Models.ServerResponse result = await queryParam.StringArray(strings);

```


### <a name="simple_query"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.QueryParamController.SimpleQuery") SimpleQuery

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> SimpleQuery(
        bool boolean,
        int number,
        string mstring,
        Dictionary<string, object> queryParameters = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| boolean |  ``` Required ```  | TODO: Add a parameter description |
| number |  ``` Required ```  | TODO: Add a parameter description |
| mstring |  ``` Required ```  | TODO: Add a parameter description |
| queryParameters | ``` Optional ``` | Additional optional query parameters are supported by this method |


#### Example Usage

```csharp
bool boolean = true;
int number = 4;
string mstring = "TestString";
// key-value map for optional query parameters
var queryParams = new Dictionary<string, object>();


PCL.Models.ServerResponse result = await queryParam.SimpleQuery(boolean, number, mstring, queryParams);

```


### <a name="string_enum_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.QueryParamController.StringEnumArray") StringEnumArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> StringEnumArray(List<PCL.Models.Days> days)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| days |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string daysValue = "[\"Tuesday\", \"Saturday\", \"Wednesday\", \"Monday\", \"Sunday\"]";
var days = Newtonsoft.Json.JsonConvert.DeserializeObject<List<PCL.Models.Days>>(daysValue);

PCL.Models.ServerResponse result = await queryParam.StringEnumArray(days);

```


### <a name="multiple_params"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.QueryParamController.MultipleParams") MultipleParams

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> MultipleParams(
        int number,
        double precision,
        string mstring,
        string url)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| number |  ``` Required ```  | TODO: Add a parameter description |
| precision |  ``` Required ```  | TODO: Add a parameter description |
| mstring |  ``` Required ```  | TODO: Add a parameter description |
| url |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
int number = 123412312;
double precision = 1112.34;
string mstring = "\"\"test./;\";12&&3asl\"\";\"qw1&34\"///..//.";
string url = "http://www.abc.com/test?a=b&c=\"http://lolol.com?param=no&another=lol\"";

PCL.Models.ServerResponse result = await queryParam.MultipleParams(number, precision, mstring, url);

```


### <a name="integer_enum_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.QueryParamController.IntegerEnumArray") IntegerEnumArray

> TODO: Add a method description


```csharp
Task<PCL.Models.ServerResponse> IntegerEnumArray(List<PCL.Models.SuiteCode> suites)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| suites |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string suitesValue = "[1, 3, 4, 2, 3]";
var suites = Newtonsoft.Json.JsonConvert.DeserializeObject<List<PCL.Models.SuiteCode>>(suitesValue);

PCL.Models.ServerResponse result = await queryParam.IntegerEnumArray(suites);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="error_codes_controller"></a>![Class: ](https://apidocs.io/img/class.png "Tester.Tests.Controllers.ErrorCodesController") ErrorCodesController

### Get singleton instance

The singleton instance of the ``` ErrorCodesController ``` class can be accessed from the API Client.

```csharp
IErrorCodesController errorCodes = client.ErrorCodes;
```

### <a name="get400"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ErrorCodesController.Get400") Get400

> TODO: Add a method description


```csharp
Task<dynamic> Get400()
```

#### Example Usage

```csharp

dynamic result = await errorCodes.Get400();

```


### <a name="get500"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ErrorCodesController.Get500") Get500

> TODO: Add a method description


```csharp
Task<dynamic> Get500()
```

#### Example Usage

```csharp

dynamic result = await errorCodes.Get500();

```


### <a name="get401"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.ErrorCodesController.Get401") Get401

> TODO: Add a method description


```csharp
Task<dynamic> Get401()
```

#### Example Usage

```csharp

dynamic result = await errorCodes.Get401();

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

## <a name="echo_controller"></a>![Class: ](https://apidocs.io/img/class.png "Tester.Tests.Controllers.EchoController") EchoController

### Get singleton instance

The singleton instance of the ``` EchoController ``` class can be accessed from the API Client.

```csharp
IEchoController echo = client.Echo;
```

### <a name="json_echo"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.EchoController.JsonEcho") JsonEcho

> Echo's back the request


```csharp
Task<dynamic> JsonEcho(object input)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| input |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string inputValue = "{\"uid\": \"1123213\", \"name\": \"Shahid\"}";
var input = Newtonsoft.Json.JsonConvert.DeserializeObject(inputValue);

dynamic result = await echo.JsonEcho(input);

```


### <a name="form_echo"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.EchoController.FormEcho") FormEcho

> Sends the request including any form params as JSON


```csharp
Task<dynamic> FormEcho(object input)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| input |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string inputValue = "{\"uid\": \"1123213\", \"name\": \"Shahid\"}";
var input = Newtonsoft.Json.JsonConvert.DeserializeObject(inputValue);

dynamic result = await echo.FormEcho(input);

```


### <a name="query_echo"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.EchoController.QueryEcho") QueryEcho

> TODO: Add a method description


```csharp
Task<PCL.Models.EchoResponse> QueryEcho(Dictionary<string, object> queryParameters = null)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| queryParameters | ``` Optional ``` | Additional optional query parameters are supported by this method |


#### Example Usage

```csharp
// key-value map for optional query parameters
var queryParams = new Dictionary<string, object>();


PCL.Models.EchoResponse result = await echo.QueryEcho(queryParams);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="header_controller"></a>![Class: ](https://apidocs.io/img/class.png "Tester.Tests.Controllers.HeaderController") HeaderController

### Get singleton instance

The singleton instance of the ``` HeaderController ``` class can be accessed from the API Client.

```csharp
IHeaderController header = client.Header;
```

### <a name="send_headers"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.HeaderController.SendHeaders") SendHeaders

> Sends a single header params


```csharp
Task<PCL.Models.ServerResponse> SendHeaders(string customHeader, string mvalue)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| customHeader |  ``` Required ```  | TODO: Add a parameter description |
| mvalue |  ``` Required ```  | Represents the value of the custom header |


#### Example Usage

```csharp
string customHeader = "TestString";
string mvalue = "TestString";

PCL.Models.ServerResponse result = await header.SendHeaders(customHeader, mvalue);

```


[Back to List of Controllers](#list_of_controllers)

## <a name="template_params_controller"></a>![Class: ](https://apidocs.io/img/class.png "Tester.Tests.Controllers.TemplateParamsController") TemplateParamsController

### Get singleton instance

The singleton instance of the ``` TemplateParamsController ``` class can be accessed from the API Client.

```csharp
ITemplateParamsController templateParams = client.TemplateParams;
```

### <a name="send_string_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.TemplateParamsController.SendStringArray") SendStringArray

> TODO: Add a method description


```csharp
Task<PCL.Models.EchoResponse> SendStringArray(List<string> strings)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string stringsValue = "[\"abc\", \"def\"]";
var strings = Newtonsoft.Json.JsonConvert.DeserializeObject<List<string>>(stringsValue);

PCL.Models.EchoResponse result = await templateParams.SendStringArray(strings);

```


### <a name="send_integer_array"></a>![Method: ](https://apidocs.io/img/method.png "Tester.Tests.Controllers.TemplateParamsController.SendIntegerArray") SendIntegerArray

> TODO: Add a method description


```csharp
Task<PCL.Models.EchoResponse> SendIntegerArray(List<int> integers)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
string integersValue = "[1,2,3,4,5]";
var integers = Newtonsoft.Json.JsonConvert.DeserializeObject<List<int>>(integersValue);

PCL.Models.EchoResponse result = await templateParams.SendIntegerArray(integers);

```


[Back to List of Controllers](#list_of_controllers)



