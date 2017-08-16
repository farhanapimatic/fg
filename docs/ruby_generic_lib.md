# Getting started

Testing various
 api 
features

## How to Build

This client library is a Ruby gem which can be compiled and used in your Ruby and Ruby on Rails project. This library requires a few gems from the RubyGems repository.

1. Open the command line interface or the terminal and navigate to the folder containing the source code.
2. Run ``` gem build tester.gemspec ``` to build the gem.
3. Once built, the gem can be installed on the current work environment using ``` gem install tester-1.1.0.gem ```

![Building Gem](https://apidocs.io/illustration/ruby?step=buildSDK&workspaceFolder=Tester-Ruby&workspaceName=Tester-Ruby&projectName=tester&gemName=tester&gemVer=1.1.0)

## How to Use

The following section explains how to use the Tester Ruby Gem in a new Rails project using RubyMine&trade;. The basic workflow presented here is also applicable if you prefer using a different editor or IDE.

### 1. Starting a new project

Close any existing projects in RubyMine&trade; by selecting ``` File -> Close Project ```. Next, click on ``` Create New Project ``` to create a new project from scratch.

![Create a new project in RubyMine](https://apidocs.io/illustration/ruby?step=createNewProject0&workspaceFolder=Tester-Ruby&workspaceName=Tester&projectName=tester&gemName=tester&gemVer=1.1.0)

Next, provide ``` TestApp ``` as the project name, choose ``` Rails Application ``` as the project type, and click ``` OK ```.

![Create a new Rails Application in RubyMine - step 1](https://apidocs.io/illustration/ruby?step=createNewProject1&workspaceFolder=Tester-Ruby&workspaceName=Tester&projectName=tester&gemName=tester&gemVer=1.1.0)

In the next dialog make sure that correct *Ruby SDK* is being used (minimum 2.0.0) and click ``` OK ```.

![Create a new Rails Application in RubyMine - step 2](https://apidocs.io/illustration/ruby?step=createNewProject2&workspaceFolder=Tester-Ruby&workspaceName=Tester&projectName=tester&gemName=tester&gemVer=1.1.0)

This will create a new Rails Application project with an existing set of files and folder.

### 2. Add reference of the gem

In order to use the Tester gem in the new project we must add a gem reference. Locate the ```Gemfile``` in the *Project Explorer* window under the ``` TestApp ``` project node. The file contains references to all gems being used in the project. Here, add the reference to the library gem by adding the following line: ``` gem 'tester', '~> 1.1.0' ```

![Add references of the Gemfile](https://apidocs.io/illustration/ruby?step=addReference&workspaceFolder=Tester-Ruby&workspaceName=Tester&projectName=tester&gemName=tester&gemVer=1.1.0)

### 3. Adding a new Rails Controller

Once the ``` TestApp ``` project is created, a folder named ``` controllers ``` will be visible in the *Project Explorer* under the following path: ``` TestApp > app > controllers ```. Right click on this folder and select ``` New -> Run Rails Generator... ```.

![Run Rails Generator on Controllers Folder](https://apidocs.io/illustration/ruby?step=addCode0&workspaceFolder=Tester-Ruby&workspaceName=Tester&projectName=tester&gemName=tester&gemVer=1.1.0)

Selecting the said option will popup a small window where the generator names are displayed. Here, select the ``` controller ``` template.

![Create a new Controller](https://apidocs.io/illustration/ruby?step=addCode1&workspaceFolder=Tester-Ruby&workspaceName=Tester&projectName=tester&gemName=tester&gemVer=1.1.0)

Next, a popup window will ask you for a Controller name and included Actions. For controller name provide ``` Hello ``` and include an action named ``` Index ``` and click ``` OK ```.

![Add a new Controller](https://apidocs.io/illustration/ruby?step=addCode2&workspaceFolder=Tester-Ruby&workspaceName=Tester&projectName=tester&gemName=tester&gemVer=1.1.0)

A new controller class anmed ``` HelloController ``` will be created in a file named ``` hello_controller.rb ``` containing a method named ``` Index ```. In this method, add code for initialization and a sample for its usage.

![Initialize the library](https://apidocs.io/illustration/ruby?step=addCode3&workspaceFolder=Tester-Ruby&workspaceName=Tester&projectName=tester&gemName=tester&gemVer=1.1.0)

## How to Test

You can test the generated SDK and the server with automatically generated test
cases as follows:

  1. From terminal/cmd navigate to the root directory of the SDK.
  2. Invoke: `bundle exec rake`

## Initialization

### 

API client can be initialized as following.

```ruby

client = Tester::TesterClient.new
```

The added initlization code can be debugged by putting a breakpoint in the ``` Index ``` method and running the project in debug mode by selecting ``` Run -> Debug 'Development: TestApp' ```.

![Debug the TestApp](https://apidocs.io/illustration/ruby?step=addCode4&workspaceFolder=Tester-Ruby&workspaceName=Tester&projectName=tester&gemName=tester&gemVer=1.1.0&initLine=client%2520%253D%2520TesterClient.new)



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

The singleton instance of the ``` ResponseTypesController ``` class can be accessed from the API Client.

```ruby
responseTypes = client.response_types
```

### <a name="get_date_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_date_array") get_date_array

> TODO: Add a method description


```ruby
def get_date_array; end
```

#### Example Usage

```ruby

result = responseTypes.get_date_array()

```


### <a name="get_date"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_date") get_date

> TODO: Add a method description


```ruby
def get_date; end
```

#### Example Usage

```ruby

result = responseTypes.get_date()

```


### <a name="get_long"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_long") get_long

> TODO: Add a method description


```ruby
def get_long; end
```

#### Example Usage

```ruby

result = responseTypes.get_long()

```


### <a name="get_model"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_model") get_model

> TODO: Add a method description


```ruby
def get_model; end
```

#### Example Usage

```ruby

result = responseTypes.get_model()

```


### <a name="get_string_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_string_enum_array") get_string_enum_array

> TODO: Add a method description


```ruby
def get_string_enum_array; end
```

#### Example Usage

```ruby

result = responseTypes.get_string_enum_array()

```


### <a name="get_string_enum"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_string_enum") get_string_enum

> TODO: Add a method description


```ruby
def get_string_enum; end
```

#### Example Usage

```ruby

result = responseTypes.get_string_enum()

```


### <a name="get_model_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_model_array") get_model_array

> TODO: Add a method description


```ruby
def get_model_array; end
```

#### Example Usage

```ruby

result = responseTypes.get_model_array()

```


### <a name="get_int_enum"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_int_enum") get_int_enum

> TODO: Add a method description


```ruby
def get_int_enum; end
```

#### Example Usage

```ruby

result = responseTypes.get_int_enum()

```


### <a name="get_int_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_int_enum_array") get_int_enum_array

> TODO: Add a method description


```ruby
def get_int_enum_array; end
```

#### Example Usage

```ruby

result = responseTypes.get_int_enum_array()

```


### <a name="get_precision"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_precision") get_precision

> TODO: Add a method description


```ruby
def get_precision; end
```

#### Example Usage

```ruby

result = responseTypes.get_precision()

```


### <a name="get_binary"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_binary") get_binary

> gets a binary object


```ruby
def get_binary; end
```

#### Example Usage

```ruby

result = responseTypes.get_binary()

```


### <a name="get_integer"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_integer") get_integer

> Gets a integer response


```ruby
def get_integer; end
```

#### Example Usage

```ruby

result = responseTypes.get_integer()

```


### <a name="get_integer_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_integer_array") get_integer_array

> Get an array of integers.


```ruby
def get_integer_array; end
```

#### Example Usage

```ruby

result = responseTypes.get_integer_array()

```


### <a name="get_dynamic"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_dynamic") get_dynamic

> TODO: Add a method description


```ruby
def get_dynamic; end
```

#### Example Usage

```ruby

result = responseTypes.get_dynamic()

```


### <a name="get_dynamic_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_dynamic_array") get_dynamic_array

> TODO: Add a method description


```ruby
def get_dynamic_array; end
```

#### Example Usage

```ruby

result = responseTypes.get_dynamic_array()

```


### <a name="get_3339_datetime"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_3339_datetime") get_3339_datetime

> TODO: Add a method description


```ruby
def get_3339_datetime; end
```

#### Example Usage

```ruby

result = responseTypes.get_3339_datetime()

```


### <a name="get_3339_datetime_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_3339_datetime_array") get_3339_datetime_array

> TODO: Add a method description


```ruby
def get_3339_datetime_array; end
```

#### Example Usage

```ruby

result = responseTypes.get_3339_datetime_array()

```


### <a name="get_boolean"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_boolean") get_boolean

> TODO: Add a method description


```ruby
def get_boolean; end
```

#### Example Usage

```ruby

result = responseTypes.get_boolean()

```


### <a name="get_boolean_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_boolean_array") get_boolean_array

> TODO: Add a method description


```ruby
def get_boolean_array; end
```

#### Example Usage

```ruby

result = responseTypes.get_boolean_array()

```


### <a name="get_headers"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_headers") get_headers

> TODO: Add a method description


```ruby
def get_headers; end
```

#### Example Usage

```ruby

responseTypes.get_headers()

```


### <a name="get_1123_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_1123_date_time") get_1123_date_time

> TODO: Add a method description


```ruby
def get_1123_date_time; end
```

#### Example Usage

```ruby

result = responseTypes.get_1123_date_time()

```


### <a name="get_unix_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_unix_date_time") get_unix_date_time

> TODO: Add a method description


```ruby
def get_unix_date_time; end
```

#### Example Usage

```ruby

result = responseTypes.get_unix_date_time()

```


### <a name="get_1123_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_1123_date_time_array") get_1123_date_time_array

> TODO: Add a method description


```ruby
def get_1123_date_time_array; end
```

#### Example Usage

```ruby

result = responseTypes.get_1123_date_time_array()

```


### <a name="get_unix_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_unix_date_time_array") get_unix_date_time_array

> TODO: Add a method description


```ruby
def get_unix_date_time_array; end
```

#### Example Usage

```ruby

result = responseTypes.get_unix_date_time_array()

```


[Back to List of Controllers](#list_of_controllers)

## <a name="body_params_controller"></a>![Class: ](https://apidocs.io/img/class.png ".BodyParamsController") BodyParamsController

### Get singleton instance

The singleton instance of the ``` BodyParamsController ``` class can be accessed from the API Client.

```ruby
bodyParams = client.body_params
```

### <a name="send_date_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_date_array") send_date_array

> TODO: Add a method description


```ruby
def send_date_array(dates); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dates |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
dates_value = "["1994-02-13", "1994-02-13"]";
dates = JSON.parse(dates_value);

result = bodyParams.send_date_array(dates)

```


### <a name="send_date"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_date") send_date

> TODO: Add a method description


```ruby
def send_date(date); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| date |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
date = 1994-02-13

result = bodyParams.send_date(date)

```


### <a name="send_unix_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_unix_date_time") send_unix_date_time

> TODO: Add a method description


```ruby
def send_unix_date_time(datetime); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
datetime = 1484719381

result = bodyParams.send_unix_date_time(datetime)

```


### <a name="send_rfc_1123_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_rfc_1123_date_time") send_rfc_1123_date_time

> TODO: Add a method description


```ruby
def send_rfc_1123_date_time(datetime); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
datetime = Sun, 06 Nov 1994 08:49:37 GMT

result = bodyParams.send_rfc_1123_date_time(datetime)

```


### <a name="send_rfc_3339_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_rfc_3339_date_time") send_rfc_3339_date_time

> TODO: Add a method description


```ruby
def send_rfc_3339_date_time(datetime); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
datetime = 1994-02-13T14:01:54.9571247Z

result = bodyParams.send_rfc_3339_date_time(datetime)

```


### <a name="send_unix_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_unix_date_time_array") send_unix_date_time_array

> TODO: Add a method description


```ruby
def send_unix_date_time_array(datetimes); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
datetimes_value = "[1484719381,1484719381]";
datetimes = JSON.parse(datetimes_value);

result = bodyParams.send_unix_date_time_array(datetimes)

```


### <a name="send_rfc_1123_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_rfc_1123_date_time_array") send_rfc_1123_date_time_array

> TODO: Add a method description


```ruby
def send_rfc_1123_date_time_array(datetimes); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
datetimes_value = "["Sun, 06 Nov 1994 08:49:37 GMT","Sun, 06 Nov 1994 08:49:37 GMT"]";
datetimes = JSON.parse(datetimes_value);

result = bodyParams.send_rfc_1123_date_time_array(datetimes)

```


### <a name="send_rfc_3339_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_rfc_3339_date_time_array") send_rfc_3339_date_time_array

> TODO: Add a method description


```ruby
def send_rfc_3339_date_time_array(datetimes); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
datetimes_value = "["1994-02-13T14:01:54.9571247Z","1994-02-13T14:01:54.9571247Z"]";
datetimes = JSON.parse(datetimes_value);

result = bodyParams.send_rfc_3339_date_time_array(datetimes)

```


### <a name="send_string_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_string_array") send_string_array

> sends a string body param


```ruby
def send_string_array(sarray); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| sarray |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
sarray_value = "["abc", "def"]";
sarray = JSON.parse(sarray_value);

result = bodyParams.send_string_array(sarray)

```


### <a name="send_integer_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_integer_array") send_integer_array

> TODO: Add a method description


```ruby
def send_integer_array(integers); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
integers_value = "[1,2,3,4,5]";
integers = JSON.parse(integers_value);

result = bodyParams.send_integer_array(integers)

```


### <a name="send_model"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_model") send_model

> TODO: Add a method description


```ruby
def send_model(model); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| model |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
model_value = "{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}";
model = JSON.parse(model_value);

result = bodyParams.send_model(model)

```


### <a name="send_model_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_model_array") send_model_array

> TODO: Add a method description


```ruby
def send_model_array(models); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| models |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
models_value = "[{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"},{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}]";
models = JSON.parse(models_value);

result = bodyParams.send_model_array(models)

```


### <a name="send_dynamic"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_dynamic") send_dynamic

> TODO: Add a method description


```ruby
def send_dynamic(dynamic); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dynamic |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
dynamic_value = "{\"uid\": \"1123213\", \"name\": \"Shahid\"}";
dynamic = JSON.parse(dynamic_value);

result = bodyParams.send_dynamic(dynamic)

```


### <a name="send_string"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_string") send_string

> TODO: Add a method description


```ruby
def send_string(value); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| value |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
value = 'TestString'

result = bodyParams.send_string(value)

```


### <a name="send_string_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_string_enum_array") send_string_enum_array

> TODO: Add a method description


```ruby
def send_string_enum_array(days); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| days |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
days = [Tester::Days::TUESDAY,Tester::Days::SATURDAY,Tester::Days::MONDAY,Tester::Days::SUNDAY]

result = bodyParams.send_string_enum_array(days)

```


### <a name="send_integer_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_integer_enum_array") send_integer_enum_array

> TODO: Add a method description


```ruby
def send_integer_enum_array(suites); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| suites |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
suites = [Tester::SuiteCode::HEARTS,Tester::SuiteCode::CLUBS,Tester::SuiteCode::DIAMONDS,Tester::SuiteCode::SPADES,Tester::SuiteCode::CLUBS]

result = bodyParams.send_integer_enum_array(suites)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="form_params_controller"></a>![Class: ](https://apidocs.io/img/class.png ".FormParamsController") FormParamsController

### Get singleton instance

The singleton instance of the ``` FormParamsController ``` class can be accessed from the API Client.

```ruby
formParams = client.form_params
```

### <a name="send_date_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_date_array") send_date_array

> TODO: Add a method description


```ruby
def send_date_array(dates); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dates |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
dates_value = "["1994-02-13","1994-02-13"]";
dates = JSON.parse(dates_value);

result = formParams.send_date_array(dates)

```


### <a name="send_date"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_date") send_date

> TODO: Add a method description


```ruby
def send_date(date); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| date |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
date = 1994-02-13

result = formParams.send_date(date)

```


### <a name="send_unix_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_unix_date_time") send_unix_date_time

> TODO: Add a method description


```ruby
def send_unix_date_time(datetime); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
datetime = 1484719381

result = formParams.send_unix_date_time(datetime)

```


### <a name="send_rfc_1123_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_rfc_1123_date_time") send_rfc_1123_date_time

> TODO: Add a method description


```ruby
def send_rfc_1123_date_time(datetime); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
datetime = Sun, 06 Nov 1994 08:49:37 GMT

result = formParams.send_rfc_1123_date_time(datetime)

```


### <a name="send_rfc_3339_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_rfc_3339_date_time") send_rfc_3339_date_time

> TODO: Add a method description


```ruby
def send_rfc_3339_date_time(datetime); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
datetime = 1994-02-13T14:01:54.9571247Z

result = formParams.send_rfc_3339_date_time(datetime)

```


### <a name="send_unix_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_unix_date_time_array") send_unix_date_time_array

> TODO: Add a method description


```ruby
def send_unix_date_time_array(datetimes); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
datetimes_value = "[1484719381,1484719381]";
datetimes = JSON.parse(datetimes_value);

result = formParams.send_unix_date_time_array(datetimes)

```


### <a name="send_rfc_1123_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_rfc_1123_date_time_array") send_rfc_1123_date_time_array

> TODO: Add a method description


```ruby
def send_rfc_1123_date_time_array(datetimes); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
datetimes_value = "["Sun, 06 Nov 1994 08:49:37 GMT","Sun, 06 Nov 1994 08:49:37 GMT"]";
datetimes = JSON.parse(datetimes_value);

result = formParams.send_rfc_1123_date_time_array(datetimes)

```


### <a name="send_long"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_long") send_long

> TODO: Add a method description


```ruby
def send_long(value); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| value |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
value = 5147483647

result = formParams.send_long(value)

```


### <a name="send_integer_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_integer_array") send_integer_array

> TODO: Add a method description


```ruby
def send_integer_array(integers); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
integers_value = "[1,2,3,4,5]";
integers = JSON.parse(integers_value);

result = formParams.send_integer_array(integers)

```


### <a name="send_string_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_string_array") send_string_array

> TODO: Add a method description


```ruby
def send_string_array(strings); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
strings_value = "["abc", "def"]";
strings = JSON.parse(strings_value);

result = formParams.send_string_array(strings)

```


### <a name="send_model"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_model") send_model

> TODO: Add a method description


```ruby
def send_model(model); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| model |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
model_value = "{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}";
model = JSON.parse(model_value);

result = formParams.send_model(model)

```


### <a name="send_model_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_model_array") send_model_array

> TODO: Add a method description


```ruby
def send_model_array(models); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| models |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
models_value = "[{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"},{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}]";
models = JSON.parse(models_value);

result = formParams.send_model_array(models)

```


### <a name="send_file"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_file") send_file

> TODO: Add a method description


```ruby
def send_file(file); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
file = Faraday::UploadIO.new('PathToFile', 'application/octet-stream')

result = formParams.send_file(file)

```


### <a name="send_string"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_string") send_string

> TODO: Add a method description


```ruby
def send_string(value); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| value |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
value = 'TestString'

result = formParams.send_string(value)

```


### <a name="send_rfc_3339_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_rfc_3339_date_time_array") send_rfc_3339_date_time_array

> TODO: Add a method description


```ruby
def send_rfc_3339_date_time_array(datetimes); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
datetimes_value = "["1994-02-13T14:01:54.9571247Z","1994-02-13T14:01:54.9571247Z"]";
datetimes = JSON.parse(datetimes_value);

result = formParams.send_rfc_3339_date_time_array(datetimes)

```


### <a name="send_mixed_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_mixed_array") send_mixed_array

> Send a variety for form params. Returns file count and body params


```ruby
def send_mixed_array(options = Hash.new); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | TODO: Add a parameter description |
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |
| models |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
collect = Hash.new

file = Faraday::UploadIO.new('PathToFile', 'application/octet-stream')
collect['file'] = file

integers_value = "[1,2,3,4,5]";
integers = JSON.parse(integers_value);
collect['integers'] = integers

models_value = "[{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"},{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}]";
models = JSON.parse(models_value);
collect['models'] = models

strings_value = "["abc", "def"]";
strings = JSON.parse(strings_value);
collect['strings'] = strings


result = formParams.send_mixed_array(collect)

```


### <a name="send_integer_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_integer_enum_array") send_integer_enum_array

> TODO: Add a method description


```ruby
def send_integer_enum_array(suites); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| suites |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
suites = [Tester::SuiteCode::HEARTS,Tester::SuiteCode::CLUBS,Tester::SuiteCode::DIAMONDS,Tester::SuiteCode::SPADES,Tester::SuiteCode::CLUBS]

result = formParams.send_integer_enum_array(suites)

```


### <a name="send_string_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_string_enum_array") send_string_enum_array

> TODO: Add a method description


```ruby
def send_string_enum_array(days); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| days |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
days = [Tester::Days::TUESDAY,Tester::Days::SATURDAY,Tester::Days::MONDAY,Tester::Days::SUNDAY]

result = formParams.send_string_enum_array(days)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="query_param_controller"></a>![Class: ](https://apidocs.io/img/class.png ".QueryParamController") QueryParamController

### Get singleton instance

The singleton instance of the ``` QueryParamController ``` class can be accessed from the API Client.

```ruby
queryParam = client.query_param
```

### <a name="date_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.date_array") date_array

> TODO: Add a method description


```ruby
def date_array(dates); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dates |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
dates_value = "["1994-02-13","1994-02-13"]";
dates = JSON.parse(dates_value);

result = queryParam.date_array(dates)

```


### <a name="date"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.date") date

> TODO: Add a method description


```ruby
def date(date); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| date |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
date = 1994-02-13

result = queryParam.date(date)

```


### <a name="unix_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.unix_date_time_array") unix_date_time_array

> TODO: Add a method description


```ruby
def unix_date_time_array(datetimes); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
datetimes_value = "[1484719381,1484719381]";
datetimes = JSON.parse(datetimes_value);

result = queryParam.unix_date_time_array(datetimes)

```


### <a name="unix_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.unix_date_time") unix_date_time

> TODO: Add a method description


```ruby
def unix_date_time(datetime); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
datetime = 1484719381

result = queryParam.unix_date_time(datetime)

```


### <a name="rfc_1123_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.rfc_1123_date_time") rfc_1123_date_time

> TODO: Add a method description


```ruby
def rfc_1123_date_time(datetime); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
datetime = Sun, 06 Nov 1994 08:49:37 GMT

result = queryParam.rfc_1123_date_time(datetime)

```


### <a name="rfc_1123_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.rfc_1123_date_time_array") rfc_1123_date_time_array

> TODO: Add a method description


```ruby
def rfc_1123_date_time_array(datetimes); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
datetimes_value = "["Sun, 06 Nov 1994 08:49:37 GMT","Sun, 06 Nov 1994 08:49:37 GMT"]";
datetimes = JSON.parse(datetimes_value);

result = queryParam.rfc_1123_date_time_array(datetimes)

```


### <a name="rfc_3339_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.rfc_3339_date_time_array") rfc_3339_date_time_array

> TODO: Add a method description


```ruby
def rfc_3339_date_time_array(datetimes); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
datetimes_value = "["1994-02-13T14:01:54.9571247Z","1994-02-13T14:01:54.9571247Z"]";
datetimes = JSON.parse(datetimes_value);

result = queryParam.rfc_3339_date_time_array(datetimes)

```


### <a name="rfc_3339_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.rfc_3339_date_time") rfc_3339_date_time

> TODO: Add a method description


```ruby
def rfc_3339_date_time(datetime); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
datetime = 1994-02-13T14:01:54.9571247Z

result = queryParam.rfc_3339_date_time(datetime)

```


### <a name="no_params"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.no_params") no_params

> TODO: Add a method description


```ruby
def no_params; end
```

#### Example Usage

```ruby

result = queryParam.no_params()

```


### <a name="string_param"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.string_param") string_param

> TODO: Add a method description


```ruby
def string_param(string); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| string |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
string = 'l;asd;asdwe[2304&&;\'.d??\\a\\\\\\;sd//'

result = queryParam.string_param(string)

```


### <a name="url_param"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.url_param") url_param

> TODO: Add a method description


```ruby
def url_param(url); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| url |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
url = 'https://www.shahidisawesome.com/and/also/a/narcissist?thisis=aparameter&another=one'

result = queryParam.url_param(url)

```


### <a name="number_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.number_array") number_array

> TODO: Add a method description


```ruby
def number_array(integers); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
integers_value = "[1,2,3,4,5]";
integers = JSON.parse(integers_value);

result = queryParam.number_array(integers)

```


### <a name="string_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.string_array") string_array

> TODO: Add a method description


```ruby
def string_array(strings); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
strings_value = "["abc", "def"]";
strings = JSON.parse(strings_value);

result = queryParam.string_array(strings)

```


### <a name="simple_query"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.simple_query") simple_query

> TODO: Add a method description


```ruby
def simple_query(boolean,
                     number,
                     string,
                     _query_parameters = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| boolean |  ``` Required ```  | TODO: Add a parameter description |
| number |  ``` Required ```  | TODO: Add a parameter description |
| string |  ``` Required ```  | TODO: Add a parameter description |
| _query_parameters | ``` Optional ``` | Additional optional query parameters are supported by this method |


#### Example Usage

```ruby
boolean = true
number = 4
string = 'TestString'
# key-value map for optional query parameters
queryParams = { 'key' => 'value' }

result = queryParam.simple_query(boolean, number, string, queryParams)

```


### <a name="string_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.string_enum_array") string_enum_array

> TODO: Add a method description


```ruby
def string_enum_array(days); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| days |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
days = [Tester::Days::TUESDAY,Tester::Days::SATURDAY,Tester::Days::MONDAY,Tester::Days::SUNDAY]

result = queryParam.string_enum_array(days)

```


### <a name="multiple_params"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.multiple_params") multiple_params

> TODO: Add a method description


```ruby
def multiple_params(number,
                        precision,
                        string,
                        url); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| number |  ``` Required ```  | TODO: Add a parameter description |
| precision |  ``` Required ```  | TODO: Add a parameter description |
| string |  ``` Required ```  | TODO: Add a parameter description |
| url |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
number = 123412312
precision = 1112.34
string = '""test./;";12&&3asl"";"qw1&34"///..//.'
url = 'http://www.abc.com/test?a=b&c="http://lolol.com?param=no&another=lol"'

result = queryParam.multiple_params(number, precision, string, url)

```


### <a name="integer_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.integer_enum_array") integer_enum_array

> TODO: Add a method description


```ruby
def integer_enum_array(suites); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| suites |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
suites = [Tester::SuiteCode::HEARTS,Tester::SuiteCode::CLUBS,Tester::SuiteCode::DIAMONDS,Tester::SuiteCode::SPADES,Tester::SuiteCode::CLUBS]

result = queryParam.integer_enum_array(suites)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="error_codes_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ErrorCodesController") ErrorCodesController

### Get singleton instance

The singleton instance of the ``` ErrorCodesController ``` class can be accessed from the API Client.

```ruby
errorCodes = client.error_codes
```

### <a name="get_400"></a>![Method: ](https://apidocs.io/img/method.png ".ErrorCodesController.get_400") get_400

> TODO: Add a method description


```ruby
def get_400; end
```

#### Example Usage

```ruby

result = errorCodes.get_400()

```


### <a name="get_500"></a>![Method: ](https://apidocs.io/img/method.png ".ErrorCodesController.get_500") get_500

> TODO: Add a method description


```ruby
def get_500; end
```

#### Example Usage

```ruby

result = errorCodes.get_500()

```


### <a name="get_401"></a>![Method: ](https://apidocs.io/img/method.png ".ErrorCodesController.get_401") get_401

> TODO: Add a method description


```ruby
def get_401; end
```

#### Example Usage

```ruby

result = errorCodes.get_401()

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

The singleton instance of the ``` EchoController ``` class can be accessed from the API Client.

```ruby
echo = client.echo
```

### <a name="json_echo"></a>![Method: ](https://apidocs.io/img/method.png ".EchoController.json_echo") json_echo

> Echo's back the request


```ruby
def json_echo(input); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| input |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
input_value = "{\"uid\": \"1123213\", \"name\": \"Shahid\"}";
input = JSON.parse(input_value);

result = echo.json_echo(input)

```


### <a name="form_echo"></a>![Method: ](https://apidocs.io/img/method.png ".EchoController.form_echo") form_echo

> Sends the request including any form params as JSON


```ruby
def form_echo(input); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| input |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
input_value = "{\"uid\": \"1123213\", \"name\": \"Shahid\"}";
input = JSON.parse(input_value);

result = echo.form_echo(input)

```


### <a name="query_echo"></a>![Method: ](https://apidocs.io/img/method.png ".EchoController.query_echo") query_echo

> TODO: Add a method description


```ruby
def query_echo(_query_parameters = nil); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| _query_parameters | ``` Optional ``` | Additional optional query parameters are supported by this method |


#### Example Usage

```ruby
# key-value map for optional query parameters
queryParams = { 'key' => 'value' }

result = echo.query_echo(queryParams)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="header_controller"></a>![Class: ](https://apidocs.io/img/class.png ".HeaderController") HeaderController

### Get singleton instance

The singleton instance of the ``` HeaderController ``` class can be accessed from the API Client.

```ruby
header = client.header
```

### <a name="send_headers"></a>![Method: ](https://apidocs.io/img/method.png ".HeaderController.send_headers") send_headers

> Sends a single header params


```ruby
def send_headers(custom_header,
                     value); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| custom_header |  ``` Required ```  | TODO: Add a parameter description |
| value |  ``` Required ```  | Represents the value of the custom header |


#### Example Usage

```ruby
custom_header = 'TestString'
value = 'TestString'

result = header.send_headers(custom_header, value)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="template_params_controller"></a>![Class: ](https://apidocs.io/img/class.png ".TemplateParamsController") TemplateParamsController

### Get singleton instance

The singleton instance of the ``` TemplateParamsController ``` class can be accessed from the API Client.

```ruby
templateParams = client.template_params
```

### <a name="send_string_array"></a>![Method: ](https://apidocs.io/img/method.png ".TemplateParamsController.send_string_array") send_string_array

> TODO: Add a method description


```ruby
def send_string_array(strings); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
strings_value = "["abc", "def"]";
strings = JSON.parse(strings_value);

result = templateParams.send_string_array(strings)

```


### <a name="send_integer_array"></a>![Method: ](https://apidocs.io/img/method.png ".TemplateParamsController.send_integer_array") send_integer_array

> TODO: Add a method description


```ruby
def send_integer_array(integers); end
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```ruby
integers_value = "[1,2,3,4,5]";
integers = JSON.parse(integers_value);

result = templateParams.send_integer_array(integers)

```


[Back to List of Controllers](#list_of_controllers)



