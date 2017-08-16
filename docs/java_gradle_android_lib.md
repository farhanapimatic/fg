# Getting started

Testing various
 api 
features

## How to Build

The generated code uses a few Gradle dependencies e.g., Jackson, Volley,
and Apache HttpClient. The reference to these dependencies is already
added in the build.gradle file will be installed automatically. Therefore,
you will need internet access for a successful build.

* In order to open the client library in Android Studio click on ``` Open an Existing Android Project ```.

![Importing SDK into Android Studio - Step 1](https://apidocs.io/illustration/android?step=import1&workspaceFolder=Tester&workspaceName=Tester&projectName=TesterLib&rootNamespace=org.hopto.apimatic)

* Browse to locate the folder containing the source code. Select the location of the Tester gradle project and click ``` Ok ```.

![Importing SDK into Android Studio - Step 2](https://apidocs.io/illustration/android?step=import2&workspaceFolder=Tester&workspaceName=Tester&projectName=TesterLib&rootNamespace=org.hopto.apimatic)

* Upon successful import, the project can be built by clicking on ``` Build > Make Project ``` or  pressing ``` Ctrl + F9 ```.

![Importing SDK into Android Studio - Step 3](https://apidocs.io/illustration/android?step=import3&workspaceFolder=Tester&workspaceName=Tester&projectName=TesterLib&rootNamespace=org.hopto.apimatic)

## How to Use

The following section explains how to use the Tester library in a new project.

### 1. Starting a new project 

For starting a new project, click on ``` Create New Android Studio Project ```.

![Add a new project in Android Studio - Step 1](https://apidocs.io/illustration/android?step=createNewProject0&workspaceFolder=Tester&workspaceName=Tester&projectName=TesterLib&rootNamespace=org.hopto.apimatic)

Here, configure the new project by adding the name, domain and location of the sample application followed by clicking ``` Next ```.

![Create a new Android Studio Project - Step 2](https://apidocs.io/illustration/android?step=createNewProject1&workspaceFolder=Tester&workspaceName=Tester&projectName=TesterLib&rootNamespace=org.hopto.apimatic)

Following this, select the ``` Phone and Tablet ```` option as shown in the illustration below and click ``` Next ```. 

![Create a new Android Studio Project - Step 3](https://apidocs.io/illustration/android?step=createNewProject2&workspaceFolder=Tester&workspaceName=Tester&projectName=TesterLib&rootNamespace=org.hopto.apimatic)

In the following step, choose ``` Empty Activity ``` as the activity type and click ``` Next ```.

![Create a new Android Studio Project - Step 4](https://apidocs.io/illustration/android?step=createNewProject3&workspaceFolder=Tester&workspaceName=Tester&projectName=TesterLib&rootNamespace=org.hopto.apimatic)

In this step, provide an ``` Activity Name ``` and ``` Layout Name ``` and click ``` Finish ```.  This would take you to the newly created project.

![Create a new Android Studio Project - Step 4](https://apidocs.io/illustration/android?step=createNewProject4&workspaceFolder=Tester&workspaceName=Tester&projectName=TesterLib&rootNamespace=org.hopto.apimatic)

### 2. Add reference of the library project

In order to add a dependency to this sample application, click on the android button shown in the project explorer on the left side as shown in the picture. Click on ``` Project ``` in the drop down that emerges.  

![Adding dependency to the client library - Step 1](https://apidocs.io/illustration/android?step=testProject0&workspaceFolder=Tester&workspaceName=Tester&projectName=TesterLib&rootNamespace=org.hopto.apimatic)

Right click the sample application in the project explorer and click on ``` New > Module ```  as shown in the picture.

![Adding dependency to the client library - Step 2](https://apidocs.io/illustration/android?step=testProject1&workspaceFolder=Tester&workspaceName=Tester&projectName=TesterLib&rootNamespace=org.hopto.apimatic)

Choose ``` Import Gradle Project ``` and click ``` Next ```.

![Adding dependency to the client library - Step 3](https://apidocs.io/illustration/android?step=testProject2&workspaceFolder=Tester&workspaceName=Tester&projectName=TesterLib&rootNamespace=org.hopto.apimatic)

Click on ``` Finish ``` which would take you back to the sample application with the refernced SDK. 

![Adding dependency to the client library - Step 4](https://apidocs.io/illustration/android?step=testProject3&workspaceFolder=Tester&workspaceName=Tester&projectName=TesterLib&rootNamespace=org.hopto.apimatic)

In the following step naigate to the ``` SampleApplication >  app > build.gradle ``` file and add the following line ```compile project(path: ':Tester')``` to the dependencies section as shown in the illustration below.

![Adding dependency to the client library - Step 5](https://apidocs.io/illustration/android?step=testProject4&workspaceFolder=Tester&workspaceName=Tester&projectName=TesterLib&rootNamespace=org.hopto.apimatic)

Finally, press ``` Sync Now ``` in the warning visible as shown in the picture below.

![Adding dependency to the client library - Step 6](https://apidocs.io/illustration/android?step=testProject5&workspaceFolder=Tester&workspaceName=Tester&projectName=TesterLib&rootNamespace=org.hopto.apimatic)

### 3. Write sample code

Once the ``` SampleApplication ``` is created, a file named ``` SampleApplication > app > src > main > java > MainActivity ``` will be visible in the *Project Explorer* with an ``` onCreate ``` method. This is the entry point for the execution of the created project.
Here, you can add code to initialize the client library and instantiate a *Controller* class. Sample code to initialize the client library and using controller methods is given in the subsequent sections.

## How to Test

The generated code and the server can be tested using automatically generated test cases. 
JUnit is used as the testing framework and test runner.

In Android Studio, for running the tests do the following:

1. Right click on *SampleApplication > TesterLib > androidTest > java)* from the project explorer.
2. Select "Run All Tests" or use "Ctrl + Shift + F10" to run the Tests.

## Initialization

### 

API client can be initialized as following. The `appContext` being passed is the Android application [`Context`](https://developer.android.com/reference/android/content/Context.html).

```java

org.hopto.apimatic.Configuration.initialize(appContext);
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

## <a name="response_types_controller"></a>![Class: ](https://apidocs.io/img/class.png "org.hopto.apimatic.controllers.ResponseTypesController") ResponseTypesController

### Get singleton instance

The singleton instance of the ``` ResponseTypesController ``` class can be accessed from the API Client.

```java
ResponseTypesController responseTypes = client.getResponseTypes();
```

### <a name="get_date_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.getDateArrayAsync") getDateArrayAsync

> TODO: Add a method description


```java
void getDateArrayAsync(final APICallBack<List<Date>> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.getDateArrayAsync(new APICallBack<List<Date>>() {
    public void onSuccess(HttpContext context, List<Date> response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_date_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.getDateAsync") getDateAsync

> TODO: Add a method description


```java
void getDateAsync(final APICallBack<Date> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.getDateAsync(new APICallBack<Date>() {
    public void onSuccess(HttpContext context, Date response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_long_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.getLongAsync") getLongAsync

> TODO: Add a method description


```java
void getLongAsync(final APICallBack<Long> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.getLongAsync(new APICallBack<Long>() {
    public void onSuccess(HttpContext context, Long response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_model_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.getModelAsync") getModelAsync

> TODO: Add a method description


```java
void getModelAsync(final APICallBack<Person> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.getModelAsync(new APICallBack<Person>() {
    public void onSuccess(HttpContext context, Person response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_string_enum_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.getStringEnumArrayAsync") getStringEnumArrayAsync

> TODO: Add a method description


```java
void getStringEnumArrayAsync(final APICallBack<List<Days>> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.getStringEnumArrayAsync(new APICallBack<List<Days>>() {
    public void onSuccess(HttpContext context, List<Days> response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_string_enum_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.getStringEnumAsync") getStringEnumAsync

> TODO: Add a method description


```java
void getStringEnumAsync(final APICallBack<Days> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.getStringEnumAsync(new APICallBack<Days>() {
    public void onSuccess(HttpContext context, Days response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_model_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.getModelArrayAsync") getModelArrayAsync

> TODO: Add a method description


```java
void getModelArrayAsync(final APICallBack<List<Person>> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.getModelArrayAsync(new APICallBack<List<Person>>() {
    public void onSuccess(HttpContext context, List<Person> response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_int_enum_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.getIntEnumAsync") getIntEnumAsync

> TODO: Add a method description


```java
void getIntEnumAsync(final APICallBack<SuiteCode> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.getIntEnumAsync(new APICallBack<SuiteCode>() {
    public void onSuccess(HttpContext context, SuiteCode response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_int_enum_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.getIntEnumArrayAsync") getIntEnumArrayAsync

> TODO: Add a method description


```java
void getIntEnumArrayAsync(final APICallBack<List<SuiteCode>> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.getIntEnumArrayAsync(new APICallBack<List<SuiteCode>>() {
    public void onSuccess(HttpContext context, List<SuiteCode> response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_precision_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.getPrecisionAsync") getPrecisionAsync

> TODO: Add a method description


```java
void getPrecisionAsync(final APICallBack<Double> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.getPrecisionAsync(new APICallBack<Double>() {
    public void onSuccess(HttpContext context, Double response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_binary_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.getBinaryAsync") getBinaryAsync

> gets a binary object


```java
void getBinaryAsync(final APICallBack<InputStream> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.getBinaryAsync(new APICallBack<InputStream>() {
    public void onSuccess(HttpContext context, InputStream response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_integer_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.getIntegerAsync") getIntegerAsync

> Gets a integer response


```java
void getIntegerAsync(final APICallBack<Integer> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.getIntegerAsync(new APICallBack<Integer>() {
    public void onSuccess(HttpContext context, Integer response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_integer_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.getIntegerArrayAsync") getIntegerArrayAsync

> Get an array of integers.


```java
void getIntegerArrayAsync(final APICallBack<List<Integer>> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.getIntegerArrayAsync(new APICallBack<List<Integer>>() {
    public void onSuccess(HttpContext context, List<Integer> response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_dynamic_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.getDynamicAsync") getDynamicAsync

> TODO: Add a method description


```java
void getDynamicAsync(final APICallBack<DynamicResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.getDynamicAsync(new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_dynamic_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.getDynamicArrayAsync") getDynamicArrayAsync

> TODO: Add a method description


```java
void getDynamicArrayAsync(final APICallBack<DynamicResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.getDynamicArrayAsync(new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get3339_datetime_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.get3339DatetimeAsync") get3339DatetimeAsync

> TODO: Add a method description


```java
void get3339DatetimeAsync(final APICallBack<Date> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.get3339DatetimeAsync(new APICallBack<Date>() {
    public void onSuccess(HttpContext context, Date response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get3339_datetime_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.get3339DatetimeArrayAsync") get3339DatetimeArrayAsync

> TODO: Add a method description


```java
void get3339DatetimeArrayAsync(final APICallBack<List<Date>> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.get3339DatetimeArrayAsync(new APICallBack<List<Date>>() {
    public void onSuccess(HttpContext context, List<Date> response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_boolean_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.getBooleanAsync") getBooleanAsync

> TODO: Add a method description


```java
void getBooleanAsync(final APICallBack<Boolean> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.getBooleanAsync(new APICallBack<Boolean>() {
    public void onSuccess(HttpContext context, Boolean response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_boolean_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.getBooleanArrayAsync") getBooleanArrayAsync

> TODO: Add a method description


```java
void getBooleanArrayAsync(final APICallBack<List<Boolean>> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.getBooleanArrayAsync(new APICallBack<List<Boolean>>() {
    public void onSuccess(HttpContext context, List<Boolean> response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_headers_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.getHeadersAsync") getHeadersAsync

> TODO: Add a method description


```java
void getHeadersAsync(final APICallBack<Object> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.getHeadersAsync(new APICallBack<void>() {
    public void onSuccess(HttpContext context, void response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get1123_date_time_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.get1123DateTimeAsync") get1123DateTimeAsync

> TODO: Add a method description


```java
void get1123DateTimeAsync(final APICallBack<Date> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.get1123DateTimeAsync(new APICallBack<Date>() {
    public void onSuccess(HttpContext context, Date response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_unix_date_time_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.getUnixDateTimeAsync") getUnixDateTimeAsync

> TODO: Add a method description


```java
void getUnixDateTimeAsync(final APICallBack<Date> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.getUnixDateTimeAsync(new APICallBack<Date>() {
    public void onSuccess(HttpContext context, Date response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get1123_date_time_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.get1123DateTimeArrayAsync") get1123DateTimeArrayAsync

> TODO: Add a method description


```java
void get1123DateTimeArrayAsync(final APICallBack<List<Date>> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.get1123DateTimeArrayAsync(new APICallBack<List<Date>>() {
    public void onSuccess(HttpContext context, List<Date> response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get_unix_date_time_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ResponseTypesController.getUnixDateTimeArrayAsync") getUnixDateTimeArrayAsync

> TODO: Add a method description


```java
void getUnixDateTimeArrayAsync(final APICallBack<List<Date>> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
responseTypes.getUnixDateTimeArrayAsync(new APICallBack<List<Date>>() {
    public void onSuccess(HttpContext context, List<Date> response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="body_params_controller"></a>![Class: ](https://apidocs.io/img/class.png "org.hopto.apimatic.controllers.BodyParamsController") BodyParamsController

### Get singleton instance

The singleton instance of the ``` BodyParamsController ``` class can be accessed from the API Client.

```java
BodyParamsController bodyParams = client.getBodyParams();
```

### <a name="send_date_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.BodyParamsController.sendDateArrayAsync") sendDateArrayAsync

> TODO: Add a method description


```java
void sendDateArrayAsync(
        final List<Date> dates,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dates |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String datesValue = ["1994-02-13", "1994-02-13"];
    List<Date> dates = mapper.readValue(datesValue,new TypeReference<List<Date>> (){});
    // Invoking the API call with sample inputs
    bodyParams.sendDateArrayAsync(dates, new APICallBack<ServerResponse>() {
        public void onSuccess(HttpContext context, ServerResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="send_date_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.BodyParamsController.sendDateAsync") sendDateAsync

> TODO: Add a method description


```java
void sendDateAsync(
        final Date date,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| date |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
Date date = 1994-02-13;
// Invoking the API call with sample inputs
bodyParams.sendDateAsync(date, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="send_unix_date_time_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.BodyParamsController.sendUnixDateTimeAsync") sendUnixDateTimeAsync

> TODO: Add a method description


```java
void sendUnixDateTimeAsync(
        final Date datetime,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
Date datetime = 1484719381;
// Invoking the API call with sample inputs
bodyParams.sendUnixDateTimeAsync(datetime, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="send_rfc1123_date_time_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.BodyParamsController.sendRfc1123DateTimeAsync") sendRfc1123DateTimeAsync

> TODO: Add a method description


```java
void sendRfc1123DateTimeAsync(
        final Date datetime,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
Date datetime = Sun, 06 Nov 1994 08:49:37 GMT;
// Invoking the API call with sample inputs
bodyParams.sendRfc1123DateTimeAsync(datetime, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="send_rfc3339_date_time_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.BodyParamsController.sendRfc3339DateTimeAsync") sendRfc3339DateTimeAsync

> TODO: Add a method description


```java
void sendRfc3339DateTimeAsync(
        final Date datetime,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
Date datetime = 1994-02-13T14:01:54.9571247Z;
// Invoking the API call with sample inputs
bodyParams.sendRfc3339DateTimeAsync(datetime, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="send_unix_date_time_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.BodyParamsController.sendUnixDateTimeArrayAsync") sendUnixDateTimeArrayAsync

> TODO: Add a method description


```java
void sendUnixDateTimeArrayAsync(
        final List<Date> datetimes,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String datetimesValue = [1484719381,1484719381];
    List<Date> datetimes = mapper.readValue(datetimesValue,new TypeReference<List<Date>> (){});
    // Invoking the API call with sample inputs
    bodyParams.sendUnixDateTimeArrayAsync(datetimes, new APICallBack<ServerResponse>() {
        public void onSuccess(HttpContext context, ServerResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="send_rfc1123_date_time_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.BodyParamsController.sendRfc1123DateTimeArrayAsync") sendRfc1123DateTimeArrayAsync

> TODO: Add a method description


```java
void sendRfc1123DateTimeArrayAsync(
        final List<Date> datetimes,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String datetimesValue = ["Sun, 06 Nov 1994 08:49:37 GMT","Sun, 06 Nov 1994 08:49:37 GMT"];
    List<Date> datetimes = mapper.readValue(datetimesValue,new TypeReference<List<Date>> (){});
    // Invoking the API call with sample inputs
    bodyParams.sendRfc1123DateTimeArrayAsync(datetimes, new APICallBack<ServerResponse>() {
        public void onSuccess(HttpContext context, ServerResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="send_rfc3339_date_time_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.BodyParamsController.sendRfc3339DateTimeArrayAsync") sendRfc3339DateTimeArrayAsync

> TODO: Add a method description


```java
void sendRfc3339DateTimeArrayAsync(
        final List<Date> datetimes,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String datetimesValue = ["1994-02-13T14:01:54.9571247Z","1994-02-13T14:01:54.9571247Z"];
    List<Date> datetimes = mapper.readValue(datetimesValue,new TypeReference<List<Date>> (){});
    // Invoking the API call with sample inputs
    bodyParams.sendRfc3339DateTimeArrayAsync(datetimes, new APICallBack<ServerResponse>() {
        public void onSuccess(HttpContext context, ServerResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="send_string_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.BodyParamsController.sendStringArrayAsync") sendStringArrayAsync

> sends a string body param


```java
void sendStringArrayAsync(
        final List<String> sarray,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| sarray |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String sarrayValue = "[\"abc\", \"def\"]";
    List<String> sarray = mapper.readValue(sarrayValue,new TypeReference<List<String>> (){});
    // Invoking the API call with sample inputs
    bodyParams.sendStringArrayAsync(sarray, new APICallBack<ServerResponse>() {
        public void onSuccess(HttpContext context, ServerResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="send_integer_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.BodyParamsController.sendIntegerArrayAsync") sendIntegerArrayAsync

> TODO: Add a method description


```java
void sendIntegerArrayAsync(
        final List<Integer> integers,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String integersValue = "[1,2,3,4,5]";
    List<Integer> integers = mapper.readValue(integersValue,new TypeReference<List<Integer>> (){});
    // Invoking the API call with sample inputs
    bodyParams.sendIntegerArrayAsync(integers, new APICallBack<ServerResponse>() {
        public void onSuccess(HttpContext context, ServerResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="send_model_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.BodyParamsController.sendModelAsync") sendModelAsync

> TODO: Add a method description


```java
void sendModelAsync(
        final Employee model,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| model |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String modelValue = "{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}";
    Employee model = mapper.readValue(modelValue,new TypeReference<Employee> (){});
    // Invoking the API call with sample inputs
    bodyParams.sendModelAsync(model, new APICallBack<ServerResponse>() {
        public void onSuccess(HttpContext context, ServerResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="send_model_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.BodyParamsController.sendModelArrayAsync") sendModelArrayAsync

> TODO: Add a method description


```java
void sendModelArrayAsync(
        final List<Employee> models,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| models |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String modelsValue = "[{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"},{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}]";
    List<Employee> models = mapper.readValue(modelsValue,new TypeReference<List<Employee>> (){});
    // Invoking the API call with sample inputs
    bodyParams.sendModelArrayAsync(models, new APICallBack<ServerResponse>() {
        public void onSuccess(HttpContext context, ServerResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="send_dynamic_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.BodyParamsController.sendDynamicAsync") sendDynamicAsync

> TODO: Add a method description


```java
void sendDynamicAsync(
        final Object dynamic,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dynamic |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String dynamicValue = "{\"uid\": \"1123213\", \"name\": \"Shahid\"}";
    Object dynamic = mapper.readValue(dynamicValue,new TypeReference<Object> (){});
    // Invoking the API call with sample inputs
    bodyParams.sendDynamicAsync(dynamic, new APICallBack<ServerResponse>() {
        public void onSuccess(HttpContext context, ServerResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="send_string_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.BodyParamsController.sendStringAsync") sendStringAsync

> TODO: Add a method description


```java
void sendStringAsync(
        final String value,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| value |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
String value = "TestString";
// Invoking the API call with sample inputs
bodyParams.sendStringAsync(value, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="send_string_enum_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.BodyParamsController.sendStringEnumArrayAsync") sendStringEnumArrayAsync

> TODO: Add a method description


```java
void sendStringEnumArrayAsync(
        final List<Days> days,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| days |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String daysValue = "[\"Tuesday\", \"Saturday\", \"Wednesday\", \"Monday\", \"Sunday\"]";
    List<Days> days = mapper.readValue(daysValue,new TypeReference<List<Days>> (){});
    // Invoking the API call with sample inputs
    bodyParams.sendStringEnumArrayAsync(days, new APICallBack<ServerResponse>() {
        public void onSuccess(HttpContext context, ServerResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="send_integer_enum_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.BodyParamsController.sendIntegerEnumArrayAsync") sendIntegerEnumArrayAsync

> TODO: Add a method description


```java
void sendIntegerEnumArrayAsync(
        final List<SuiteCode> suites,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| suites |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String suitesValue = "[1, 3, 4, 2, 3]";
    List<SuiteCode> suites = mapper.readValue(suitesValue,new TypeReference<List<SuiteCode>> (){});
    // Invoking the API call with sample inputs
    bodyParams.sendIntegerEnumArrayAsync(suites, new APICallBack<ServerResponse>() {
        public void onSuccess(HttpContext context, ServerResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


[Back to List of Controllers](#list_of_controllers)

## <a name="form_params_controller"></a>![Class: ](https://apidocs.io/img/class.png "org.hopto.apimatic.controllers.FormParamsController") FormParamsController

### Get singleton instance

The singleton instance of the ``` FormParamsController ``` class can be accessed from the API Client.

```java
FormParamsController formParams = client.getFormParams();
```

### <a name="send_date_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.FormParamsController.sendDateArrayAsync") sendDateArrayAsync

> TODO: Add a method description


```java
void sendDateArrayAsync(
        final List<Date> dates,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dates |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
String datesValue = ["1994-02-13","1994-02-13"];
List<Date> dates = mapper.readValue(datesValue,new TypeReference<List<Date>> (){});
// Invoking the API call with sample inputs
formParams.sendDateArrayAsync(dates, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="send_date_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.FormParamsController.sendDateAsync") sendDateAsync

> TODO: Add a method description


```java
void sendDateAsync(
        final Date date,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| date |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
Date date = 1994-02-13;
// Invoking the API call with sample inputs
formParams.sendDateAsync(date, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="send_unix_date_time_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.FormParamsController.sendUnixDateTimeAsync") sendUnixDateTimeAsync

> TODO: Add a method description


```java
void sendUnixDateTimeAsync(
        final Date datetime,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
Date datetime = 1484719381;
// Invoking the API call with sample inputs
formParams.sendUnixDateTimeAsync(datetime, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="send_rfc1123_date_time_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.FormParamsController.sendRfc1123DateTimeAsync") sendRfc1123DateTimeAsync

> TODO: Add a method description


```java
void sendRfc1123DateTimeAsync(
        final Date datetime,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
Date datetime = Sun, 06 Nov 1994 08:49:37 GMT;
// Invoking the API call with sample inputs
formParams.sendRfc1123DateTimeAsync(datetime, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="send_rfc3339_date_time_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.FormParamsController.sendRfc3339DateTimeAsync") sendRfc3339DateTimeAsync

> TODO: Add a method description


```java
void sendRfc3339DateTimeAsync(
        final Date datetime,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
Date datetime = 1994-02-13T14:01:54.9571247Z;
// Invoking the API call with sample inputs
formParams.sendRfc3339DateTimeAsync(datetime, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="send_unix_date_time_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.FormParamsController.sendUnixDateTimeArrayAsync") sendUnixDateTimeArrayAsync

> TODO: Add a method description


```java
void sendUnixDateTimeArrayAsync(
        final List<Date> datetimes,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
String datetimesValue = [1484719381,1484719381];
List<Date> datetimes = mapper.readValue(datetimesValue,new TypeReference<List<Date>> (){});
// Invoking the API call with sample inputs
formParams.sendUnixDateTimeArrayAsync(datetimes, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="send_rfc1123_date_time_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.FormParamsController.sendRfc1123DateTimeArrayAsync") sendRfc1123DateTimeArrayAsync

> TODO: Add a method description


```java
void sendRfc1123DateTimeArrayAsync(
        final List<Date> datetimes,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
String datetimesValue = ["Sun, 06 Nov 1994 08:49:37 GMT","Sun, 06 Nov 1994 08:49:37 GMT"];
List<Date> datetimes = mapper.readValue(datetimesValue,new TypeReference<List<Date>> (){});
// Invoking the API call with sample inputs
formParams.sendRfc1123DateTimeArrayAsync(datetimes, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="send_long_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.FormParamsController.sendLongAsync") sendLongAsync

> TODO: Add a method description


```java
void sendLongAsync(
        final long value,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| value |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
long value = 5147483647L;
// Invoking the API call with sample inputs
formParams.sendLongAsync(value, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="send_integer_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.FormParamsController.sendIntegerArrayAsync") sendIntegerArrayAsync

> TODO: Add a method description


```java
void sendIntegerArrayAsync(
        final List<Integer> integers,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
String integersValue = "[1,2,3,4,5]";
List<Integer> integers = mapper.readValue(integersValue,new TypeReference<List<Integer>> (){});
// Invoking the API call with sample inputs
formParams.sendIntegerArrayAsync(integers, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="send_string_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.FormParamsController.sendStringArrayAsync") sendStringArrayAsync

> TODO: Add a method description


```java
void sendStringArrayAsync(
        final List<String> strings,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
String stringsValue = "[\"abc\", \"def\"]";
List<String> strings = mapper.readValue(stringsValue,new TypeReference<List<String>> (){});
// Invoking the API call with sample inputs
formParams.sendStringArrayAsync(strings, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="send_model_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.FormParamsController.sendModelAsync") sendModelAsync

> TODO: Add a method description


```java
void sendModelAsync(
        final Employee model,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| model |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
String modelValue = "{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}";
Employee model = mapper.readValue(modelValue,new TypeReference<Employee> (){});
// Invoking the API call with sample inputs
formParams.sendModelAsync(model, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="send_model_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.FormParamsController.sendModelArrayAsync") sendModelArrayAsync

> TODO: Add a method description


```java
void sendModelArrayAsync(
        final List<Employee> models,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| models |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
String modelsValue = "[{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"},{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}]";
List<Employee> models = mapper.readValue(modelsValue,new TypeReference<List<Employee>> (){});
// Invoking the API call with sample inputs
formParams.sendModelArrayAsync(models, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="send_file_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.FormParamsController.sendFileAsync") sendFileAsync

> TODO: Add a method description


```java
void sendFileAsync(
        final File file,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
File file = new File("PathToFile");
// Invoking the API call with sample inputs
formParams.sendFileAsync(file, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="send_string_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.FormParamsController.sendStringAsync") sendStringAsync

> TODO: Add a method description


```java
void sendStringAsync(
        final String value,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| value |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
String value = "TestString";
// Invoking the API call with sample inputs
formParams.sendStringAsync(value, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="send_rfc3339_date_time_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.FormParamsController.sendRfc3339DateTimeArrayAsync") sendRfc3339DateTimeArrayAsync

> TODO: Add a method description


```java
void sendRfc3339DateTimeArrayAsync(
        final List<Date> datetimes,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
String datetimesValue = ["1994-02-13T14:01:54.9571247Z","1994-02-13T14:01:54.9571247Z"];
List<Date> datetimes = mapper.readValue(datetimesValue,new TypeReference<List<Date>> (){});
// Invoking the API call with sample inputs
formParams.sendRfc3339DateTimeArrayAsync(datetimes, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="send_mixed_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.FormParamsController.sendMixedArrayAsync") sendMixedArrayAsync

> Send a variety for form params. Returns file count and body params


```java
void sendMixedArrayAsync(
        final SendMixedArrayInput input,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| file |  ``` Required ```  | TODO: Add a parameter description |
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |
| models |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
SendMixedArrayInput collect = new SendMixedArrayInput();

File file = new File("PathToFile");
collect.setFile(file);

String integersValue = "[1,2,3,4,5]";
List<Integer> integers = mapper.readValue(integersValue,new TypeReference<List<Integer>> (){});
collect.setIntegers(integers);

String modelsValue = "[{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"},{\"name\":\"Shahid Khaliq\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"boss\":{\"personType\":\"Boss\",\"name\":\"Zeeshan Ejaz\",\"age\":5147483645,\"address\":\"H # 531, S # 20\",\"uid\":\"123321\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\",\"salary\":20000,\"department\":\"Software Development\",\"joiningDay\":\"Saturday\",\"workingDays\":[\"Monday\",\"Tuesday\",\"Friday\"],\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\",\"promotedAt\":1484719381},\"dependents\":[{\"name\":\"Future Wife\",\"age\":5147483649,\"address\":\"H # 531, S # 20\",\"uid\":\"123412\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"},{\"name\":\"Future Kid\",\"age\":5147483648,\"address\":\"H # 531, S # 20\",\"uid\":\"312341\",\"birthday\":\"1994-02-13\",\"birthtime\":\"1994-02-13T14:01:54.9571247Z\"}],\"hiredAt\":\"Sun, 06 Nov 1994 08:49:37 GMT\"}]";
List<Employee> models = mapper.readValue(modelsValue,new TypeReference<List<Employee>> (){});
collect.setModels(models);

String stringsValue = "[\"abc\", \"def\"]";
List<String> strings = mapper.readValue(stringsValue,new TypeReference<List<String>> (){});
collect.setStrings(strings);

// Invoking the API call with sample inputs
formParams.sendMixedArrayAsync(collect, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
}
);

```


### <a name="send_integer_enum_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.FormParamsController.sendIntegerEnumArrayAsync") sendIntegerEnumArrayAsync

> TODO: Add a method description


```java
void sendIntegerEnumArrayAsync(
        final List<SuiteCode> suites,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| suites |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
String suitesValue = "[1, 3, 4, 2, 3]";
List<SuiteCode> suites = mapper.readValue(suitesValue,new TypeReference<List<SuiteCode>> (){});
// Invoking the API call with sample inputs
formParams.sendIntegerEnumArrayAsync(suites, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="send_string_enum_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.FormParamsController.sendStringEnumArrayAsync") sendStringEnumArrayAsync

> TODO: Add a method description


```java
void sendStringEnumArrayAsync(
        final List<Days> days,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| days |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
String daysValue = "[\"Tuesday\", \"Saturday\", \"Wednesday\", \"Monday\", \"Sunday\"]";
List<Days> days = mapper.readValue(daysValue,new TypeReference<List<Days>> (){});
// Invoking the API call with sample inputs
formParams.sendStringEnumArrayAsync(days, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="query_param_controller"></a>![Class: ](https://apidocs.io/img/class.png "org.hopto.apimatic.controllers.QueryParamController") QueryParamController

### Get singleton instance

The singleton instance of the ``` QueryParamController ``` class can be accessed from the API Client.

```java
QueryParamController queryParam = client.getQueryParam();
```

### <a name="date_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.QueryParamController.dateArrayAsync") dateArrayAsync

> TODO: Add a method description


```java
void dateArrayAsync(
        final List<Date> dates,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| dates |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
String datesValue = ["1994-02-13","1994-02-13"];
List<Date> dates = mapper.readValue(datesValue,new TypeReference<List<Date>> (){});
// Invoking the API call with sample inputs
queryParam.dateArrayAsync(dates, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="date_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.QueryParamController.dateAsync") dateAsync

> TODO: Add a method description


```java
void dateAsync(
        final Date date,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| date |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
Date date = 1994-02-13;
// Invoking the API call with sample inputs
queryParam.dateAsync(date, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="unix_date_time_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.QueryParamController.unixDateTimeArrayAsync") unixDateTimeArrayAsync

> TODO: Add a method description


```java
void unixDateTimeArrayAsync(
        final List<Date> datetimes,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
String datetimesValue = [1484719381,1484719381];
List<Date> datetimes = mapper.readValue(datetimesValue,new TypeReference<List<Date>> (){});
// Invoking the API call with sample inputs
queryParam.unixDateTimeArrayAsync(datetimes, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="unix_date_time_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.QueryParamController.unixDateTimeAsync") unixDateTimeAsync

> TODO: Add a method description


```java
void unixDateTimeAsync(
        final Date datetime,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
Date datetime = 1484719381;
// Invoking the API call with sample inputs
queryParam.unixDateTimeAsync(datetime, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="rfc1123_date_time_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.QueryParamController.rfc1123DateTimeAsync") rfc1123DateTimeAsync

> TODO: Add a method description


```java
void rfc1123DateTimeAsync(
        final Date datetime,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
Date datetime = Sun, 06 Nov 1994 08:49:37 GMT;
// Invoking the API call with sample inputs
queryParam.rfc1123DateTimeAsync(datetime, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="rfc1123_date_time_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.QueryParamController.rfc1123DateTimeArrayAsync") rfc1123DateTimeArrayAsync

> TODO: Add a method description


```java
void rfc1123DateTimeArrayAsync(
        final List<Date> datetimes,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
String datetimesValue = ["Sun, 06 Nov 1994 08:49:37 GMT","Sun, 06 Nov 1994 08:49:37 GMT"];
List<Date> datetimes = mapper.readValue(datetimesValue,new TypeReference<List<Date>> (){});
// Invoking the API call with sample inputs
queryParam.rfc1123DateTimeArrayAsync(datetimes, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="rfc3339_date_time_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.QueryParamController.rfc3339DateTimeArrayAsync") rfc3339DateTimeArrayAsync

> TODO: Add a method description


```java
void rfc3339DateTimeArrayAsync(
        final List<Date> datetimes,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetimes |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
String datetimesValue = ["1994-02-13T14:01:54.9571247Z","1994-02-13T14:01:54.9571247Z"];
List<Date> datetimes = mapper.readValue(datetimesValue,new TypeReference<List<Date>> (){});
// Invoking the API call with sample inputs
queryParam.rfc3339DateTimeArrayAsync(datetimes, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="rfc3339_date_time_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.QueryParamController.rfc3339DateTimeAsync") rfc3339DateTimeAsync

> TODO: Add a method description


```java
void rfc3339DateTimeAsync(
        final Date datetime,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| datetime |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
Date datetime = 1994-02-13T14:01:54.9571247Z;
// Invoking the API call with sample inputs
queryParam.rfc3339DateTimeAsync(datetime, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="no_params_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.QueryParamController.noParamsAsync") noParamsAsync

> TODO: Add a method description


```java
void noParamsAsync(final APICallBack<ServerResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
queryParam.noParamsAsync(new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="string_param_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.QueryParamController.stringParamAsync") stringParamAsync

> TODO: Add a method description


```java
void stringParamAsync(
        final String string,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| string |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
String string = "l;asd;asdwe[2304&&;'.d??\\a\\\\\\;sd//";
// Invoking the API call with sample inputs
queryParam.stringParamAsync(string, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="url_param_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.QueryParamController.urlParamAsync") urlParamAsync

> TODO: Add a method description


```java
void urlParamAsync(
        final String url,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| url |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
String url = "https://www.shahidisawesome.com/and/also/a/narcissist?thisis=aparameter&another=one";
// Invoking the API call with sample inputs
queryParam.urlParamAsync(url, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="number_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.QueryParamController.numberArrayAsync") numberArrayAsync

> TODO: Add a method description


```java
void numberArrayAsync(
        final List<Integer> integers,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
String integersValue = "[1,2,3,4,5]";
List<Integer> integers = mapper.readValue(integersValue,new TypeReference<List<Integer>> (){});
// Invoking the API call with sample inputs
queryParam.numberArrayAsync(integers, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="string_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.QueryParamController.stringArrayAsync") stringArrayAsync

> TODO: Add a method description


```java
void stringArrayAsync(
        final List<String> strings,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
String stringsValue = "[\"abc\", \"def\"]";
List<String> strings = mapper.readValue(stringsValue,new TypeReference<List<String>> (){});
// Invoking the API call with sample inputs
queryParam.stringArrayAsync(strings, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="simple_query_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.QueryParamController.simpleQueryAsync") simpleQueryAsync

> TODO: Add a method description


```java
void simpleQueryAsync(
        final boolean mboolean,
        final int number,
        final String string,
        Map<String, Object> queryParameters,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| mboolean |  ``` Required ```  | TODO: Add a parameter description |
| number |  ``` Required ```  | TODO: Add a parameter description |
| string |  ``` Required ```  | TODO: Add a parameter description |
| queryParameters | ``` Optional ``` | Additional optional query parameters are supported by this method |


#### Example Usage

```java
boolean mboolean = true;
int number = 4;
String string = "TestString";
// key-value map for optional query parameters
Map<String, Object> queryParams = new LinkedHashMap<String, Object>();
// Invoking the API call with sample inputs
queryParam.simpleQueryAsync(mboolean, number, string, queryParams, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="string_enum_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.QueryParamController.stringEnumArrayAsync") stringEnumArrayAsync

> TODO: Add a method description


```java
void stringEnumArrayAsync(
        final List<Days> days,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| days |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
String daysValue = "[\"Tuesday\", \"Saturday\", \"Wednesday\", \"Monday\", \"Sunday\"]";
List<Days> days = mapper.readValue(daysValue,new TypeReference<List<Days>> (){});
// Invoking the API call with sample inputs
queryParam.stringEnumArrayAsync(days, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="multiple_params_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.QueryParamController.multipleParamsAsync") multipleParamsAsync

> TODO: Add a method description


```java
void multipleParamsAsync(
        final int number,
        final double precision,
        final String string,
        final String url,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| number |  ``` Required ```  | TODO: Add a parameter description |
| precision |  ``` Required ```  | TODO: Add a parameter description |
| string |  ``` Required ```  | TODO: Add a parameter description |
| url |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
int number = 123412312;
double precision = 1112.34;
String string = "\"\"test./;\";12&&3asl\"\";\"qw1&34\"///..//.";
String url = "http://www.abc.com/test?a=b&c=\"http://lolol.com?param=no&another=lol\"";
// Invoking the API call with sample inputs
queryParam.multipleParamsAsync(number, precision, string, url, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="integer_enum_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.QueryParamController.integerEnumArrayAsync") integerEnumArrayAsync

> TODO: Add a method description


```java
void integerEnumArrayAsync(
        final List<SuiteCode> suites,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| suites |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
String suitesValue = "[1, 3, 4, 2, 3]";
List<SuiteCode> suites = mapper.readValue(suitesValue,new TypeReference<List<SuiteCode>> (){});
// Invoking the API call with sample inputs
queryParam.integerEnumArrayAsync(suites, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="error_codes_controller"></a>![Class: ](https://apidocs.io/img/class.png "org.hopto.apimatic.controllers.ErrorCodesController") ErrorCodesController

### Get singleton instance

The singleton instance of the ``` ErrorCodesController ``` class can be accessed from the API Client.

```java
ErrorCodesController errorCodes = client.getErrorCodes();
```

### <a name="get400_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ErrorCodesController.get400Async") get400Async

> TODO: Add a method description


```java
void get400Async(final APICallBack<DynamicResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
errorCodes.get400Async(new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get500_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ErrorCodesController.get500Async") get500Async

> TODO: Add a method description


```java
void get500Async(final APICallBack<DynamicResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
errorCodes.get500Async(new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="get401_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.ErrorCodesController.get401Async") get401Async

> TODO: Add a method description


```java
void get401Async(final APICallBack<DynamicResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
errorCodes.get401Async(new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

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

## <a name="echo_controller"></a>![Class: ](https://apidocs.io/img/class.png "org.hopto.apimatic.controllers.EchoController") EchoController

### Get singleton instance

The singleton instance of the ``` EchoController ``` class can be accessed from the API Client.

```java
EchoController echo = client.getEcho();
```

### <a name="json_echo_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.EchoController.jsonEchoAsync") jsonEchoAsync

> Echo's back the request


```java
void jsonEchoAsync(
        final Object input,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| input |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
try {
    String inputValue = "{\"uid\": \"1123213\", \"name\": \"Shahid\"}";
    Object input = mapper.readValue(inputValue,new TypeReference<Object> (){});
    // Invoking the API call with sample inputs
    echo.jsonEchoAsync(input, new APICallBack<DynamicResponse>() {
        public void onSuccess(HttpContext context, DynamicResponse response) {
            // TODO success callback handler
        }
        public void onFailure(HttpContext context, Throwable error) {
            // TODO failure callback handler
        }
    });
} catch(JsonProcessingException e) {
    // TODO Auto-generated catch block
    e.printStackTrace();
}
```


### <a name="form_echo_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.EchoController.formEchoAsync") formEchoAsync

> Sends the request including any form params as JSON


```java
void formEchoAsync(
        final Object input,
        final APICallBack<DynamicResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| input |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
String inputValue = "{\"uid\": \"1123213\", \"name\": \"Shahid\"}";
Object input = mapper.readValue(inputValue,new TypeReference<Object> (){});
// Invoking the API call with sample inputs
echo.formEchoAsync(input, new APICallBack<DynamicResponse>() {
    public void onSuccess(HttpContext context, DynamicResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="query_echo_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.EchoController.queryEchoAsync") queryEchoAsync

> TODO: Add a method description


```java
void queryEchoAsync(
        Map<String, Object> queryParameters,
        final APICallBack<EchoResponse> callBack)
```

#### Example Usage

```java
// key-value map for optional query parameters
Map<String, Object> queryParams = new LinkedHashMap<String, Object>();
// Invoking the API call with sample inputs
echo.queryEchoAsync(queryParams, new APICallBack<EchoResponse>() {
    public void onSuccess(HttpContext context, EchoResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="header_controller"></a>![Class: ](https://apidocs.io/img/class.png "org.hopto.apimatic.controllers.HeaderController") HeaderController

### Get singleton instance

The singleton instance of the ``` HeaderController ``` class can be accessed from the API Client.

```java
HeaderController header = client.getHeader();
```

### <a name="send_headers_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.HeaderController.sendHeadersAsync") sendHeadersAsync

> Sends a single header params


```java
void sendHeadersAsync(
        final String customHeader,
        final String value,
        final APICallBack<ServerResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| customHeader |  ``` Required ```  | TODO: Add a parameter description |
| value |  ``` Required ```  | Represents the value of the custom header |


#### Example Usage

```java
String customHeader = "TestString";
String value = "TestString";
// Invoking the API call with sample inputs
header.sendHeadersAsync(customHeader, value, new APICallBack<ServerResponse>() {
    public void onSuccess(HttpContext context, ServerResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="template_params_controller"></a>![Class: ](https://apidocs.io/img/class.png "org.hopto.apimatic.controllers.TemplateParamsController") TemplateParamsController

### Get singleton instance

The singleton instance of the ``` TemplateParamsController ``` class can be accessed from the API Client.

```java
TemplateParamsController templateParams = client.getTemplateParams();
```

### <a name="send_string_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.TemplateParamsController.sendStringArrayAsync") sendStringArrayAsync

> TODO: Add a method description


```java
void sendStringArrayAsync(
        final List<String> strings,
        final APICallBack<EchoResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| strings |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
String stringsValue = "[\"abc\", \"def\"]";
List<String> strings = mapper.readValue(stringsValue,new TypeReference<List<String>> (){});
// Invoking the API call with sample inputs
templateParams.sendStringArrayAsync(strings, new APICallBack<EchoResponse>() {
    public void onSuccess(HttpContext context, EchoResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


### <a name="send_integer_array_async"></a>![Method: ](https://apidocs.io/img/method.png "org.hopto.apimatic.controllers.TemplateParamsController.sendIntegerArrayAsync") sendIntegerArrayAsync

> TODO: Add a method description


```java
void sendIntegerArrayAsync(
        final List<Integer> integers,
        final APICallBack<EchoResponse> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| integers |  ``` Required ```  ``` Collection ```  | TODO: Add a parameter description |


#### Example Usage

```java
String integersValue = "[1,2,3,4,5]";
List<Integer> integers = mapper.readValue(integersValue,new TypeReference<List<Integer>> (){});
// Invoking the API call with sample inputs
templateParams.sendIntegerArrayAsync(integers, new APICallBack<EchoResponse>() {
    public void onSuccess(HttpContext context, EchoResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)



