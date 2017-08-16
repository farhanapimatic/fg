# Getting started

## How to Build

The generated code uses the Newtonsoft Json.NET NuGet Package. If the automatic NuGet package restore
is enabled, these dependencies will be installed automatically. Therefore,
you will need internet access for build.

1. Open the solution (AWSECommerceService.sln) file.
2. Invoke the build process using `Ctrl+Shift+B` shortcut key or using the `Build` menu as shown below.

![Building SDK using Visual Studio](https://apidocs.io/illustration/cs?step=buildSDK&workspaceFolder=AWSECommerceService-CSharp&workspaceName=AWSECommerceService&projectName=AWSECommerceService.PCL)

## How to Use

The build process generates a portable class library, which can be used like a normal class library. The generated library is compatible with Windows Forms, Windows RT, Windows Phone 8,
Silverlight 5, Xamarin iOS, Xamarin Android and Mono. More information on how to use can be found at the [MSDN Portable Class Libraries documentation](http://msdn.microsoft.com/en-us/library/vstudio/gg597391%28v=vs.100%29.aspx).

The following section explains how to use the AWSECommerceService library in a new console project.

### 1. Starting a new project

For starting a new project, right click on the current solution from the *solution explorer* and choose  ``` Add -> New Project ```.

![Add a new project in the existing solution using Visual Studio](https://apidocs.io/illustration/cs?step=addProject&workspaceFolder=AWSECommerceService-CSharp&workspaceName=AWSECommerceService&projectName=AWSECommerceService.PCL)

Next, choose "Console Application", provide a ``` TestConsoleProject ``` as the project name and click ``` OK ```.

![Create a new console project using Visual Studio](https://apidocs.io/illustration/cs?step=createProject&workspaceFolder=AWSECommerceService-CSharp&workspaceName=AWSECommerceService&projectName=AWSECommerceService.PCL)

### 2. Set as startup project

The new console project is the entry point for the eventual execution. This requires us to set the ``` TestConsoleProject ``` as the start-up project. To do this, right-click on the  ``` TestConsoleProject ``` and choose  ``` Set as StartUp Project ``` form the context menu.

![Set the new cosole project as the start up project](https://apidocs.io/illustration/cs?step=setStartup&workspaceFolder=AWSECommerceService-CSharp&workspaceName=AWSECommerceService&projectName=AWSECommerceService.PCL)

### 3. Add reference of the library project

In order to use the AWSECommerceService library in the new project, first we must add a projet reference to the ``` TestConsoleProject ```. First, right click on the ``` References ``` node in the *solution explorer* and click ``` Add Reference... ```.

![Open references of the TestConsoleProject](https://apidocs.io/illustration/cs?step=addReference&workspaceFolder=AWSECommerceService-CSharp&workspaceName=AWSECommerceService&projectName=AWSECommerceService.PCL)

Next, a window will be displayed where we must set the ``` checkbox ``` on ``` AWSECommerceService.PCL ``` and click ``` OK ```. By doing this, we have added a reference of the ```AWSECommerceService.PCL``` project into the new ``` TestConsoleProject ```.

![Add a reference to the TestConsoleProject](https://apidocs.io/illustration/cs?step=createReference&workspaceFolder=AWSECommerceService-CSharp&workspaceName=AWSECommerceService&projectName=AWSECommerceService.PCL)

### 4. Write sample code

Once the ``` TestConsoleProject ``` is created, a file named ``` Program.cs ``` will be visible in the *solution explorer* with an empty ``` Main ``` method. This is the entry point for the execution of the entire solution.
Here, you can add code to initialize the client library and acquire the instance of a *Controller* class. Sample code to initialize the client library and using controller methods is given in the subsequent sections.

![Add a reference to the TestConsoleProject](https://apidocs.io/illustration/cs?step=addCode&workspaceFolder=AWSECommerceService-CSharp&workspaceName=AWSECommerceService&projectName=AWSECommerceService.PCL)

## How to Test

The generated SDK also contain one or more Tests, which are contained in the Tests project.
In order to invoke these test cases, you will need *NUnit 3.0 Test Adapter Extension for Visual Studio*.
Once the SDK is complied, the test cases should appear in the Test Explorer window.
Here, you can click *Run All* to execute these test cases.

## Initialization

### 

API client can be initialized as following.

```csharp

AWSECommerceServiceClient client = new AWSECommerceServiceClient();
```



# Class Reference

## <a name="list_of_controllers"></a>List of Controllers

* [AWSECommerceServiceBindingController](#awse_commerce_service_binding_controller)

## <a name="awse_commerce_service_binding_controller"></a>![Class: ](https://apidocs.io/img/class.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController") AWSECommerceServiceBindingController

### Get singleton instance

The singleton instance of the ``` AWSECommerceServiceBindingController ``` class can be accessed from the API Client.

```csharp
AWSECommerceServiceBindingController aWSECommerceServiceBinding = client.AWSECommerceServiceBinding;
```

### <a name="create_cart_modify97"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartModify97") CreateCartModify97

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartModifyResponseMsg> CreateCartModify97(Models.CartModifyRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartModifyRequestMsg();

Models.CartModifyResponseMsg result = await aWSECommerceServiceBinding.CreateCartModify97(body);

```


### <a name="create_cart_clear98"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartClear98") CreateCartClear98

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartClearResponseMsg> CreateCartClear98(Models.CartClearRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartClearRequestMsg();

Models.CartClearResponseMsg result = await aWSECommerceServiceBinding.CreateCartClear98(body);

```


### <a name="create_cart_create96"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartCreate96") CreateCartCreate96

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartCreateResponseMsg> CreateCartCreate96(Models.CartCreateRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartCreateRequestMsg();

Models.CartCreateResponseMsg result = await aWSECommerceServiceBinding.CreateCartCreate96(body);

```


### <a name="create_cart_add95"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartAdd95") CreateCartAdd95

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartAddResponseMsg> CreateCartAdd95(Models.CartAddRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartAddRequestMsg();

Models.CartAddResponseMsg result = await aWSECommerceServiceBinding.CreateCartAdd95(body);

```


### <a name="create_cart_get94"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartGet94") CreateCartGet94

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartGetResponseMsg> CreateCartGet94(Models.CartGetRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartGetRequestMsg();

Models.CartGetResponseMsg result = await aWSECommerceServiceBinding.CreateCartGet94(body);

```


### <a name="create_similarity_lookup93"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateSimilarityLookup93") CreateSimilarityLookup93

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.SimilarityLookupResponseMsg> CreateSimilarityLookup93(Models.SimilarityLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.SimilarityLookupRequestMsg();

Models.SimilarityLookupResponseMsg result = await aWSECommerceServiceBinding.CreateSimilarityLookup93(body);

```


### <a name="create_browse_node_lookup92"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateBrowseNodeLookup92") CreateBrowseNodeLookup92

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.BrowseNodeLookupResponseMsg> CreateBrowseNodeLookup92(Models.BrowseNodeLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.BrowseNodeLookupRequestMsg();

Models.BrowseNodeLookupResponseMsg result = await aWSECommerceServiceBinding.CreateBrowseNodeLookup92(body);

```


### <a name="create_item_lookup91"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateItemLookup91") CreateItemLookup91

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.ItemLookupResponseMsg> CreateItemLookup91(Models.ItemLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.ItemLookupRequestMsg();

Models.ItemLookupResponseMsg result = await aWSECommerceServiceBinding.CreateItemLookup91(body);

```


### <a name="create_item_search90"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateItemSearch90") CreateItemSearch90

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.ItemSearchResponseMsg> CreateItemSearch90(Models.ItemSearchRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.ItemSearchRequestMsg();

Models.ItemSearchResponseMsg result = await aWSECommerceServiceBinding.CreateItemSearch90(body);

```


### <a name="create_cart_clear89"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartClear89") CreateCartClear89

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartClearResponseMsg> CreateCartClear89(Models.CartClearRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartClearRequestMsg();

Models.CartClearResponseMsg result = await aWSECommerceServiceBinding.CreateCartClear89(body);

```


### <a name="create_cart_modify88"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartModify88") CreateCartModify88

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartModifyResponseMsg> CreateCartModify88(Models.CartModifyRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartModifyRequestMsg();

Models.CartModifyResponseMsg result = await aWSECommerceServiceBinding.CreateCartModify88(body);

```


### <a name="create_cart_create87"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartCreate87") CreateCartCreate87

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartCreateResponseMsg> CreateCartCreate87(Models.CartCreateRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartCreateRequestMsg();

Models.CartCreateResponseMsg result = await aWSECommerceServiceBinding.CreateCartCreate87(body);

```


### <a name="create_cart_add86"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartAdd86") CreateCartAdd86

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartAddResponseMsg> CreateCartAdd86(Models.CartAddRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartAddRequestMsg();

Models.CartAddResponseMsg result = await aWSECommerceServiceBinding.CreateCartAdd86(body);

```


### <a name="create_cart_get85"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartGet85") CreateCartGet85

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartGetResponseMsg> CreateCartGet85(Models.CartGetRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartGetRequestMsg();

Models.CartGetResponseMsg result = await aWSECommerceServiceBinding.CreateCartGet85(body);

```


### <a name="create_similarity_lookup84"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateSimilarityLookup84") CreateSimilarityLookup84

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.SimilarityLookupResponseMsg> CreateSimilarityLookup84(Models.SimilarityLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.SimilarityLookupRequestMsg();

Models.SimilarityLookupResponseMsg result = await aWSECommerceServiceBinding.CreateSimilarityLookup84(body);

```


### <a name="create_browse_node_lookup83"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateBrowseNodeLookup83") CreateBrowseNodeLookup83

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.BrowseNodeLookupResponseMsg> CreateBrowseNodeLookup83(Models.BrowseNodeLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.BrowseNodeLookupRequestMsg();

Models.BrowseNodeLookupResponseMsg result = await aWSECommerceServiceBinding.CreateBrowseNodeLookup83(body);

```


### <a name="create_item_lookup82"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateItemLookup82") CreateItemLookup82

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.ItemLookupResponseMsg> CreateItemLookup82(Models.ItemLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.ItemLookupRequestMsg();

Models.ItemLookupResponseMsg result = await aWSECommerceServiceBinding.CreateItemLookup82(body);

```


### <a name="create_item_search81"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateItemSearch81") CreateItemSearch81

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.ItemSearchResponseMsg> CreateItemSearch81(Models.ItemSearchRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.ItemSearchRequestMsg();

Models.ItemSearchResponseMsg result = await aWSECommerceServiceBinding.CreateItemSearch81(body);

```


### <a name="create_cart_clear80"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartClear80") CreateCartClear80

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartClearResponseMsg> CreateCartClear80(Models.CartClearRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartClearRequestMsg();

Models.CartClearResponseMsg result = await aWSECommerceServiceBinding.CreateCartClear80(body);

```


### <a name="create_cart_modify79"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartModify79") CreateCartModify79

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartModifyResponseMsg> CreateCartModify79(Models.CartModifyRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartModifyRequestMsg();

Models.CartModifyResponseMsg result = await aWSECommerceServiceBinding.CreateCartModify79(body);

```


### <a name="create_cart_create78"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartCreate78") CreateCartCreate78

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartCreateResponseMsg> CreateCartCreate78(Models.CartCreateRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartCreateRequestMsg();

Models.CartCreateResponseMsg result = await aWSECommerceServiceBinding.CreateCartCreate78(body);

```


### <a name="create_cart_add77"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartAdd77") CreateCartAdd77

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartAddResponseMsg> CreateCartAdd77(Models.CartAddRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartAddRequestMsg();

Models.CartAddResponseMsg result = await aWSECommerceServiceBinding.CreateCartAdd77(body);

```


### <a name="create_cart_get76"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartGet76") CreateCartGet76

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartGetResponseMsg> CreateCartGet76(Models.CartGetRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartGetRequestMsg();

Models.CartGetResponseMsg result = await aWSECommerceServiceBinding.CreateCartGet76(body);

```


### <a name="create_similarity_lookup75"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateSimilarityLookup75") CreateSimilarityLookup75

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.SimilarityLookupResponseMsg> CreateSimilarityLookup75(Models.SimilarityLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.SimilarityLookupRequestMsg();

Models.SimilarityLookupResponseMsg result = await aWSECommerceServiceBinding.CreateSimilarityLookup75(body);

```


### <a name="create_browse_node_lookup74"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateBrowseNodeLookup74") CreateBrowseNodeLookup74

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.BrowseNodeLookupResponseMsg> CreateBrowseNodeLookup74(Models.BrowseNodeLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.BrowseNodeLookupRequestMsg();

Models.BrowseNodeLookupResponseMsg result = await aWSECommerceServiceBinding.CreateBrowseNodeLookup74(body);

```


### <a name="create_item_lookup73"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateItemLookup73") CreateItemLookup73

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.ItemLookupResponseMsg> CreateItemLookup73(Models.ItemLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.ItemLookupRequestMsg();

Models.ItemLookupResponseMsg result = await aWSECommerceServiceBinding.CreateItemLookup73(body);

```


### <a name="create_item_search72"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateItemSearch72") CreateItemSearch72

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.ItemSearchResponseMsg> CreateItemSearch72(Models.ItemSearchRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.ItemSearchRequestMsg();

Models.ItemSearchResponseMsg result = await aWSECommerceServiceBinding.CreateItemSearch72(body);

```


### <a name="create_cart_clear71"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartClear71") CreateCartClear71

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartClearResponseMsg> CreateCartClear71(Models.CartClearRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartClearRequestMsg();

Models.CartClearResponseMsg result = await aWSECommerceServiceBinding.CreateCartClear71(body);

```


### <a name="create_cart_modify70"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartModify70") CreateCartModify70

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartModifyResponseMsg> CreateCartModify70(Models.CartModifyRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartModifyRequestMsg();

Models.CartModifyResponseMsg result = await aWSECommerceServiceBinding.CreateCartModify70(body);

```


### <a name="create_cart_create69"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartCreate69") CreateCartCreate69

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartCreateResponseMsg> CreateCartCreate69(Models.CartCreateRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartCreateRequestMsg();

Models.CartCreateResponseMsg result = await aWSECommerceServiceBinding.CreateCartCreate69(body);

```


### <a name="create_cart_add68"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartAdd68") CreateCartAdd68

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartAddResponseMsg> CreateCartAdd68(Models.CartAddRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartAddRequestMsg();

Models.CartAddResponseMsg result = await aWSECommerceServiceBinding.CreateCartAdd68(body);

```


### <a name="create_cart_get67"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartGet67") CreateCartGet67

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartGetResponseMsg> CreateCartGet67(Models.CartGetRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartGetRequestMsg();

Models.CartGetResponseMsg result = await aWSECommerceServiceBinding.CreateCartGet67(body);

```


### <a name="create_similarity_lookup66"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateSimilarityLookup66") CreateSimilarityLookup66

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.SimilarityLookupResponseMsg> CreateSimilarityLookup66(Models.SimilarityLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.SimilarityLookupRequestMsg();

Models.SimilarityLookupResponseMsg result = await aWSECommerceServiceBinding.CreateSimilarityLookup66(body);

```


### <a name="create_browse_node_lookup65"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateBrowseNodeLookup65") CreateBrowseNodeLookup65

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.BrowseNodeLookupResponseMsg> CreateBrowseNodeLookup65(Models.BrowseNodeLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.BrowseNodeLookupRequestMsg();

Models.BrowseNodeLookupResponseMsg result = await aWSECommerceServiceBinding.CreateBrowseNodeLookup65(body);

```


### <a name="create_item_lookup64"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateItemLookup64") CreateItemLookup64

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.ItemLookupResponseMsg> CreateItemLookup64(Models.ItemLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.ItemLookupRequestMsg();

Models.ItemLookupResponseMsg result = await aWSECommerceServiceBinding.CreateItemLookup64(body);

```


### <a name="create_item_search63"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateItemSearch63") CreateItemSearch63

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.ItemSearchResponseMsg> CreateItemSearch63(Models.ItemSearchRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.ItemSearchRequestMsg();

Models.ItemSearchResponseMsg result = await aWSECommerceServiceBinding.CreateItemSearch63(body);

```


### <a name="create_cart_clear62"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartClear62") CreateCartClear62

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartClearResponseMsg> CreateCartClear62(Models.CartClearRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartClearRequestMsg();

Models.CartClearResponseMsg result = await aWSECommerceServiceBinding.CreateCartClear62(body);

```


### <a name="create_cart_modify61"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartModify61") CreateCartModify61

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartModifyResponseMsg> CreateCartModify61(Models.CartModifyRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartModifyRequestMsg();

Models.CartModifyResponseMsg result = await aWSECommerceServiceBinding.CreateCartModify61(body);

```


### <a name="create_cart_create60"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartCreate60") CreateCartCreate60

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartCreateResponseMsg> CreateCartCreate60(Models.CartCreateRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartCreateRequestMsg();

Models.CartCreateResponseMsg result = await aWSECommerceServiceBinding.CreateCartCreate60(body);

```


### <a name="create_cart_add59"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartAdd59") CreateCartAdd59

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartAddResponseMsg> CreateCartAdd59(Models.CartAddRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartAddRequestMsg();

Models.CartAddResponseMsg result = await aWSECommerceServiceBinding.CreateCartAdd59(body);

```


### <a name="create_cart_get58"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartGet58") CreateCartGet58

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartGetResponseMsg> CreateCartGet58(Models.CartGetRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartGetRequestMsg();

Models.CartGetResponseMsg result = await aWSECommerceServiceBinding.CreateCartGet58(body);

```


### <a name="create_similarity_lookup57"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateSimilarityLookup57") CreateSimilarityLookup57

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.SimilarityLookupResponseMsg> CreateSimilarityLookup57(Models.SimilarityLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.SimilarityLookupRequestMsg();

Models.SimilarityLookupResponseMsg result = await aWSECommerceServiceBinding.CreateSimilarityLookup57(body);

```


### <a name="create_browse_node_lookup56"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateBrowseNodeLookup56") CreateBrowseNodeLookup56

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.BrowseNodeLookupResponseMsg> CreateBrowseNodeLookup56(Models.BrowseNodeLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.BrowseNodeLookupRequestMsg();

Models.BrowseNodeLookupResponseMsg result = await aWSECommerceServiceBinding.CreateBrowseNodeLookup56(body);

```


### <a name="create_item_lookup55"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateItemLookup55") CreateItemLookup55

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.ItemLookupResponseMsg> CreateItemLookup55(Models.ItemLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.ItemLookupRequestMsg();

Models.ItemLookupResponseMsg result = await aWSECommerceServiceBinding.CreateItemLookup55(body);

```


### <a name="create_item_search54"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateItemSearch54") CreateItemSearch54

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.ItemSearchResponseMsg> CreateItemSearch54(Models.ItemSearchRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.ItemSearchRequestMsg();

Models.ItemSearchResponseMsg result = await aWSECommerceServiceBinding.CreateItemSearch54(body);

```


### <a name="create_cart_clear53"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartClear53") CreateCartClear53

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartClearResponseMsg> CreateCartClear53(Models.CartClearRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartClearRequestMsg();

Models.CartClearResponseMsg result = await aWSECommerceServiceBinding.CreateCartClear53(body);

```


### <a name="create_cart_modify52"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartModify52") CreateCartModify52

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartModifyResponseMsg> CreateCartModify52(Models.CartModifyRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartModifyRequestMsg();

Models.CartModifyResponseMsg result = await aWSECommerceServiceBinding.CreateCartModify52(body);

```


### <a name="create_cart_create51"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartCreate51") CreateCartCreate51

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartCreateResponseMsg> CreateCartCreate51(Models.CartCreateRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartCreateRequestMsg();

Models.CartCreateResponseMsg result = await aWSECommerceServiceBinding.CreateCartCreate51(body);

```


### <a name="create_cart_add50"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartAdd50") CreateCartAdd50

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartAddResponseMsg> CreateCartAdd50(Models.CartAddRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartAddRequestMsg();

Models.CartAddResponseMsg result = await aWSECommerceServiceBinding.CreateCartAdd50(body);

```


### <a name="create_cart_get49"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartGet49") CreateCartGet49

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartGetResponseMsg> CreateCartGet49(Models.CartGetRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartGetRequestMsg();

Models.CartGetResponseMsg result = await aWSECommerceServiceBinding.CreateCartGet49(body);

```


### <a name="create_similarity_lookup48"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateSimilarityLookup48") CreateSimilarityLookup48

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.SimilarityLookupResponseMsg> CreateSimilarityLookup48(Models.SimilarityLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.SimilarityLookupRequestMsg();

Models.SimilarityLookupResponseMsg result = await aWSECommerceServiceBinding.CreateSimilarityLookup48(body);

```


### <a name="create_browse_node_lookup47"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateBrowseNodeLookup47") CreateBrowseNodeLookup47

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.BrowseNodeLookupResponseMsg> CreateBrowseNodeLookup47(Models.BrowseNodeLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.BrowseNodeLookupRequestMsg();

Models.BrowseNodeLookupResponseMsg result = await aWSECommerceServiceBinding.CreateBrowseNodeLookup47(body);

```


### <a name="create_item_lookup46"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateItemLookup46") CreateItemLookup46

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.ItemLookupResponseMsg> CreateItemLookup46(Models.ItemLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.ItemLookupRequestMsg();

Models.ItemLookupResponseMsg result = await aWSECommerceServiceBinding.CreateItemLookup46(body);

```


### <a name="create_item_search45"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateItemSearch45") CreateItemSearch45

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.ItemSearchResponseMsg> CreateItemSearch45(Models.ItemSearchRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.ItemSearchRequestMsg();

Models.ItemSearchResponseMsg result = await aWSECommerceServiceBinding.CreateItemSearch45(body);

```


### <a name="create_cart_clear44"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartClear44") CreateCartClear44

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartClearResponseMsg> CreateCartClear44(Models.CartClearRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartClearRequestMsg();

Models.CartClearResponseMsg result = await aWSECommerceServiceBinding.CreateCartClear44(body);

```


### <a name="create_cart_modify43"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartModify43") CreateCartModify43

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartModifyResponseMsg> CreateCartModify43(Models.CartModifyRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartModifyRequestMsg();

Models.CartModifyResponseMsg result = await aWSECommerceServiceBinding.CreateCartModify43(body);

```


### <a name="create_cart_create42"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartCreate42") CreateCartCreate42

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartCreateResponseMsg> CreateCartCreate42(Models.CartCreateRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartCreateRequestMsg();

Models.CartCreateResponseMsg result = await aWSECommerceServiceBinding.CreateCartCreate42(body);

```


### <a name="create_cart_add41"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartAdd41") CreateCartAdd41

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartAddResponseMsg> CreateCartAdd41(Models.CartAddRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartAddRequestMsg();

Models.CartAddResponseMsg result = await aWSECommerceServiceBinding.CreateCartAdd41(body);

```


### <a name="create_cart_get40"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartGet40") CreateCartGet40

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartGetResponseMsg> CreateCartGet40(Models.CartGetRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartGetRequestMsg();

Models.CartGetResponseMsg result = await aWSECommerceServiceBinding.CreateCartGet40(body);

```


### <a name="create_similarity_lookup39"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateSimilarityLookup39") CreateSimilarityLookup39

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.SimilarityLookupResponseMsg> CreateSimilarityLookup39(Models.SimilarityLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.SimilarityLookupRequestMsg();

Models.SimilarityLookupResponseMsg result = await aWSECommerceServiceBinding.CreateSimilarityLookup39(body);

```


### <a name="create_browse_node_lookup38"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateBrowseNodeLookup38") CreateBrowseNodeLookup38

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.BrowseNodeLookupResponseMsg> CreateBrowseNodeLookup38(Models.BrowseNodeLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.BrowseNodeLookupRequestMsg();

Models.BrowseNodeLookupResponseMsg result = await aWSECommerceServiceBinding.CreateBrowseNodeLookup38(body);

```


### <a name="create_item_lookup37"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateItemLookup37") CreateItemLookup37

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.ItemLookupResponseMsg> CreateItemLookup37(Models.ItemLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.ItemLookupRequestMsg();

Models.ItemLookupResponseMsg result = await aWSECommerceServiceBinding.CreateItemLookup37(body);

```


### <a name="create_item_search36"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateItemSearch36") CreateItemSearch36

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.ItemSearchResponseMsg> CreateItemSearch36(Models.ItemSearchRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.ItemSearchRequestMsg();

Models.ItemSearchResponseMsg result = await aWSECommerceServiceBinding.CreateItemSearch36(body);

```


### <a name="create_cart_clear35"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartClear35") CreateCartClear35

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartClearResponseMsg> CreateCartClear35(Models.CartClearRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartClearRequestMsg();

Models.CartClearResponseMsg result = await aWSECommerceServiceBinding.CreateCartClear35(body);

```


### <a name="create_cart_modify34"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartModify34") CreateCartModify34

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartModifyResponseMsg> CreateCartModify34(Models.CartModifyRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartModifyRequestMsg();

Models.CartModifyResponseMsg result = await aWSECommerceServiceBinding.CreateCartModify34(body);

```


### <a name="create_cart_create33"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartCreate33") CreateCartCreate33

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartCreateResponseMsg> CreateCartCreate33(Models.CartCreateRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartCreateRequestMsg();

Models.CartCreateResponseMsg result = await aWSECommerceServiceBinding.CreateCartCreate33(body);

```


### <a name="create_cart_add32"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartAdd32") CreateCartAdd32

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartAddResponseMsg> CreateCartAdd32(Models.CartAddRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartAddRequestMsg();

Models.CartAddResponseMsg result = await aWSECommerceServiceBinding.CreateCartAdd32(body);

```


### <a name="create_cart_get31"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartGet31") CreateCartGet31

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartGetResponseMsg> CreateCartGet31(Models.CartGetRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartGetRequestMsg();

Models.CartGetResponseMsg result = await aWSECommerceServiceBinding.CreateCartGet31(body);

```


### <a name="create_similarity_lookup30"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateSimilarityLookup30") CreateSimilarityLookup30

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.SimilarityLookupResponseMsg> CreateSimilarityLookup30(Models.SimilarityLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.SimilarityLookupRequestMsg();

Models.SimilarityLookupResponseMsg result = await aWSECommerceServiceBinding.CreateSimilarityLookup30(body);

```


### <a name="create_browse_node_lookup29"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateBrowseNodeLookup29") CreateBrowseNodeLookup29

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.BrowseNodeLookupResponseMsg> CreateBrowseNodeLookup29(Models.BrowseNodeLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.BrowseNodeLookupRequestMsg();

Models.BrowseNodeLookupResponseMsg result = await aWSECommerceServiceBinding.CreateBrowseNodeLookup29(body);

```


### <a name="create_item_lookup28"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateItemLookup28") CreateItemLookup28

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.ItemLookupResponseMsg> CreateItemLookup28(Models.ItemLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.ItemLookupRequestMsg();

Models.ItemLookupResponseMsg result = await aWSECommerceServiceBinding.CreateItemLookup28(body);

```


### <a name="create_item_search27"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateItemSearch27") CreateItemSearch27

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.ItemSearchResponseMsg> CreateItemSearch27(Models.ItemSearchRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.ItemSearchRequestMsg();

Models.ItemSearchResponseMsg result = await aWSECommerceServiceBinding.CreateItemSearch27(body);

```


### <a name="create_cart_clear26"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartClear26") CreateCartClear26

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartClearResponseMsg> CreateCartClear26(Models.CartClearRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartClearRequestMsg();

Models.CartClearResponseMsg result = await aWSECommerceServiceBinding.CreateCartClear26(body);

```


### <a name="create_cart_modify25"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartModify25") CreateCartModify25

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartModifyResponseMsg> CreateCartModify25(Models.CartModifyRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartModifyRequestMsg();

Models.CartModifyResponseMsg result = await aWSECommerceServiceBinding.CreateCartModify25(body);

```


### <a name="create_cart_create24"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartCreate24") CreateCartCreate24

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartCreateResponseMsg> CreateCartCreate24(Models.CartCreateRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartCreateRequestMsg();

Models.CartCreateResponseMsg result = await aWSECommerceServiceBinding.CreateCartCreate24(body);

```


### <a name="create_cart_add23"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartAdd23") CreateCartAdd23

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartAddResponseMsg> CreateCartAdd23(Models.CartAddRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartAddRequestMsg();

Models.CartAddResponseMsg result = await aWSECommerceServiceBinding.CreateCartAdd23(body);

```


### <a name="create_cart_get22"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartGet22") CreateCartGet22

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartGetResponseMsg> CreateCartGet22(Models.CartGetRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartGetRequestMsg();

Models.CartGetResponseMsg result = await aWSECommerceServiceBinding.CreateCartGet22(body);

```


### <a name="create_similarity_lookup21"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateSimilarityLookup21") CreateSimilarityLookup21

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.SimilarityLookupResponseMsg> CreateSimilarityLookup21(Models.SimilarityLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.SimilarityLookupRequestMsg();

Models.SimilarityLookupResponseMsg result = await aWSECommerceServiceBinding.CreateSimilarityLookup21(body);

```


### <a name="create_browse_node_lookup20"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateBrowseNodeLookup20") CreateBrowseNodeLookup20

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.BrowseNodeLookupResponseMsg> CreateBrowseNodeLookup20(Models.BrowseNodeLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.BrowseNodeLookupRequestMsg();

Models.BrowseNodeLookupResponseMsg result = await aWSECommerceServiceBinding.CreateBrowseNodeLookup20(body);

```


### <a name="create_item_lookup19"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateItemLookup19") CreateItemLookup19

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.ItemLookupResponseMsg> CreateItemLookup19(Models.ItemLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.ItemLookupRequestMsg();

Models.ItemLookupResponseMsg result = await aWSECommerceServiceBinding.CreateItemLookup19(body);

```


### <a name="create_item_search18"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateItemSearch18") CreateItemSearch18

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.ItemSearchResponseMsg> CreateItemSearch18(Models.ItemSearchRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.ItemSearchRequestMsg();

Models.ItemSearchResponseMsg result = await aWSECommerceServiceBinding.CreateItemSearch18(body);

```


### <a name="create_cart_clear17"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartClear17") CreateCartClear17

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartClearResponseMsg> CreateCartClear17(Models.CartClearRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartClearRequestMsg();

Models.CartClearResponseMsg result = await aWSECommerceServiceBinding.CreateCartClear17(body);

```


### <a name="create_cart_modify16"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartModify16") CreateCartModify16

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartModifyResponseMsg> CreateCartModify16(Models.CartModifyRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartModifyRequestMsg();

Models.CartModifyResponseMsg result = await aWSECommerceServiceBinding.CreateCartModify16(body);

```


### <a name="create_cart_create15"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartCreate15") CreateCartCreate15

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartCreateResponseMsg> CreateCartCreate15(Models.CartCreateRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartCreateRequestMsg();

Models.CartCreateResponseMsg result = await aWSECommerceServiceBinding.CreateCartCreate15(body);

```


### <a name="create_cart_add14"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartAdd14") CreateCartAdd14

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartAddResponseMsg> CreateCartAdd14(Models.CartAddRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartAddRequestMsg();

Models.CartAddResponseMsg result = await aWSECommerceServiceBinding.CreateCartAdd14(body);

```


### <a name="create_cart_get13"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartGet13") CreateCartGet13

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartGetResponseMsg> CreateCartGet13(Models.CartGetRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartGetRequestMsg();

Models.CartGetResponseMsg result = await aWSECommerceServiceBinding.CreateCartGet13(body);

```


### <a name="create_similarity_lookup12"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateSimilarityLookup12") CreateSimilarityLookup12

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.SimilarityLookupResponseMsg> CreateSimilarityLookup12(Models.SimilarityLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.SimilarityLookupRequestMsg();

Models.SimilarityLookupResponseMsg result = await aWSECommerceServiceBinding.CreateSimilarityLookup12(body);

```


### <a name="create_browse_node_lookup11"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateBrowseNodeLookup11") CreateBrowseNodeLookup11

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.BrowseNodeLookupResponseMsg> CreateBrowseNodeLookup11(Models.BrowseNodeLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.BrowseNodeLookupRequestMsg();

Models.BrowseNodeLookupResponseMsg result = await aWSECommerceServiceBinding.CreateBrowseNodeLookup11(body);

```


### <a name="create_item_lookup10"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateItemLookup10") CreateItemLookup10

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.ItemLookupResponseMsg> CreateItemLookup10(Models.ItemLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.ItemLookupRequestMsg();

Models.ItemLookupResponseMsg result = await aWSECommerceServiceBinding.CreateItemLookup10(body);

```


### <a name="create_item_search9"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateItemSearch9") CreateItemSearch9

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.ItemSearchResponseMsg> CreateItemSearch9(Models.ItemSearchRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.ItemSearchRequestMsg();

Models.ItemSearchResponseMsg result = await aWSECommerceServiceBinding.CreateItemSearch9(body);

```


### <a name="create_cart_clear"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartClear") CreateCartClear

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartClearResponseMsg> CreateCartClear(Models.CartClearRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartClearRequestMsg();

Models.CartClearResponseMsg result = await aWSECommerceServiceBinding.CreateCartClear(body);

```


### <a name="create_cart_modify"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartModify") CreateCartModify

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartModifyResponseMsg> CreateCartModify(Models.CartModifyRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartModifyRequestMsg();

Models.CartModifyResponseMsg result = await aWSECommerceServiceBinding.CreateCartModify(body);

```


### <a name="create_cart_create"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartCreate") CreateCartCreate

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartCreateResponseMsg> CreateCartCreate(Models.CartCreateRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartCreateRequestMsg();

Models.CartCreateResponseMsg result = await aWSECommerceServiceBinding.CreateCartCreate(body);

```


### <a name="create_cart_add"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartAdd") CreateCartAdd

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartAddResponseMsg> CreateCartAdd(Models.CartAddRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartAddRequestMsg();

Models.CartAddResponseMsg result = await aWSECommerceServiceBinding.CreateCartAdd(body);

```


### <a name="create_cart_get"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateCartGet") CreateCartGet

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.CartGetResponseMsg> CreateCartGet(Models.CartGetRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.CartGetRequestMsg();

Models.CartGetResponseMsg result = await aWSECommerceServiceBinding.CreateCartGet(body);

```


### <a name="create_similarity_lookup"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateSimilarityLookup") CreateSimilarityLookup

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.SimilarityLookupResponseMsg> CreateSimilarityLookup(Models.SimilarityLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.SimilarityLookupRequestMsg();

Models.SimilarityLookupResponseMsg result = await aWSECommerceServiceBinding.CreateSimilarityLookup(body);

```


### <a name="create_browse_node_lookup"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateBrowseNodeLookup") CreateBrowseNodeLookup

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.BrowseNodeLookupResponseMsg> CreateBrowseNodeLookup(Models.BrowseNodeLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.BrowseNodeLookupRequestMsg();

Models.BrowseNodeLookupResponseMsg result = await aWSECommerceServiceBinding.CreateBrowseNodeLookup(body);

```


### <a name="create_item_lookup"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateItemLookup") CreateItemLookup

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.ItemLookupResponseMsg> CreateItemLookup(Models.ItemLookupRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.ItemLookupRequestMsg();

Models.ItemLookupResponseMsg result = await aWSECommerceServiceBinding.CreateItemLookup(body);

```


### <a name="create_item_search"></a>![Method: ](https://apidocs.io/img/method.png "AWSECommerceService.PCL.Controllers.AWSECommerceServiceBindingController.CreateItemSearch") CreateItemSearch

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```csharp
Task<Models.ItemSearchResponseMsg> CreateItemSearch(Models.ItemSearchRequestMsg body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```csharp
var body = new Models.ItemSearchRequestMsg();

Models.ItemSearchResponseMsg result = await aWSECommerceServiceBinding.CreateItemSearch(body);

```


[Back to List of Controllers](#list_of_controllers)



