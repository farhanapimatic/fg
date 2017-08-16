# Getting started

Testing various
 api 
features

## How to Build


You must have Python 2 >=2.7.9 or Python 3 >=3.4 installed on your system to install and run this SDK. This SDK package depends on other Python packages like nose, jsonpickle etc. 
These dependencies are defined in the ```requirements.txt``` file that comes with the SDK.
To resolve these dependencies, you can use the PIP Dependency manager. Install it by following steps at [https://pip.pypa.io/en/stable/installing/](https://pip.pypa.io/en/stable/installing/).

Python and PIP executables should be defined in your PATH. Open command prompt and type ```pip --version```.
This should display the version of the PIP Dependency Manager installed if your installation was successful and the paths are properly defined.

* Using command line, navigate to the directory containing the generated files (including ```requirements.txt```) for the SDK.
* Run the command ```pip install -r requirements.txt```. This should install all the required dependencies.

![Building SDK - Step 1](https://apidocs.io/illustration/python?step=installDependencies&workspaceFolder=Tester-Python)


## How to Use

The following section explains how to use the Tester SDK package in a new project.

### 1. Open Project in an IDE

Open up a Python IDE like PyCharm. The basic workflow presented here is also applicable if you prefer using a different editor or IDE.

![Open project in PyCharm - Step 1](https://apidocs.io/illustration/python?step=pyCharm)

Click on ```Open``` in PyCharm to browse to your generated SDK directory and then click ```OK```.

![Open project in PyCharm - Step 2](https://apidocs.io/illustration/python?step=openProject0&workspaceFolder=Tester-Python)     

The project files will be displayed in the side bar as follows:

![Open project in PyCharm - Step 3](https://apidocs.io/illustration/python?step=openProject1&workspaceFolder=Tester-Python&projectName=tester)     

### 2. Add a new Test Project

Create a new directory by right clicking on the solution name as shown below:

![Add a new project in PyCharm - Step 1](https://apidocs.io/illustration/python?step=createDirectory&workspaceFolder=Tester-Python&projectName=tester)

Name the directory as "test"

![Add a new project in PyCharm - Step 2](https://apidocs.io/illustration/python?step=nameDirectory)
   
Add a python file to this project with the name "testsdk"

![Add a new project in PyCharm - Step 3](https://apidocs.io/illustration/python?step=createFile&workspaceFolder=Tester-Python&projectName=tester)

Name it "testsdk"

![Add a new project in PyCharm - Step 4](https://apidocs.io/illustration/python?step=nameFile)

In your python file you will be required to import the generated python library using the following code lines

```Python
from tester.tester_client import TesterClient
```

![Add a new project in PyCharm - Step 4](https://apidocs.io/illustration/python?step=projectFiles&workspaceFolder=Tester-Python&libraryName=tester.tester_client&projectName=tester)

After this you can write code to instantiate an API client object, get a controller object and  make API calls. Sample code is given in the subsequent sections.

### 3. Run the Test Project

To run the file within your test project, right click on your Python file inside your Test project and click on ```Run```

![Run Test Project - Step 1](https://apidocs.io/illustration/python?step=runProject&workspaceFolder=Tester-Python&libraryName=tester.tester_client&projectName=tester)


## How to Test

You can test the generated SDK and the server with automatically generated test
cases. unittest is used as the testing framework and nose is used as the test
runner. You can run the tests as follows:

  1. From terminal/cmd navigate to the root directory of the SDK.
  2. Invoke 'pip install -r test-requirements.txt'
  3. Invoke 'nosetests'

## Initialization

### 

API client can be initialized as following.

```python

client = TesterClient()
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

### Get controller instance

An instance of the ``` ResponseTypesController ``` class can be accessed from the API Client.

```python
 response_types_client = client.response_types
```

### <a name="get_date_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_date_array") get_date_array

> TODO: Add a method description

```python
def get_date_array(self)
```

#### Example Usage

```python

result = response_types_client.get_date_array()

```


### <a name="get_date"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_date") get_date

> TODO: Add a method description

```python
def get_date(self)
```

#### Example Usage

```python

result = response_types_client.get_date()

```


### <a name="get_long"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_long") get_long

> TODO: Add a method description

```python
def get_long(self)
```

#### Example Usage

```python

result = response_types_client.get_long()

```


### <a name="get_model"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_model") get_model

> TODO: Add a method description

```python
def get_model(self)
```

#### Example Usage

```python

result = response_types_client.get_model()

```


### <a name="get_string_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_string_enum_array") get_string_enum_array

> TODO: Add a method description

```python
def get_string_enum_array(self)
```

#### Example Usage

```python

result = response_types_client.get_string_enum_array()

```


### <a name="get_string_enum"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_string_enum") get_string_enum

> TODO: Add a method description

```python
def get_string_enum(self)
```

#### Example Usage

```python

result = response_types_client.get_string_enum()

```


### <a name="get_model_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_model_array") get_model_array

> TODO: Add a method description

```python
def get_model_array(self)
```

#### Example Usage

```python

result = response_types_client.get_model_array()

```


### <a name="get_int_enum"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_int_enum") get_int_enum

> TODO: Add a method description

```python
def get_int_enum(self)
```

#### Example Usage

```python

result = response_types_client.get_int_enum()

```


### <a name="get_int_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_int_enum_array") get_int_enum_array

> TODO: Add a method description

```python
def get_int_enum_array(self)
```

#### Example Usage

```python

result = response_types_client.get_int_enum_array()

```


### <a name="get_precision"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_precision") get_precision

> TODO: Add a method description

```python
def get_precision(self)
```

#### Example Usage

```python

result = response_types_client.get_precision()

```


### <a name="get_binary"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_binary") get_binary

> gets a binary object

```python
def get_binary(self)
```

#### Example Usage

```python

result = response_types_client.get_binary()

```


### <a name="get_integer"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_integer") get_integer

> Gets a integer response

```python
def get_integer(self)
```

#### Example Usage

```python

result = response_types_client.get_integer()

```


### <a name="get_integer_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_integer_array") get_integer_array

> Get an array of integers.

```python
def get_integer_array(self)
```

#### Example Usage

```python

result = response_types_client.get_integer_array()

```


### <a name="get_dynamic"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_dynamic") get_dynamic

> TODO: Add a method description

```python
def get_dynamic(self)
```

#### Example Usage

```python

result = response_types_client.get_dynamic()

```


### <a name="get_dynamic_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_dynamic_array") get_dynamic_array

> TODO: Add a method description

```python
def get_dynamic_array(self)
```

#### Example Usage

```python

result = response_types_client.get_dynamic_array()

```


### <a name="get_3339_datetime"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_3339_datetime") get_3339_datetime

> TODO: Add a method description

```python
def get_3339_datetime(self)
```

#### Example Usage

```python

result = response_types_client.get_3339_datetime()

```


### <a name="get_3339_datetime_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_3339_datetime_array") get_3339_datetime_array

> TODO: Add a method description

```python
def get_3339_datetime_array(self)
```

#### Example Usage

```python

result = response_types_client.get_3339_datetime_array()

```


### <a name="get_boolean"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_boolean") get_boolean

> TODO: Add a method description

```python
def get_boolean(self)
```

#### Example Usage

```python

result = response_types_client.get_boolean()

```


### <a name="get_boolean_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_boolean_array") get_boolean_array

> TODO: Add a method description

```python
def get_boolean_array(self)
```

#### Example Usage

```python

result = response_types_client.get_boolean_array()

```


### <a name="get_headers"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_headers") get_headers

> TODO: Add a method description

```python
def get_headers(self)
```

#### Example Usage

```python

response_types_client.get_headers()

```


### <a name="get_1123_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_1123_date_time") get_1123_date_time

> TODO: Add a method description

```python
def get_1123_date_time(self)
```

#### Example Usage

```python

result = response_types_client.get_1123_date_time()

```


### <a name="get_unix_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_unix_date_time") get_unix_date_time

> TODO: Add a method description

```python
def get_unix_date_time(self)
```

#### Example Usage

```python

result = response_types_client.get_unix_date_time()

```


### <a name="get_1123_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_1123_date_time_array") get_1123_date_time_array

> TODO: Add a method description

```python
def get_1123_date_time_array(self)
```

#### Example Usage

```python

result = response_types_client.get_1123_date_time_array()

```


### <a name="get_unix_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".ResponseTypesController.get_unix_date_time_array") get_unix_date_time_array

> TODO: Add a method description

```python
def get_unix_date_time_array(self)
```

#### Example Usage

```python

result = response_types_client.get_unix_date_time_array()

```


[Back to List of Controllers](#list_of_controllers)

## <a name="body_params_controller"></a>![Class: ](https://apidocs.io/img/class.png ".BodyParamsController") BodyParamsController

### Get controller instance

An instance of the ``` BodyParamsController ``` class can be accessed from the API Client.

```python
 body_params_client = client.body_params
```

### <a name="send_date_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_date_array") send_date_array

> TODO: Add a method description

```python
def send_date_array(self,
                        dates)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dates |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
dates_value = ["1994-02-13", "1994-02-13"]
dates = json.loads(dates_value)

result = body_params_client.send_date_array(dates)

```


### <a name="send_date"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_date") send_date

> TODO: Add a method description

```python
def send_date(self,
                  date)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| date |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
date = 1994-02-13

result = body_params_client.send_date(date)

```


### <a name="send_unix_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_unix_date_time") send_unix_date_time

> TODO: Add a method description

```python
def send_unix_date_time(self,
                            datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
datetime = 1484719381

result = body_params_client.send_unix_date_time(datetime)

```


### <a name="send_rfc_1123_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_rfc_1123_date_time") send_rfc_1123_date_time

> TODO: Add a method description

```python
def send_rfc_1123_date_time(self,
                                datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
datetime = Sun, 06 Nov 1994 08:49:37 GMT

result = body_params_client.send_rfc_1123_date_time(datetime)

```


### <a name="send_rfc_3339_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_rfc_3339_date_time") send_rfc_3339_date_time

> TODO: Add a method description

```python
def send_rfc_3339_date_time(self,
                                datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
datetime = 1994-02-13T14:01:54.9571247Z

result = body_params_client.send_rfc_3339_date_time(datetime)

```


### <a name="send_unix_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_unix_date_time_array") send_unix_date_time_array

> TODO: Add a method description

```python
def send_unix_date_time_array(self,
                                  datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
datetimes_value = [1484719381,1484719381]
datetimes = json.loads(datetimes_value)

result = body_params_client.send_unix_date_time_array(datetimes)

```


### <a name="send_rfc_1123_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_rfc_1123_date_time_array") send_rfc_1123_date_time_array

> TODO: Add a method description

```python
def send_rfc_1123_date_time_array(self,
                                      datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
datetimes_value = ["Sun, 06 Nov 1994 08:49:37 GMT","Sun, 06 Nov 1994 08:49:37 GMT"]
datetimes = json.loads(datetimes_value)

result = body_params_client.send_rfc_1123_date_time_array(datetimes)

```


### <a name="send_rfc_3339_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_rfc_3339_date_time_array") send_rfc_3339_date_time_array

> TODO: Add a method description

```python
def send_rfc_3339_date_time_array(self,
                                      datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
datetimes_value = ["1994-02-13T14:01:54.9571247Z","1994-02-13T14:01:54.9571247Z"]
datetimes = json.loads(datetimes_value)

result = body_params_client.send_rfc_3339_date_time_array(datetimes)

```


### <a name="send_string_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_string_array") send_string_array

> sends a string body param

```python
def send_string_array(self,
                          sarray)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| sarray |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
sarray_value = '["abc", "def"]'
sarray = json.loads(sarray_value)

result = body_params_client.send_string_array(sarray)

```


### <a name="send_integer_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_integer_array") send_integer_array

> TODO: Add a method description

```python
def send_integer_array(self,
                           integers)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
integers_value = "[1,2,3,4,5]"
integers = json.loads(integers_value)

result = body_params_client.send_integer_array(integers)

```


### <a name="send_model"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_model") send_model

> TODO: Add a method description

```python
def send_model(self,
                   model)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| model |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
model_value = "{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}"
model = json.loads(model_value)

result = body_params_client.send_model(model)

```


### <a name="send_model_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_model_array") send_model_array

> TODO: Add a method description

```python
def send_model_array(self,
                         models)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| models |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
models_value = "[{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"},{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}]"
models = json.loads(models_value)

result = body_params_client.send_model_array(models)

```


### <a name="send_dynamic"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_dynamic") send_dynamic

> TODO: Add a method description

```python
def send_dynamic(self,
                     dynamic)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dynamic |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
dynamic_value = "{\"uid\": \"1123213\", \"name\": \"Shahid\"}"
dynamic = json.loads(dynamic_value)

result = body_params_client.send_dynamic(dynamic)

```


### <a name="send_string"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_string") send_string

> TODO: Add a method description

```python
def send_string(self,
                    value)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| value |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
value = 'TestString'

result = body_params_client.send_string(value)

```


### <a name="send_string_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_string_enum_array") send_string_enum_array

> TODO: Add a method description

```python
def send_string_enum_array(self,
                               days)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| days |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
days = [Days.TUESDAY,Days.SATURDAY,Days.MONDAY,Days.SUNDAY]

result = body_params_client.send_string_enum_array(days)

```


### <a name="send_integer_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".BodyParamsController.send_integer_enum_array") send_integer_enum_array

> TODO: Add a method description

```python
def send_integer_enum_array(self,
                                suites)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| suites |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
suites = [SuiteCode.HEARTS,SuiteCode.CLUBS,SuiteCode.DIAMONDS,SuiteCode.SPADES,SuiteCode.CLUBS]

result = body_params_client.send_integer_enum_array(suites)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="form_params_controller"></a>![Class: ](https://apidocs.io/img/class.png ".FormParamsController") FormParamsController

### Get controller instance

An instance of the ``` FormParamsController ``` class can be accessed from the API Client.

```python
 form_params_client = client.form_params
```

### <a name="send_date_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_date_array") send_date_array

> TODO: Add a method description

```python
def send_date_array(self,
                        dates)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dates |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
dates_value = ["1994-02-13","1994-02-13"]
dates = json.loads(dates_value)

result = form_params_client.send_date_array(dates)

```


### <a name="send_date"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_date") send_date

> TODO: Add a method description

```python
def send_date(self,
                  date)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| date |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
date = 1994-02-13

result = form_params_client.send_date(date)

```


### <a name="send_unix_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_unix_date_time") send_unix_date_time

> TODO: Add a method description

```python
def send_unix_date_time(self,
                            datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
datetime = 1484719381

result = form_params_client.send_unix_date_time(datetime)

```


### <a name="send_rfc_1123_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_rfc_1123_date_time") send_rfc_1123_date_time

> TODO: Add a method description

```python
def send_rfc_1123_date_time(self,
                                datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
datetime = Sun, 06 Nov 1994 08:49:37 GMT

result = form_params_client.send_rfc_1123_date_time(datetime)

```


### <a name="send_rfc_3339_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_rfc_3339_date_time") send_rfc_3339_date_time

> TODO: Add a method description

```python
def send_rfc_3339_date_time(self,
                                datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
datetime = 1994-02-13T14:01:54.9571247Z

result = form_params_client.send_rfc_3339_date_time(datetime)

```


### <a name="send_unix_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_unix_date_time_array") send_unix_date_time_array

> TODO: Add a method description

```python
def send_unix_date_time_array(self,
                                  datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
datetimes_value = [1484719381,1484719381]
datetimes = json.loads(datetimes_value)

result = form_params_client.send_unix_date_time_array(datetimes)

```


### <a name="send_rfc_1123_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_rfc_1123_date_time_array") send_rfc_1123_date_time_array

> TODO: Add a method description

```python
def send_rfc_1123_date_time_array(self,
                                      datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
datetimes_value = ["Sun, 06 Nov 1994 08:49:37 GMT","Sun, 06 Nov 1994 08:49:37 GMT"]
datetimes = json.loads(datetimes_value)

result = form_params_client.send_rfc_1123_date_time_array(datetimes)

```


### <a name="send_long"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_long") send_long

> TODO: Add a method description

```python
def send_long(self,
                  value)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| value |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
value = 5147483647

result = form_params_client.send_long(value)

```


### <a name="send_integer_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_integer_array") send_integer_array

> TODO: Add a method description

```python
def send_integer_array(self,
                           integers)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
integers_value = "[1,2,3,4,5]"
integers = json.loads(integers_value)

result = form_params_client.send_integer_array(integers)

```


### <a name="send_string_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_string_array") send_string_array

> TODO: Add a method description

```python
def send_string_array(self,
                          strings)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
strings_value = '["abc", "def"]'
strings = json.loads(strings_value)

result = form_params_client.send_string_array(strings)

```


### <a name="send_model"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_model") send_model

> TODO: Add a method description

```python
def send_model(self,
                   model)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| model |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
model_value = "{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}"
model = json.loads(model_value)

result = form_params_client.send_model(model)

```


### <a name="send_model_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_model_array") send_model_array

> TODO: Add a method description

```python
def send_model_array(self,
                         models)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| models |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
models_value = "[{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"},{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}]"
models = json.loads(models_value)

result = form_params_client.send_model_array(models)

```


### <a name="send_file"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_file") send_file

> TODO: Add a method description

```python
def send_file(self,
                  file)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
file = open("pathtofile", 'rb')

result = form_params_client.send_file(file)

```


### <a name="send_string"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_string") send_string

> TODO: Add a method description

```python
def send_string(self,
                    value)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| value |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
value = 'TestString'

result = form_params_client.send_string(value)

```


### <a name="send_rfc_3339_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_rfc_3339_date_time_array") send_rfc_3339_date_time_array

> TODO: Add a method description

```python
def send_rfc_3339_date_time_array(self,
                                      datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
datetimes_value = ["1994-02-13T14:01:54.9571247Z","1994-02-13T14:01:54.9571247Z"]
datetimes = json.loads(datetimes_value)

result = form_params_client.send_rfc_3339_date_time_array(datetimes)

```


### <a name="send_mixed_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_mixed_array") send_mixed_array

> Send a variety for form params. Returns file count and body params

```python
def send_mixed_array(self,
                         options=dict())
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | TODO: Add a parameter description |
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |
| models |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
collect = {}

file = open("pathtofile", 'rb')
collect['file'] = file

integers_value = "[1,2,3,4,5]"
integers = json.loads(integers_value)
collect['integers'] = integers

models_value = "[{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"},{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}]"
models = json.loads(models_value)
collect['models'] = models

strings_value = '["abc", "def"]'
strings = json.loads(strings_value)
collect['strings'] = strings


result = form_params_client.send_mixed_array(collect)

```


### <a name="send_integer_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_integer_enum_array") send_integer_enum_array

> TODO: Add a method description

```python
def send_integer_enum_array(self,
                                suites)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| suites |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
suites = [SuiteCode.HEARTS,SuiteCode.CLUBS,SuiteCode.DIAMONDS,SuiteCode.SPADES,SuiteCode.CLUBS]

result = form_params_client.send_integer_enum_array(suites)

```


### <a name="send_string_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".FormParamsController.send_string_enum_array") send_string_enum_array

> TODO: Add a method description

```python
def send_string_enum_array(self,
                               days)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| days |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
days = [Days.TUESDAY,Days.SATURDAY,Days.MONDAY,Days.SUNDAY]

result = form_params_client.send_string_enum_array(days)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="query_param_controller"></a>![Class: ](https://apidocs.io/img/class.png ".QueryParamController") QueryParamController

### Get controller instance

An instance of the ``` QueryParamController ``` class can be accessed from the API Client.

```python
 query_param_client = client.query_param
```

### <a name="date_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.date_array") date_array

> TODO: Add a method description

```python
def date_array(self,
                   dates)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dates |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
dates_value = ["1994-02-13","1994-02-13"]
dates = json.loads(dates_value)

result = query_param_client.date_array(dates)

```


### <a name="date"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.date") date

> TODO: Add a method description

```python
def date(self,
                date)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| date |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
date = 1994-02-13

result = query_param_client.date(date)

```


### <a name="unix_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.unix_date_time_array") unix_date_time_array

> TODO: Add a method description

```python
def unix_date_time_array(self,
                             datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
datetimes_value = [1484719381,1484719381]
datetimes = json.loads(datetimes_value)

result = query_param_client.unix_date_time_array(datetimes)

```


### <a name="unix_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.unix_date_time") unix_date_time

> TODO: Add a method description

```python
def unix_date_time(self,
                       datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
datetime = 1484719381

result = query_param_client.unix_date_time(datetime)

```


### <a name="rfc_1123_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.rfc_1123_date_time") rfc_1123_date_time

> TODO: Add a method description

```python
def rfc_1123_date_time(self,
                           datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
datetime = Sun, 06 Nov 1994 08:49:37 GMT

result = query_param_client.rfc_1123_date_time(datetime)

```


### <a name="rfc_1123_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.rfc_1123_date_time_array") rfc_1123_date_time_array

> TODO: Add a method description

```python
def rfc_1123_date_time_array(self,
                                 datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
datetimes_value = ["Sun, 06 Nov 1994 08:49:37 GMT","Sun, 06 Nov 1994 08:49:37 GMT"]
datetimes = json.loads(datetimes_value)

result = query_param_client.rfc_1123_date_time_array(datetimes)

```


### <a name="rfc_3339_date_time_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.rfc_3339_date_time_array") rfc_3339_date_time_array

> TODO: Add a method description

```python
def rfc_3339_date_time_array(self,
                                 datetimes)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
datetimes_value = ["1994-02-13T14:01:54.9571247Z","1994-02-13T14:01:54.9571247Z"]
datetimes = json.loads(datetimes_value)

result = query_param_client.rfc_3339_date_time_array(datetimes)

```


### <a name="rfc_3339_date_time"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.rfc_3339_date_time") rfc_3339_date_time

> TODO: Add a method description

```python
def rfc_3339_date_time(self,
                           datetime)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
datetime = 1994-02-13T14:01:54.9571247Z

result = query_param_client.rfc_3339_date_time(datetime)

```


### <a name="no_params"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.no_params") no_params

> TODO: Add a method description

```python
def no_params(self)
```

#### Example Usage

```python

result = query_param_client.no_params()

```


### <a name="string_param"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.string_param") string_param

> TODO: Add a method description

```python
def string_param(self,
                     string)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| string |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
string = 'l;asd;asdwe[2304&&;\'.d??\\a\\\\\\;sd//'

result = query_param_client.string_param(string)

```


### <a name="url_param"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.url_param") url_param

> TODO: Add a method description

```python
def url_param(self,
                  url)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| url |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
url = 'https://www.shahidisawesome.com/and/also/a/narcissist?thisis=aparameter&another=one'

result = query_param_client.url_param(url)

```


### <a name="number_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.number_array") number_array

> TODO: Add a method description

```python
def number_array(self,
                     integers)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
integers_value = "[1,2,3,4,5]"
integers = json.loads(integers_value)

result = query_param_client.number_array(integers)

```


### <a name="string_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.string_array") string_array

> TODO: Add a method description

```python
def string_array(self,
                     strings)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
strings_value = '["abc", "def"]'
strings = json.loads(strings_value)

result = query_param_client.string_array(strings)

```


### <a name="simple_query"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.simple_query") simple_query

> TODO: Add a method description

```python
def simple_query(self,
                     boolean,
                     number,
                     string,
                     _optional_query_parameters=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| boolean |  ``` Required ```  | TODO: Add a parameter description |
| number |  ``` Required ```  | TODO: Add a parameter description |
| string |  ``` Required ```  | TODO: Add a parameter description |
| _optional_query_parameters | ``` Optional ``` | Additional optional query parameters are supported by this method |



#### Example Usage

```python
boolean = True
number = 4
string = 'TestString'
# key-value map for optional query parameters
optional_query_parameters = { }


result = query_param_client.simple_query(boolean, number, string, optional_query_parameters)

```


### <a name="string_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.string_enum_array") string_enum_array

> TODO: Add a method description

```python
def string_enum_array(self,
                          days)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| days |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
days = [Days.TUESDAY,Days.SATURDAY,Days.MONDAY,Days.SUNDAY]

result = query_param_client.string_enum_array(days)

```


### <a name="multiple_params"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.multiple_params") multiple_params

> TODO: Add a method description

```python
def multiple_params(self,
                        number,
                        precision,
                        string,
                        url)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| number |  ``` Required ```  | TODO: Add a parameter description |
| precision |  ``` Required ```  | TODO: Add a parameter description |
| string |  ``` Required ```  | TODO: Add a parameter description |
| url |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
number = 123412312
precision = 1112.34
string = '""test./;";12&&3asl"";"qw1&34"///..//.'
url = 'http://www.abc.com/test?a=b&c="http://lolol.com?param=no&another=lol"'

result = query_param_client.multiple_params(number, precision, string, url)

```


### <a name="integer_enum_array"></a>![Method: ](https://apidocs.io/img/method.png ".QueryParamController.integer_enum_array") integer_enum_array

> TODO: Add a method description

```python
def integer_enum_array(self,
                           suites)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| suites |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
suites = [SuiteCode.HEARTS,SuiteCode.CLUBS,SuiteCode.DIAMONDS,SuiteCode.SPADES,SuiteCode.CLUBS]

result = query_param_client.integer_enum_array(suites)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="error_codes_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ErrorCodesController") ErrorCodesController

### Get controller instance

An instance of the ``` ErrorCodesController ``` class can be accessed from the API Client.

```python
 error_codes_client = client.error_codes
```

### <a name="get_400"></a>![Method: ](https://apidocs.io/img/method.png ".ErrorCodesController.get_400") get_400

> TODO: Add a method description

```python
def get_400(self)
```

#### Example Usage

```python

result = error_codes_client.get_400()

```


### <a name="get_500"></a>![Method: ](https://apidocs.io/img/method.png ".ErrorCodesController.get_500") get_500

> TODO: Add a method description

```python
def get_500(self)
```

#### Example Usage

```python

result = error_codes_client.get_500()

```


### <a name="get_401"></a>![Method: ](https://apidocs.io/img/method.png ".ErrorCodesController.get_401") get_401

> TODO: Add a method description

```python
def get_401(self)
```

#### Example Usage

```python

result = error_codes_client.get_401()

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

### Get controller instance

An instance of the ``` EchoController ``` class can be accessed from the API Client.

```python
 echo_client = client.echo
```

### <a name="json_echo"></a>![Method: ](https://apidocs.io/img/method.png ".EchoController.json_echo") json_echo

> Echo's back the request

```python
def json_echo(self,
                  input)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| input |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
input_value = "{\"uid\": \"1123213\", \"name\": \"Shahid\"}"
input = json.loads(input_value)

result = echo_client.json_echo(input)

```


### <a name="form_echo"></a>![Method: ](https://apidocs.io/img/method.png ".EchoController.form_echo") form_echo

> Sends the request including any form params as JSON

```python
def form_echo(self,
                  input)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| input |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
input_value = "{\"uid\": \"1123213\", \"name\": \"Shahid\"}"
input = json.loads(input_value)

result = echo_client.form_echo(input)

```


### <a name="query_echo"></a>![Method: ](https://apidocs.io/img/method.png ".EchoController.query_echo") query_echo

> TODO: Add a method description

```python
def query_echo(self,
                   _optional_query_parameters=None)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| _optional_query_parameters | ``` Optional ``` | Additional optional query parameters are supported by this method |



#### Example Usage

```python
# key-value map for optional query parameters
optional_query_parameters = { }


result = echo_client.query_echo(optional_query_parameters)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="header_controller"></a>![Class: ](https://apidocs.io/img/class.png ".HeaderController") HeaderController

### Get controller instance

An instance of the ``` HeaderController ``` class can be accessed from the API Client.

```python
 header_client = client.header
```

### <a name="send_headers"></a>![Method: ](https://apidocs.io/img/method.png ".HeaderController.send_headers") send_headers

> Sends a single header params

```python
def send_headers(self,
                     custom_header,
                     value)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| customHeader |  ``` Required ```  | TODO: Add a parameter description |
| value |  ``` Required ```  | Represents the value of the custom header |



#### Example Usage

```python
custom_header = 'TestString'
value = 'TestString'

result = header_client.send_headers(custom_header, value)

```


[Back to List of Controllers](#list_of_controllers)

## <a name="template_params_controller"></a>![Class: ](https://apidocs.io/img/class.png ".TemplateParamsController") TemplateParamsController

### Get controller instance

An instance of the ``` TemplateParamsController ``` class can be accessed from the API Client.

```python
 template_params_client = client.template_params
```

### <a name="send_string_array"></a>![Method: ](https://apidocs.io/img/method.png ".TemplateParamsController.send_string_array") send_string_array

> TODO: Add a method description

```python
def send_string_array(self,
                          strings)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
strings_value = '["abc", "def"]'
strings = json.loads(strings_value)

result = template_params_client.send_string_array(strings)

```


### <a name="send_integer_array"></a>![Method: ](https://apidocs.io/img/method.png ".TemplateParamsController.send_integer_array") send_integer_array

> TODO: Add a method description

```python
def send_integer_array(self,
                           integers)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |



#### Example Usage

```python
integers_value = "[1,2,3,4,5]"
integers = json.loads(integers_value)

result = template_params_client.send_integer_array(integers)

```


[Back to List of Controllers](#list_of_controllers)



