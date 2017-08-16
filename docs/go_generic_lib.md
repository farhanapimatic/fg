# Getting started

Testing various
 api 
features

## How to Build


* In order to successfully build and run your SDK files, you are required to have the following setup in your system:
    * **Go**  (Visit [https://golang.org/doc/install](https://golang.org/doc/install) for more details on how to install Go)
    * **Java VM** Version 8 or later
    * **Eclipse 4.6 (Neon)** or later ([http://www.eclipse.org/neon/](http://www.eclipse.org/neon/))
    * **GoClipse** setup within above installed Eclipse (Follow the instructions at [this link](https://github.com/GoClipse/goclipse/blob/latest/documentation/Installation.md#instructions) to setup GoClipse)
* Ensure that ```GOPATH``` environment variable is set in the system variables. If not, set it to your workspace directory where you will be adding your Go projects.
* The generated code uses unirest-go http library. Therefore, you will need internet access to resolve this dependency. If Go is properly installed and configured, run the following command to pull the dependency:

```Go
go get github.com/apimatic/unirest-go
```

This will install unirest-go in the ```GOPATH``` you specified in the system variables.

Now follow the steps mentioned below to build your SDK:

1. Open eclipse in the Go language perspective and click on the ```Import``` option in ```File``` menu.

![Importing SDK into Eclipse - Step 1](https://apidocs.io/illustration/go?step=import0)

2. Select ```General -> Existing Projects into Workspace``` option from the tree list.

![Importing SDK into Eclipse - Step 2](https://apidocs.io/illustration/go?step=import1)

3. In ```Select root directory```, provide path to the unzipped archive for the generated code. Once the path is set and the Project becomes visible under ```Projects``` click ```Finish```

![Importing SDK into Eclipse - Step 3](https://apidocs.io/illustration/go?step=import2&workspaceFolder=Tester-GoLang&projectName=tester_lib)

4. The Go library will be imported and its files will be visible in the Project Explorer

![Importing SDK into Eclipse - Step 4](https://apidocs.io/illustration/go?step=import3&projectName=tester_lib)

## How to Use

The following section explains how to use the TesterLib library in a new project.

### 1. Add a new Test Project

Create a new project in Eclipse by ```File``` -> ```New``` -> ```Go Project```

![Add a new project in Eclipse](https://apidocs.io/illustration/go?step=createNewProject0)

Name the Project as ```Test``` and click ```Finish```

![Create a new Maven Project - Step 1](https://apidocs.io/illustration/go?step=createNewProject1)

Create a new directory in the ```src``` directory of this project

![Create a new Maven Project - Step 2](https://apidocs.io/illustration/go?step=createNewProject2&projectName=tester_lib)

Name it ```test.com```

![Create a new Maven Project - Step 3](https://apidocs.io/illustration/go?step=createNewProject3&projectName=tester_lib)

Now create a new file inside ```src/test.com```

![Create a new Maven Project - Step 4](https://apidocs.io/illustration/go?step=createNewProject4&projectName=tester_lib)

Name it ```testsdk.go```

![Create a new Maven Project - Step 5](https://apidocs.io/illustration/go?step=createNewProject5&projectName=tester_lib)

In this Go file, you can start adding code to initialize the client library. Sample code to initialize the client library and using its methods is given in the subsequent sections.

### 2. Configure the Test Project

You need to import your generated library in this project in order to make use of its functions. In order to import the library, you can add its path in the ```GOPATH``` for this project. Follow the below steps:

Right click on the project name and click on ```Properties```

![Adding dependency to the client library - Step 1](https://apidocs.io/illustration/go?step=testProject0&projectName=tester_lib)

Choose ```Go Compiler``` from the side menu. Check ```Use project specific settings``` and uncheck ```Use same value as the GOPATH environment variable.```. By default, the GOPATH value from the environment variables will be visible in ```Eclipse GOPATH```. Do not remove this as this points to the unirest dependency.

![Adding dependency to the client library - Step 2](https://apidocs.io/illustration/go?step=testProject1)

Append the library path to this GOPATH

![Adding dependency to the client library - Step 3](https://apidocs.io/illustration/go?step=testProject2&workspaceFolder=Tester-GoLang)

Once the path is appended, click on ```OK```

### 3. Build the Test Project

Right click on the project name and click on ```Build Project```

![Build Project](https://apidocs.io/illustration/go?step=buildProject&projectName=tester_lib)

### 4. Run the Test Project

If the build is successful, right click on your Go file and click on ```Run As``` -> ```Go Application```

![Run Project](https://apidocs.io/illustration/go?step=runProject&projectName=tester_lib)

## Initialization

### 
You need the following information for initializing the API client.

| Parameter | Description |
|-----------|-------------|
| suites | TODO: add a description |


To configure these for your generated code, open the file "Configuration.go" and edit it's contents.


# Class Reference

## <a name="list_of_controllers"></a>List of Controllers

* [responsetypes_pkg](#responsetypes_pkg)
* [bodyparams_pkg](#bodyparams_pkg)
* [formparams_pkg](#formparams_pkg)
* [queryparam_pkg](#queryparam_pkg)
* [errorcodes_pkg](#errorcodes_pkg)
* [echo_pkg](#echo_pkg)
* [header_pkg](#header_pkg)
* [templateparams_pkg](#templateparams_pkg)

## <a name="responsetypes_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".responsetypes_pkg") responsetypes_pkg

### Get instance

Factory for the ``` RESPONSETYPES ``` interface can be accessed from the package responsetypes_pkg.

```go
responseTypes := responsetypes_pkg.NewRESPONSETYPES()
```

### <a name="get_date_array"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.GetDateArray") GetDateArray

> TODO: Add a method description


```go
func (me *RESPONSETYPES_IMPL) GetDateArray()([]*time.Time,error)
```

#### Example Usage

```go

var result []*time.Time
result,_ = responseTypes.GetDateArray()

```


### <a name="get_date"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.GetDate") GetDate

> TODO: Add a method description


```go
func (me *RESPONSETYPES_IMPL) GetDate()(*time.Time,error)
```

#### Example Usage

```go

var result *time.Time
result,_ = responseTypes.GetDate()

```


### <a name="get_long"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.GetLong") GetLong

> TODO: Add a method description


```go
func (me *RESPONSETYPES_IMPL) GetLong()(*int64,error)
```

#### Example Usage

```go

var result *int64
result,_ = responseTypes.GetLong()

```


### <a name="get_model"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.GetModel") GetModel

> TODO: Add a method description


```go
func (me *RESPONSETYPES_IMPL) GetModel()(*models_pkg.Person,error)
```

#### Example Usage

```go

var result *models_pkg.Person
result,_ = responseTypes.GetModel()

```


### <a name="get_string_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.GetStringEnumArray") GetStringEnumArray

> TODO: Add a method description


```go
func (me *RESPONSETYPES_IMPL) GetStringEnumArray()([]models_pkg.Days,error)
```

#### Example Usage

```go

var result []models_pkg.Days
result,_ = responseTypes.GetStringEnumArray()

```


### <a name="get_string_enum"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.GetStringEnum") GetStringEnum

> TODO: Add a method description


```go
func (me *RESPONSETYPES_IMPL) GetStringEnum()(models_pkg.Days,error)
```

#### Example Usage

```go

var result models_pkg.Days
result,_ = responseTypes.GetStringEnum()

```


### <a name="get_model_array"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.GetModelArray") GetModelArray

> TODO: Add a method description


```go
func (me *RESPONSETYPES_IMPL) GetModelArray()([]*models_pkg.Person,error)
```

#### Example Usage

```go

var result []*models_pkg.Person
result,_ = responseTypes.GetModelArray()

```


### <a name="get_int_enum"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.GetIntEnum") GetIntEnum

> TODO: Add a method description


```go
func (me *RESPONSETYPES_IMPL) GetIntEnum()(models_pkg.SuiteCode,error)
```

#### Example Usage

```go

var result models_pkg.SuiteCode
result,_ = responseTypes.GetIntEnum()

```


### <a name="get_int_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.GetIntEnumArray") GetIntEnumArray

> TODO: Add a method description


```go
func (me *RESPONSETYPES_IMPL) GetIntEnumArray()([]models_pkg.SuiteCode,error)
```

#### Example Usage

```go

var result []models_pkg.SuiteCode
result,_ = responseTypes.GetIntEnumArray()

```


### <a name="get_precision"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.GetPrecision") GetPrecision

> TODO: Add a method description


```go
func (me *RESPONSETYPES_IMPL) GetPrecision()(*float64,error)
```

#### Example Usage

```go

var result *float64
result,_ = responseTypes.GetPrecision()

```


### <a name="get_binary"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.GetBinary") GetBinary

> gets a binary object


```go
func (me *RESPONSETYPES_IMPL) GetBinary()([]byte,error)
```

#### Example Usage

```go

var result []byte
result,_ = responseTypes.GetBinary()

```


### <a name="get_integer"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.GetInteger") GetInteger

> Gets a integer response


```go
func (me *RESPONSETYPES_IMPL) GetInteger()(*int64,error)
```

#### Example Usage

```go

var result *int64
result,_ = responseTypes.GetInteger()

```


### <a name="get_integer_array"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.GetIntegerArray") GetIntegerArray

> Get an array of integers.


```go
func (me *RESPONSETYPES_IMPL) GetIntegerArray()([]int64,error)
```

#### Example Usage

```go

var result []int64
result,_ = responseTypes.GetIntegerArray()

```


### <a name="get_dynamic"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.GetDynamic") GetDynamic

> TODO: Add a method description


```go
func (me *RESPONSETYPES_IMPL) GetDynamic()(interface{},error)
```

#### Example Usage

```go

var result interface{}
result,_ = responseTypes.GetDynamic()

```


### <a name="get_dynamic_array"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.GetDynamicArray") GetDynamicArray

> TODO: Add a method description


```go
func (me *RESPONSETYPES_IMPL) GetDynamicArray()(interface{},error)
```

#### Example Usage

```go

var result interface{}
result,_ = responseTypes.GetDynamicArray()

```


### <a name="get3339_datetime"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.Get3339Datetime") Get3339Datetime

> TODO: Add a method description


```go
func (me *RESPONSETYPES_IMPL) Get3339Datetime()(*time.Time,error)
```

#### Example Usage

```go

var result *time.Time
result,_ = responseTypes.Get3339Datetime()

```


### <a name="get3339_datetime_array"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.Get3339DatetimeArray") Get3339DatetimeArray

> TODO: Add a method description


```go
func (me *RESPONSETYPES_IMPL) Get3339DatetimeArray()([]*time.Time,error)
```

#### Example Usage

```go

var result []*time.Time
result,_ = responseTypes.Get3339DatetimeArray()

```


### <a name="get_boolean"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.GetBoolean") GetBoolean

> TODO: Add a method description


```go
func (me *RESPONSETYPES_IMPL) GetBoolean()(*bool,error)
```

#### Example Usage

```go

var result *bool
result,_ = responseTypes.GetBoolean()

```


### <a name="get_boolean_array"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.GetBooleanArray") GetBooleanArray

> TODO: Add a method description


```go
func (me *RESPONSETYPES_IMPL) GetBooleanArray()([]bool,error)
```

#### Example Usage

```go

var result []bool
result,_ = responseTypes.GetBooleanArray()

```


### <a name="get_headers"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.GetHeaders") GetHeaders

> TODO: Add a method description


```go
func (me *RESPONSETYPES_IMPL) GetHeaders()(,error)
```

#### Example Usage

```go

var result 
result,_ = responseTypes.GetHeaders()

```


### <a name="get1123_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.Get1123DateTime") Get1123DateTime

> TODO: Add a method description


```go
func (me *RESPONSETYPES_IMPL) Get1123DateTime()(*time.Time,error)
```

#### Example Usage

```go

var result *time.Time
result,_ = responseTypes.Get1123DateTime()

```


### <a name="get_unix_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.GetUnixDateTime") GetUnixDateTime

> TODO: Add a method description


```go
func (me *RESPONSETYPES_IMPL) GetUnixDateTime()(*time.Time,error)
```

#### Example Usage

```go

var result *time.Time
result,_ = responseTypes.GetUnixDateTime()

```


### <a name="get1123_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.Get1123DateTimeArray") Get1123DateTimeArray

> TODO: Add a method description


```go
func (me *RESPONSETYPES_IMPL) Get1123DateTimeArray()([]*time.Time,error)
```

#### Example Usage

```go

var result []*time.Time
result,_ = responseTypes.Get1123DateTimeArray()

```


### <a name="get_unix_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".responsetypes_pkg.GetUnixDateTimeArray") GetUnixDateTimeArray

> TODO: Add a method description


```go
func (me *RESPONSETYPES_IMPL) GetUnixDateTimeArray()([]*time.Time,error)
```

#### Example Usage

```go

var result []*time.Time
result,_ = responseTypes.GetUnixDateTimeArray()

```


[Back to List of Controllers](#list_of_controllers)

## <a name="bodyparams_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".bodyparams_pkg") bodyparams_pkg

### Get instance

Factory for the ``` BODYPARAMS ``` interface can be accessed from the package bodyparams_pkg.

```go
bodyParams := bodyparams_pkg.NewBODYPARAMS()
```

### <a name="send_date_array"></a>![Method: ](https://apidocs.io/img/method.png ".bodyparams_pkg.SendDateArray") SendDateArray

> TODO: Add a method description


```go
func (me *BODYPARAMS_IMPL) SendDateArray(dates []*time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dates |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
datesValue := []byte("[\"1994-02-13\", \"1994-02-13\"]")
var dates []*time.Time
json.Unmarshal(datesValue,&dates)

var result *models_pkg.ServerResponse
result,_ = bodyParams.SendDateArray(dates)

```


### <a name="send_date"></a>![Method: ](https://apidocs.io/img/method.png ".bodyparams_pkg.SendDate") SendDate

> TODO: Add a method description


```go
func (me *BODYPARAMS_IMPL) SendDate(date *time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| date |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
date := "1994-02-13"

var result *models_pkg.ServerResponse
result,_ = bodyParams.SendDate(date)

```


### <a name="send_unix_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".bodyparams_pkg.SendUnixDateTime") SendUnixDateTime

> TODO: Add a method description


```go
func (me *BODYPARAMS_IMPL) SendUnixDateTime(datetime *time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
datetime := "1484719381"

var result *models_pkg.ServerResponse
result,_ = bodyParams.SendUnixDateTime(datetime)

```


### <a name="send_rfc1123_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".bodyparams_pkg.SendRfc1123DateTime") SendRfc1123DateTime

> TODO: Add a method description


```go
func (me *BODYPARAMS_IMPL) SendRfc1123DateTime(datetime *time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
datetime := "Sun, 06 Nov 1994 08:49:37 GMT"

var result *models_pkg.ServerResponse
result,_ = bodyParams.SendRfc1123DateTime(datetime)

```


### <a name="send_rfc3339_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".bodyparams_pkg.SendRfc3339DateTime") SendRfc3339DateTime

> TODO: Add a method description


```go
func (me *BODYPARAMS_IMPL) SendRfc3339DateTime(datetime *time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
datetime := "1994-02-13T14:01:54.9571247Z"

var result *models_pkg.ServerResponse
result,_ = bodyParams.SendRfc3339DateTime(datetime)

```


### <a name="send_unix_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".bodyparams_pkg.SendUnixDateTimeArray") SendUnixDateTimeArray

> TODO: Add a method description


```go
func (me *BODYPARAMS_IMPL) SendUnixDateTimeArray(datetimes []*time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
datetimesValue := []byte("[1484719381,1484719381]")
var datetimes []*time.Time
json.Unmarshal(datetimesValue,&datetimes)

var result *models_pkg.ServerResponse
result,_ = bodyParams.SendUnixDateTimeArray(datetimes)

```


### <a name="send_rfc1123_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".bodyparams_pkg.SendRfc1123DateTimeArray") SendRfc1123DateTimeArray

> TODO: Add a method description


```go
func (me *BODYPARAMS_IMPL) SendRfc1123DateTimeArray(datetimes []*time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
datetimesValue := []byte("[\"Sun, 06 Nov 1994 08:49:37 GMT\",\"Sun, 06 Nov 1994 08:49:37 GMT\"]")
var datetimes []*time.Time
json.Unmarshal(datetimesValue,&datetimes)

var result *models_pkg.ServerResponse
result,_ = bodyParams.SendRfc1123DateTimeArray(datetimes)

```


### <a name="send_rfc3339_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".bodyparams_pkg.SendRfc3339DateTimeArray") SendRfc3339DateTimeArray

> TODO: Add a method description


```go
func (me *BODYPARAMS_IMPL) SendRfc3339DateTimeArray(datetimes []*time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
datetimesValue := []byte("[\"1994-02-13T14:01:54.9571247Z\",\"1994-02-13T14:01:54.9571247Z\"]")
var datetimes []*time.Time
json.Unmarshal(datetimesValue,&datetimes)

var result *models_pkg.ServerResponse
result,_ = bodyParams.SendRfc3339DateTimeArray(datetimes)

```


### <a name="send_string_array"></a>![Method: ](https://apidocs.io/img/method.png ".bodyparams_pkg.SendStringArray") SendStringArray

> sends a string body param


```go
func (me *BODYPARAMS_IMPL) SendStringArray(sarray []string)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| sarray |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
sarrayValue := []byte("[\"abc\", \"def\"]")
var sarray []string
json.Unmarshal(sarrayValue,&sarray)

var result *models_pkg.ServerResponse
result,_ = bodyParams.SendStringArray(sarray)

```


### <a name="send_integer_array"></a>![Method: ](https://apidocs.io/img/method.png ".bodyparams_pkg.SendIntegerArray") SendIntegerArray

> TODO: Add a method description


```go
func (me *BODYPARAMS_IMPL) SendIntegerArray(integers []int64)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
integersValue := []byte("[1,2,3,4,5]")
var integers []int64
json.Unmarshal(integersValue,&integers)

var result *models_pkg.ServerResponse
result,_ = bodyParams.SendIntegerArray(integers)

```


### <a name="send_model"></a>![Method: ](https://apidocs.io/img/method.png ".bodyparams_pkg.SendModel") SendModel

> TODO: Add a method description


```go
func (me *BODYPARAMS_IMPL) SendModel(model *models_pkg.Employee)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| model |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
modelValue := []byte("{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}")
var model *models_pkg.Employee
json.Unmarshal(modelValue,&model)

var result *models_pkg.ServerResponse
result,_ = bodyParams.SendModel(model)

```


### <a name="send_model_array"></a>![Method: ](https://apidocs.io/img/method.png ".bodyparams_pkg.SendModelArray") SendModelArray

> TODO: Add a method description


```go
func (me *BODYPARAMS_IMPL) SendModelArray(models []*models_pkg.Employee)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| models |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
modelsValue := []byte("[{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"},{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}]")
var models []*models_pkg.Employee
json.Unmarshal(modelsValue,&models)

var result *models_pkg.ServerResponse
result,_ = bodyParams.SendModelArray(models)

```


### <a name="send_dynamic"></a>![Method: ](https://apidocs.io/img/method.png ".bodyparams_pkg.SendDynamic") SendDynamic

> TODO: Add a method description


```go
func (me *BODYPARAMS_IMPL) SendDynamic(dynamic interface{})(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dynamic |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
dynamicValue := []byte("{\"uid\": \"1123213\", \"name\": \"Shahid\"}")
var dynamic interface{}
json.Unmarshal(dynamicValue,&dynamic)

var result *models_pkg.ServerResponse
result,_ = bodyParams.SendDynamic(dynamic)

```


### <a name="send_string"></a>![Method: ](https://apidocs.io/img/method.png ".bodyparams_pkg.SendString") SendString

> TODO: Add a method description


```go
func (me *BODYPARAMS_IMPL) SendString(value string)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| value |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
value := "TestString"

var result *models_pkg.ServerResponse
result,_ = bodyParams.SendString(value)

```


### <a name="send_string_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".bodyparams_pkg.SendStringEnumArray") SendStringEnumArray

> TODO: Add a method description


```go
func (me *BODYPARAMS_IMPL) SendStringEnumArray(days []models_pkg.Days)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| days |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
days := []models_pkg.Days{models_pkg.Days_TUESDAY,models_pkg.Days_SATURDAY,models_pkg.Days_MONDAY,models_pkg.Days_SUNDAY}

var result *models_pkg.ServerResponse
result,_ = bodyParams.SendStringEnumArray(days)

```


### <a name="send_integer_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".bodyparams_pkg.SendIntegerEnumArray") SendIntegerEnumArray

> TODO: Add a method description


```go
func (me *BODYPARAMS_IMPL) SendIntegerEnumArray(suites []models_pkg.SuiteCode)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| suites |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
suites := []models_pkg.SuiteCode{models_pkg.SuiteCode_HEARTS,models_pkg.SuiteCode_CLUBS,models_pkg.SuiteCode_DIAMONDS,models_pkg.SuiteCode_SPADES,models_pkg.SuiteCode_CLUBS}

var result *models_pkg.ServerResponse
result,_ = bodyParams.SendIntegerEnumArray(suites)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="formparams_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".formparams_pkg") formparams_pkg

### Get instance

Factory for the ``` FORMPARAMS ``` interface can be accessed from the package formparams_pkg.

```go
formParams := formparams_pkg.NewFORMPARAMS()
```

### <a name="send_date_array"></a>![Method: ](https://apidocs.io/img/method.png ".formparams_pkg.SendDateArray") SendDateArray

> TODO: Add a method description


```go
func (me *FORMPARAMS_IMPL) SendDateArray(dates []*time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dates |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
datesValue := []byte("[\"1994-02-13\",\"1994-02-13\"]")
var dates []*time.Time
json.Unmarshal(datesValue,&dates)

var result *models_pkg.ServerResponse
result,_ = formParams.SendDateArray(dates)

```


### <a name="send_date"></a>![Method: ](https://apidocs.io/img/method.png ".formparams_pkg.SendDate") SendDate

> TODO: Add a method description


```go
func (me *FORMPARAMS_IMPL) SendDate(date *time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| date |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
date := "1994-02-13"

var result *models_pkg.ServerResponse
result,_ = formParams.SendDate(date)

```


### <a name="send_unix_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".formparams_pkg.SendUnixDateTime") SendUnixDateTime

> TODO: Add a method description


```go
func (me *FORMPARAMS_IMPL) SendUnixDateTime(datetime *time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
datetime := "1484719381"

var result *models_pkg.ServerResponse
result,_ = formParams.SendUnixDateTime(datetime)

```


### <a name="send_rfc1123_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".formparams_pkg.SendRfc1123DateTime") SendRfc1123DateTime

> TODO: Add a method description


```go
func (me *FORMPARAMS_IMPL) SendRfc1123DateTime(datetime *time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
datetime := "Sun, 06 Nov 1994 08:49:37 GMT"

var result *models_pkg.ServerResponse
result,_ = formParams.SendRfc1123DateTime(datetime)

```


### <a name="send_rfc3339_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".formparams_pkg.SendRfc3339DateTime") SendRfc3339DateTime

> TODO: Add a method description


```go
func (me *FORMPARAMS_IMPL) SendRfc3339DateTime(datetime *time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
datetime := "1994-02-13T14:01:54.9571247Z"

var result *models_pkg.ServerResponse
result,_ = formParams.SendRfc3339DateTime(datetime)

```


### <a name="send_unix_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".formparams_pkg.SendUnixDateTimeArray") SendUnixDateTimeArray

> TODO: Add a method description


```go
func (me *FORMPARAMS_IMPL) SendUnixDateTimeArray(datetimes []*time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
datetimesValue := []byte("[1484719381,1484719381]")
var datetimes []*time.Time
json.Unmarshal(datetimesValue,&datetimes)

var result *models_pkg.ServerResponse
result,_ = formParams.SendUnixDateTimeArray(datetimes)

```


### <a name="send_rfc1123_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".formparams_pkg.SendRfc1123DateTimeArray") SendRfc1123DateTimeArray

> TODO: Add a method description


```go
func (me *FORMPARAMS_IMPL) SendRfc1123DateTimeArray(datetimes []*time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
datetimesValue := []byte("[\"Sun, 06 Nov 1994 08:49:37 GMT\",\"Sun, 06 Nov 1994 08:49:37 GMT\"]")
var datetimes []*time.Time
json.Unmarshal(datetimesValue,&datetimes)

var result *models_pkg.ServerResponse
result,_ = formParams.SendRfc1123DateTimeArray(datetimes)

```


### <a name="send_long"></a>![Method: ](https://apidocs.io/img/method.png ".formparams_pkg.SendLong") SendLong

> TODO: Add a method description


```go
func (me *FORMPARAMS_IMPL) SendLong(value int64)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| value |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
value,_ := strconv.ParseInt("5147483647", 10, 8)

var result *models_pkg.ServerResponse
result,_ = formParams.SendLong(value)

```


### <a name="send_integer_array"></a>![Method: ](https://apidocs.io/img/method.png ".formparams_pkg.SendIntegerArray") SendIntegerArray

> TODO: Add a method description


```go
func (me *FORMPARAMS_IMPL) SendIntegerArray(integers []int64)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
integersValue := []byte("[1,2,3,4,5]")
var integers []int64
json.Unmarshal(integersValue,&integers)

var result *models_pkg.ServerResponse
result,_ = formParams.SendIntegerArray(integers)

```


### <a name="send_string_array"></a>![Method: ](https://apidocs.io/img/method.png ".formparams_pkg.SendStringArray") SendStringArray

> TODO: Add a method description


```go
func (me *FORMPARAMS_IMPL) SendStringArray(strings []string)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
stringsValue := []byte("[\"abc\", \"def\"]")
var strings []string
json.Unmarshal(stringsValue,&strings)

var result *models_pkg.ServerResponse
result,_ = formParams.SendStringArray(strings)

```


### <a name="send_model"></a>![Method: ](https://apidocs.io/img/method.png ".formparams_pkg.SendModel") SendModel

> TODO: Add a method description


```go
func (me *FORMPARAMS_IMPL) SendModel(model *models_pkg.Employee)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| model |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
modelValue := []byte("{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}")
var model *models_pkg.Employee
json.Unmarshal(modelValue,&model)

var result *models_pkg.ServerResponse
result,_ = formParams.SendModel(model)

```


### <a name="send_model_array"></a>![Method: ](https://apidocs.io/img/method.png ".formparams_pkg.SendModelArray") SendModelArray

> TODO: Add a method description


```go
func (me *FORMPARAMS_IMPL) SendModelArray(models []*models_pkg.Employee)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| models |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
modelsValue := []byte("[{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"},{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}]")
var models []*models_pkg.Employee
json.Unmarshal(modelsValue,&models)

var result *models_pkg.ServerResponse
result,_ = formParams.SendModelArray(models)

```


### <a name="send_file"></a>![Method: ](https://apidocs.io/img/method.png ".formparams_pkg.SendFile") SendFile

> TODO: Add a method description


```go
func (me *FORMPARAMS_IMPL) SendFile(file []byte)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
file := []byte("http://localhost:3000/response/image")

var result *models_pkg.ServerResponse
result,_ = formParams.SendFile(file)

```


### <a name="send_string"></a>![Method: ](https://apidocs.io/img/method.png ".formparams_pkg.SendString") SendString

> TODO: Add a method description


```go
func (me *FORMPARAMS_IMPL) SendString(value string)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| value |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
value := "TestString"

var result *models_pkg.ServerResponse
result,_ = formParams.SendString(value)

```


### <a name="send_rfc3339_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".formparams_pkg.SendRfc3339DateTimeArray") SendRfc3339DateTimeArray

> TODO: Add a method description


```go
func (me *FORMPARAMS_IMPL) SendRfc3339DateTimeArray(datetimes []*time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
datetimesValue := []byte("[\"1994-02-13T14:01:54.9571247Z\",\"1994-02-13T14:01:54.9571247Z\"]")
var datetimes []*time.Time
json.Unmarshal(datetimesValue,&datetimes)

var result *models_pkg.ServerResponse
result,_ = formParams.SendRfc3339DateTimeArray(datetimes)

```


### <a name="send_mixed_array"></a>![Method: ](https://apidocs.io/img/method.png ".formparams_pkg.SendMixedArray") SendMixedArray

> Send a variety for form params. Returns file count and body params


```go
func (me *FORMPARAMS_IMPL) SendMixedArray(input *SendMixedArrayInput)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | TODO: Add a parameter description |
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |
| models |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
collect := new (formparams_pkg.SendMixedArrayInput)

file := []byte("http://localhost:3000/response/image")
collect.File = file

integersValue := []byte("[1,2,3,4,5]")
var integers []int64
json.Unmarshal(integersValue,&integers)
collect.Integers = integers

modelsValue := []byte("[{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"},{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}]")
var models []*models_pkg.Employee
json.Unmarshal(modelsValue,&models)
collect.Models = models

stringsValue := []byte("[\"abc\", \"def\"]")
var strings []string
json.Unmarshal(stringsValue,&strings)
collect.Strings = strings


var result *models_pkg.ServerResponse
result,_ = formParams.SendMixedArray(collect)

```


### <a name="send_integer_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".formparams_pkg.SendIntegerEnumArray") SendIntegerEnumArray

> TODO: Add a method description


```go
func (me *FORMPARAMS_IMPL) SendIntegerEnumArray(suites []models_pkg.SuiteCode)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| suites |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
suites := []models_pkg.SuiteCode{models_pkg.SuiteCode_HEARTS,models_pkg.SuiteCode_CLUBS,models_pkg.SuiteCode_DIAMONDS,models_pkg.SuiteCode_SPADES,models_pkg.SuiteCode_CLUBS}

var result *models_pkg.ServerResponse
result,_ = formParams.SendIntegerEnumArray(suites)

```


### <a name="send_string_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".formparams_pkg.SendStringEnumArray") SendStringEnumArray

> TODO: Add a method description


```go
func (me *FORMPARAMS_IMPL) SendStringEnumArray(days []models_pkg.Days)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| days |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
days := []models_pkg.Days{models_pkg.Days_TUESDAY,models_pkg.Days_SATURDAY,models_pkg.Days_MONDAY,models_pkg.Days_SUNDAY}

var result *models_pkg.ServerResponse
result,_ = formParams.SendStringEnumArray(days)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="queryparam_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".queryparam_pkg") queryparam_pkg

### Get instance

Factory for the ``` QUERYPARAM ``` interface can be accessed from the package queryparam_pkg.

```go
queryParam := queryparam_pkg.NewQUERYPARAM()
```

### <a name="date_array"></a>![Method: ](https://apidocs.io/img/method.png ".queryparam_pkg.DateArray") DateArray

> TODO: Add a method description


```go
func (me *QUERYPARAM_IMPL) DateArray(dates []*time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dates |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
datesValue := []byte("[\"1994-02-13\",\"1994-02-13\"]")
var dates []*time.Time
json.Unmarshal(datesValue,&dates)

var result *models_pkg.ServerResponse
result,_ = queryParam.DateArray(dates)

```


### <a name="date"></a>![Method: ](https://apidocs.io/img/method.png ".queryparam_pkg.Date") Date

> TODO: Add a method description


```go
func (me *QUERYPARAM_IMPL) Date(date *time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| date |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
date := "1994-02-13"

var result *models_pkg.ServerResponse
result,_ = queryParam.Date(date)

```


### <a name="unix_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".queryparam_pkg.UnixDateTimeArray") UnixDateTimeArray

> TODO: Add a method description


```go
func (me *QUERYPARAM_IMPL) UnixDateTimeArray(datetimes []*time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
datetimesValue := []byte("[1484719381,1484719381]")
var datetimes []*time.Time
json.Unmarshal(datetimesValue,&datetimes)

var result *models_pkg.ServerResponse
result,_ = queryParam.UnixDateTimeArray(datetimes)

```


### <a name="unix_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".queryparam_pkg.UnixDateTime") UnixDateTime

> TODO: Add a method description


```go
func (me *QUERYPARAM_IMPL) UnixDateTime(datetime *time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
datetime := "1484719381"

var result *models_pkg.ServerResponse
result,_ = queryParam.UnixDateTime(datetime)

```


### <a name="rfc1123_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".queryparam_pkg.Rfc1123DateTime") Rfc1123DateTime

> TODO: Add a method description


```go
func (me *QUERYPARAM_IMPL) Rfc1123DateTime(datetime *time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
datetime := "Sun, 06 Nov 1994 08:49:37 GMT"

var result *models_pkg.ServerResponse
result,_ = queryParam.Rfc1123DateTime(datetime)

```


### <a name="rfc1123_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".queryparam_pkg.Rfc1123DateTimeArray") Rfc1123DateTimeArray

> TODO: Add a method description


```go
func (me *QUERYPARAM_IMPL) Rfc1123DateTimeArray(datetimes []*time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
datetimesValue := []byte("[\"Sun, 06 Nov 1994 08:49:37 GMT\",\"Sun, 06 Nov 1994 08:49:37 GMT\"]")
var datetimes []*time.Time
json.Unmarshal(datetimesValue,&datetimes)

var result *models_pkg.ServerResponse
result,_ = queryParam.Rfc1123DateTimeArray(datetimes)

```


### <a name="rfc3339_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".queryparam_pkg.Rfc3339DateTimeArray") Rfc3339DateTimeArray

> TODO: Add a method description


```go
func (me *QUERYPARAM_IMPL) Rfc3339DateTimeArray(datetimes []*time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
datetimesValue := []byte("[\"1994-02-13T14:01:54.9571247Z\",\"1994-02-13T14:01:54.9571247Z\"]")
var datetimes []*time.Time
json.Unmarshal(datetimesValue,&datetimes)

var result *models_pkg.ServerResponse
result,_ = queryParam.Rfc3339DateTimeArray(datetimes)

```


### <a name="rfc3339_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".queryparam_pkg.Rfc3339DateTime") Rfc3339DateTime

> TODO: Add a method description


```go
func (me *QUERYPARAM_IMPL) Rfc3339DateTime(datetime *time.Time)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
datetime := "1994-02-13T14:01:54.9571247Z"

var result *models_pkg.ServerResponse
result,_ = queryParam.Rfc3339DateTime(datetime)

```


### <a name="no_params"></a>![Method: ](https://apidocs.io/img/method.png ".queryparam_pkg.NoParams") NoParams

> TODO: Add a method description


```go
func (me *QUERYPARAM_IMPL) NoParams()(*models_pkg.ServerResponse,error)
```

#### Example Usage

```go

var result *models_pkg.ServerResponse
result,_ = queryParam.NoParams()

```


### <a name="string_param"></a>![Method: ](https://apidocs.io/img/method.png ".queryparam_pkg.StringParam") StringParam

> TODO: Add a method description


```go
func (me *QUERYPARAM_IMPL) StringParam(mstring string)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mstring |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
mstring := "l;asd;asdwe[2304&&;'.d??\\a\\\\\\;sd//"

var result *models_pkg.ServerResponse
result,_ = queryParam.StringParam(mstring)

```


### <a name="url_param"></a>![Method: ](https://apidocs.io/img/method.png ".queryparam_pkg.UrlParam") UrlParam

> TODO: Add a method description


```go
func (me *QUERYPARAM_IMPL) UrlParam(url string)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| url |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
url := "https://www.shahidisawesome.com/and/also/a/narcissist?thisis=aparameter&another=one"

var result *models_pkg.ServerResponse
result,_ = queryParam.UrlParam(url)

```


### <a name="number_array"></a>![Method: ](https://apidocs.io/img/method.png ".queryparam_pkg.NumberArray") NumberArray

> TODO: Add a method description


```go
func (me *QUERYPARAM_IMPL) NumberArray(integers []int64)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
integersValue := []byte("[1,2,3,4,5]")
var integers []int64
json.Unmarshal(integersValue,&integers)

var result *models_pkg.ServerResponse
result,_ = queryParam.NumberArray(integers)

```


### <a name="string_array"></a>![Method: ](https://apidocs.io/img/method.png ".queryparam_pkg.StringArray") StringArray

> TODO: Add a method description


```go
func (me *QUERYPARAM_IMPL) StringArray(strings []string)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
stringsValue := []byte("[\"abc\", \"def\"]")
var strings []string
json.Unmarshal(stringsValue,&strings)

var result *models_pkg.ServerResponse
result,_ = queryParam.StringArray(strings)

```


### <a name="simple_query"></a>![Method: ](https://apidocs.io/img/method.png ".queryparam_pkg.SimpleQuery") SimpleQuery

> TODO: Add a method description


```go
func (me *QUERYPARAM_IMPL) SimpleQuery(
            boolean bool,
            number int64,
            mstring string,
                queryParameters map[string]interface{})(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| boolean |  ``` Required ```  | TODO: Add a parameter description |
| number |  ``` Required ```  | TODO: Add a parameter description |
| mstring |  ``` Required ```  | TODO: Add a parameter description |
| queryParameters | ``` Optional ``` | Additional optional query parameters are supported by this method |


#### Example Usage

```go
boolean := true
number,_ := strconv.ParseInt("4", 10, 8)
mstring := "TestString"
// key-value map for optional query parameters
	queryParams := map[string]interface{}{"key" : "value"}


var result *models_pkg.ServerResponse
result,_ = queryParam.SimpleQuery(boolean, number, mstring, queryParams)

```


### <a name="string_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".queryparam_pkg.StringEnumArray") StringEnumArray

> TODO: Add a method description


```go
func (me *QUERYPARAM_IMPL) StringEnumArray(days []models_pkg.Days)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| days |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
days := []models_pkg.Days{models_pkg.Days_TUESDAY,models_pkg.Days_SATURDAY,models_pkg.Days_MONDAY,models_pkg.Days_SUNDAY}

var result *models_pkg.ServerResponse
result,_ = queryParam.StringEnumArray(days)

```


### <a name="multiple_params"></a>![Method: ](https://apidocs.io/img/method.png ".queryparam_pkg.MultipleParams") MultipleParams

> TODO: Add a method description


```go
func (me *QUERYPARAM_IMPL) MultipleParams(
            number int64,
            precision float64,
            mstring string,
            url string)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| number |  ``` Required ```  | TODO: Add a parameter description |
| precision |  ``` Required ```  | TODO: Add a parameter description |
| mstring |  ``` Required ```  | TODO: Add a parameter description |
| url |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
number,_ := strconv.ParseInt("123412312", 10, 8)
precision := "1112.34"
mstring := "\"\"test./;\";12&&3asl\"\";\"qw1&34\"///..//."
url := "http://www.abc.com/test?a=b&c=\"http://lolol.com?param=no&another=lol\""

var result *models_pkg.ServerResponse
result,_ = queryParam.MultipleParams(number, precision, mstring, url)

```


### <a name="integer_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".queryparam_pkg.IntegerEnumArray") IntegerEnumArray

> TODO: Add a method description


```go
func (me *QUERYPARAM_IMPL) IntegerEnumArray(suites []models_pkg.SuiteCode)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| suites |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
suites := []models_pkg.SuiteCode{models_pkg.SuiteCode_HEARTS,models_pkg.SuiteCode_CLUBS,models_pkg.SuiteCode_DIAMONDS,models_pkg.SuiteCode_SPADES,models_pkg.SuiteCode_CLUBS}

var result *models_pkg.ServerResponse
result,_ = queryParam.IntegerEnumArray(suites)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="errorcodes_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".errorcodes_pkg") errorcodes_pkg

### Get instance

Factory for the ``` ERRORCODES ``` interface can be accessed from the package errorcodes_pkg.

```go
errorCodes := errorcodes_pkg.NewERRORCODES()
```

### <a name="get400"></a>![Method: ](https://apidocs.io/img/method.png ".errorcodes_pkg.Get400") Get400

> TODO: Add a method description


```go
func (me *ERRORCODES_IMPL) Get400()(interface{},error)
```

#### Example Usage

```go

var result interface{}
result,_ = errorCodes.Get400()

```


### <a name="get500"></a>![Method: ](https://apidocs.io/img/method.png ".errorcodes_pkg.Get500") Get500

> TODO: Add a method description


```go
func (me *ERRORCODES_IMPL) Get500()(interface{},error)
```

#### Example Usage

```go

var result interface{}
result,_ = errorCodes.Get500()

```


### <a name="get401"></a>![Method: ](https://apidocs.io/img/method.png ".errorcodes_pkg.Get401") Get401

> TODO: Add a method description


```go
func (me *ERRORCODES_IMPL) Get401()(interface{},error)
```

#### Example Usage

```go

var result interface{}
result,_ = errorCodes.Get401()

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

## <a name="echo_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".echo_pkg") echo_pkg

### Get instance

Factory for the ``` ECHO ``` interface can be accessed from the package echo_pkg.

```go
echo := echo_pkg.NewECHO()
```

### <a name="json_echo"></a>![Method: ](https://apidocs.io/img/method.png ".echo_pkg.JsonEcho") JsonEcho

> Echo's back the request


```go
func (me *ECHO_IMPL) JsonEcho(input interface{})(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| input |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
inputValue := []byte("{\"uid\": \"1123213\", \"name\": \"Shahid\"}")
var input interface{}
json.Unmarshal(inputValue,&input)

var result interface{}
result,_ = echo.JsonEcho(input)

```


### <a name="form_echo"></a>![Method: ](https://apidocs.io/img/method.png ".echo_pkg.FormEcho") FormEcho

> Sends the request including any form params as JSON


```go
func (me *ECHO_IMPL) FormEcho(input interface{})(interface{},error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| input |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```go
inputValue := []byte("{\"uid\": \"1123213\", \"name\": \"Shahid\"}")
var input interface{}
json.Unmarshal(inputValue,&input)

var result interface{}
result,_ = echo.FormEcho(input)

```


### <a name="query_echo"></a>![Method: ](https://apidocs.io/img/method.png ".echo_pkg.QueryEcho") QueryEcho

> TODO: Add a method description


```go
func (me *ECHO_IMPL) QueryEcho(queryParameters map[string]interface{})(*models_pkg.EchoResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| queryParameters | ``` Optional ``` | Additional optional query parameters are supported by this method |


#### Example Usage

```go
// key-value map for optional query parameters
	queryParams := map[string]interface{}{"key" : "value"}


var result *models_pkg.EchoResponse
result,_ = echo.QueryEcho(queryParams)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="header_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".header_pkg") header_pkg

### Get instance

Factory for the ``` HEADER ``` interface can be accessed from the package header_pkg.

```go
header := header_pkg.NewHEADER()
```

### <a name="send_headers"></a>![Method: ](https://apidocs.io/img/method.png ".header_pkg.SendHeaders") SendHeaders

> Sends a single header params


```go
func (me *HEADER_IMPL) SendHeaders(
            customHeader string,
            value string)(*models_pkg.ServerResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| customHeader |  ``` Required ```  | TODO: Add a parameter description |
| value |  ``` Required ```  | Represents the value of the custom header |


#### Example Usage

```go
customHeader := "TestString"
value := "TestString"

var result *models_pkg.ServerResponse
result,_ = header.SendHeaders(customHeader, value)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="templateparams_pkg"></a>![Class: ](https://apidocs.io/img/class.png ".templateparams_pkg") templateparams_pkg

### Get instance

Factory for the ``` TEMPLATEPARAMS ``` interface can be accessed from the package templateparams_pkg.

```go
templateParams := templateparams_pkg.NewTEMPLATEPARAMS()
```

### <a name="send_string_array"></a>![Method: ](https://apidocs.io/img/method.png ".templateparams_pkg.SendStringArray") SendStringArray

> TODO: Add a method description


```go
func (me *TEMPLATEPARAMS_IMPL) SendStringArray(strings []string)(*models_pkg.EchoResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
stringsValue := []byte("[\"abc\", \"def\"]")
var strings []string
json.Unmarshal(stringsValue,&strings)

var result *models_pkg.EchoResponse
result,_ = templateParams.SendStringArray(strings)

```


### <a name="send_integer_array"></a>![Method: ](https://apidocs.io/img/method.png ".templateparams_pkg.SendIntegerArray") SendIntegerArray

> TODO: Add a method description


```go
func (me *TEMPLATEPARAMS_IMPL) SendIntegerArray(integers []int64)(*models_pkg.EchoResponse,error)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```go
integersValue := []byte("[1,2,3,4,5]")
var integers []int64
json.Unmarshal(integersValue,&integers)

var result *models_pkg.EchoResponse
result,_ = templateParams.SendIntegerArray(integers)

```


[Back to List of Controllers](#list_of_controllers)



