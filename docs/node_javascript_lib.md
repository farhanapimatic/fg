# Getting started

## How to Build

The generated SDK relies on [Node Package Manager](https://www.npmjs.com/) (NPM) being available to resolve dependencies. If you don't already have NPM installed, please go ahead and follow instructions to install NPM from [here](https://nodejs.org/en/download/).
The SDK also requires Node to be installed. If Node isn't already installed, please install it from [here](https://nodejs.org/en/download/)
> NPM is installed by default when Node is installed

To check if node and npm have been successfully installed, write the following commands in command prompt:

* `node --version`
* `npm -version`

![Version Check](https://apidocs.io/illustration/nodejs?step=versionCheck&workspaceFolder=AWSECommerceService-Node)

Now use npm to resolve all dependencies by running the following command in the root directory (of the SDK folder):

```bash
npm install
```

![Resolve Dependencies](https://apidocs.io/illustration/nodejs?step=resolveDependency1&workspaceFolder=AWSECommerceService-Node)

![Resolve Dependencies](https://apidocs.io/illustration/nodejs?step=resolveDependency2)

This will install all dependencies in the `node_modules` folder.

Once dependencies are resolved, you will need to move the folder `AWSECommerceServiceLib ` in to your `node_modules` folder.

## How to Use

The following section explains how to use the library in a new project.

### 1. Open Project Folder
Open an IDE/Text Editor for JavaScript like Sublime Text. The basic workflow presented here is also applicable if you prefer using a different editor or IDE.

Click on `File` and select `Open Folder`.

![Open Folder](https://apidocs.io/illustration/nodejs?step=openFolder)

Select the folder of your SDK and click on `Select Folder` to open it up in Sublime Text. The folder will become visible in the bar on the left.

![Open Project](https://apidocs.io/illustration/nodejs?step=openProject&workspaceFolder=AWSECommerceService-Node)

### 2. Creating a Test File

Now right click on the folder name and select the `New File` option to create a new test file. Save it as `index.js` Now import the generated NodeJS library using the following lines of code:

```js
var lib = require('lib');
```

Save changes.

![Create new file](https://apidocs.io/illustration/nodejs?step=createNewFile&workspaceFolder=AWSECommerceService-Node)

![Save new file](https://apidocs.io/illustration/nodejs?step=saveNewFile&workspaceFolder=AWSECommerceService-Node)

### 3. Running The Test File

To run the `index.js` file, open up the command prompt and navigate to the Path where the SDK folder resides. Type the following command to run the file:

```
node index.js
```

![Run file](https://apidocs.io/illustration/nodejs?step=runProject&workspaceFolder=AWSECommerceService-Node)


## How to Test

These tests use Mocha framework for testing, coupled with Chai for assertions. These dependencies need to be installed for tests to run.
Tests can be run in a number of ways:

### Method 1 (Run all tests)

1. Navigate to the root directory of the SDK folder from command prompt.
2. Type `mocha --recursive` to run all the tests.

### Method 2 (Run all tests)

1. Navigate to the `../test/Controllers/` directory from command prompt.
2. Type `mocha *` to run all the tests.

### Method 3 (Run specific controller's tests)

1. Navigate to the `../test/Controllers/` directory from command prompt.
2. Type `mocha  AWSECommerceServiceController`  to run all the tests in that controller file.

> To increase mocha's default timeout, you can change the `TEST_TIMEOUT` parameter's value in `TestBootstrap.js`.

![Run Tests](https://apidocs.io/illustration/nodejs?step=runTests&controllerName=AWSECommerceServiceController)

## Initialization

### 

API client can be initialized as following:

```JavaScript
const lib = require('lib');


```



# Class Reference

## <a name="list_of_controllers"></a>List of Controllers

* [AWSECommerceServiceBindingController](#awse_commerce_service_binding_controller)

## <a name="awse_commerce_service_binding_controller"></a>![Class: ](https://apidocs.io/img/class.png ".AWSECommerceServiceBindingController") AWSECommerceServiceBindingController

### Get singleton instance

The singleton instance of the ``` AWSECommerceServiceBindingController ``` class can be accessed from the API Client.

```javascript
var controller = lib.AWSECommerceServiceBindingController;
```

### <a name="create_cart_modify70"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartModify70") createCartModify70

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartModify70(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartModifyRequestMsg({"key":"value"});

    controller.createCartModify70(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_create69"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartCreate69") createCartCreate69

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartCreate69(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartCreateRequestMsg({"key":"value"});

    controller.createCartCreate69(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_add68"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartAdd68") createCartAdd68

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartAdd68(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartAddRequestMsg({"key":"value"});

    controller.createCartAdd68(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_get67"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartGet67") createCartGet67

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartGet67(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartGetRequestMsg({"key":"value"});

    controller.createCartGet67(body, function(error, response, context) {

    
    });
```



### <a name="create_similarity_lookup66"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createSimilarityLookup66") createSimilarityLookup66

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createSimilarityLookup66(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new SimilarityLookupRequestMsg({"key":"value"});

    controller.createSimilarityLookup66(body, function(error, response, context) {

    
    });
```



### <a name="create_browse_node_lookup65"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createBrowseNodeLookup65") createBrowseNodeLookup65

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createBrowseNodeLookup65(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new BrowseNodeLookupRequestMsg({"key":"value"});

    controller.createBrowseNodeLookup65(body, function(error, response, context) {

    
    });
```



### <a name="create_item_lookup64"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createItemLookup64") createItemLookup64

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createItemLookup64(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ItemLookupRequestMsg({"key":"value"});

    controller.createItemLookup64(body, function(error, response, context) {

    
    });
```



### <a name="create_item_search63"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createItemSearch63") createItemSearch63

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createItemSearch63(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ItemSearchRequestMsg({"key":"value"});

    controller.createItemSearch63(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_clear62"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartClear62") createCartClear62

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartClear62(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartClearRequestMsg({"key":"value"});

    controller.createCartClear62(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_modify61"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartModify61") createCartModify61

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartModify61(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartModifyRequestMsg({"key":"value"});

    controller.createCartModify61(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_create60"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartCreate60") createCartCreate60

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartCreate60(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartCreateRequestMsg({"key":"value"});

    controller.createCartCreate60(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_add59"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartAdd59") createCartAdd59

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartAdd59(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartAddRequestMsg({"key":"value"});

    controller.createCartAdd59(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_get58"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartGet58") createCartGet58

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartGet58(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartGetRequestMsg({"key":"value"});

    controller.createCartGet58(body, function(error, response, context) {

    
    });
```



### <a name="create_similarity_lookup57"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createSimilarityLookup57") createSimilarityLookup57

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createSimilarityLookup57(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new SimilarityLookupRequestMsg({"key":"value"});

    controller.createSimilarityLookup57(body, function(error, response, context) {

    
    });
```



### <a name="create_browse_node_lookup56"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createBrowseNodeLookup56") createBrowseNodeLookup56

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createBrowseNodeLookup56(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new BrowseNodeLookupRequestMsg({"key":"value"});

    controller.createBrowseNodeLookup56(body, function(error, response, context) {

    
    });
```



### <a name="create_item_lookup55"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createItemLookup55") createItemLookup55

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createItemLookup55(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ItemLookupRequestMsg({"key":"value"});

    controller.createItemLookup55(body, function(error, response, context) {

    
    });
```



### <a name="create_item_search54"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createItemSearch54") createItemSearch54

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createItemSearch54(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ItemSearchRequestMsg({"key":"value"});

    controller.createItemSearch54(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_clear53"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartClear53") createCartClear53

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartClear53(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartClearRequestMsg({"key":"value"});

    controller.createCartClear53(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_modify52"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartModify52") createCartModify52

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartModify52(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartModifyRequestMsg({"key":"value"});

    controller.createCartModify52(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_create51"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartCreate51") createCartCreate51

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartCreate51(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartCreateRequestMsg({"key":"value"});

    controller.createCartCreate51(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_add50"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartAdd50") createCartAdd50

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartAdd50(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartAddRequestMsg({"key":"value"});

    controller.createCartAdd50(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_get49"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartGet49") createCartGet49

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartGet49(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartGetRequestMsg({"key":"value"});

    controller.createCartGet49(body, function(error, response, context) {

    
    });
```



### <a name="create_similarity_lookup48"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createSimilarityLookup48") createSimilarityLookup48

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createSimilarityLookup48(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new SimilarityLookupRequestMsg({"key":"value"});

    controller.createSimilarityLookup48(body, function(error, response, context) {

    
    });
```



### <a name="create_browse_node_lookup47"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createBrowseNodeLookup47") createBrowseNodeLookup47

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createBrowseNodeLookup47(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new BrowseNodeLookupRequestMsg({"key":"value"});

    controller.createBrowseNodeLookup47(body, function(error, response, context) {

    
    });
```



### <a name="create_item_lookup46"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createItemLookup46") createItemLookup46

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createItemLookup46(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ItemLookupRequestMsg({"key":"value"});

    controller.createItemLookup46(body, function(error, response, context) {

    
    });
```



### <a name="create_item_search45"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createItemSearch45") createItemSearch45

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createItemSearch45(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ItemSearchRequestMsg({"key":"value"});

    controller.createItemSearch45(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_clear44"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartClear44") createCartClear44

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartClear44(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartClearRequestMsg({"key":"value"});

    controller.createCartClear44(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_modify43"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartModify43") createCartModify43

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartModify43(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartModifyRequestMsg({"key":"value"});

    controller.createCartModify43(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_create42"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartCreate42") createCartCreate42

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartCreate42(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartCreateRequestMsg({"key":"value"});

    controller.createCartCreate42(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_add41"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartAdd41") createCartAdd41

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartAdd41(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartAddRequestMsg({"key":"value"});

    controller.createCartAdd41(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_get40"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartGet40") createCartGet40

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartGet40(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartGetRequestMsg({"key":"value"});

    controller.createCartGet40(body, function(error, response, context) {

    
    });
```



### <a name="create_similarity_lookup39"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createSimilarityLookup39") createSimilarityLookup39

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createSimilarityLookup39(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new SimilarityLookupRequestMsg({"key":"value"});

    controller.createSimilarityLookup39(body, function(error, response, context) {

    
    });
```



### <a name="create_browse_node_lookup38"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createBrowseNodeLookup38") createBrowseNodeLookup38

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createBrowseNodeLookup38(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new BrowseNodeLookupRequestMsg({"key":"value"});

    controller.createBrowseNodeLookup38(body, function(error, response, context) {

    
    });
```



### <a name="create_item_lookup37"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createItemLookup37") createItemLookup37

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createItemLookup37(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ItemLookupRequestMsg({"key":"value"});

    controller.createItemLookup37(body, function(error, response, context) {

    
    });
```



### <a name="create_item_search36"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createItemSearch36") createItemSearch36

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createItemSearch36(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ItemSearchRequestMsg({"key":"value"});

    controller.createItemSearch36(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_clear35"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartClear35") createCartClear35

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartClear35(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartClearRequestMsg({"key":"value"});

    controller.createCartClear35(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_modify34"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartModify34") createCartModify34

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartModify34(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartModifyRequestMsg({"key":"value"});

    controller.createCartModify34(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_create33"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartCreate33") createCartCreate33

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartCreate33(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartCreateRequestMsg({"key":"value"});

    controller.createCartCreate33(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_add32"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartAdd32") createCartAdd32

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartAdd32(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartAddRequestMsg({"key":"value"});

    controller.createCartAdd32(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_get31"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartGet31") createCartGet31

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartGet31(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartGetRequestMsg({"key":"value"});

    controller.createCartGet31(body, function(error, response, context) {

    
    });
```



### <a name="create_similarity_lookup30"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createSimilarityLookup30") createSimilarityLookup30

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createSimilarityLookup30(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new SimilarityLookupRequestMsg({"key":"value"});

    controller.createSimilarityLookup30(body, function(error, response, context) {

    
    });
```



### <a name="create_browse_node_lookup29"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createBrowseNodeLookup29") createBrowseNodeLookup29

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createBrowseNodeLookup29(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new BrowseNodeLookupRequestMsg({"key":"value"});

    controller.createBrowseNodeLookup29(body, function(error, response, context) {

    
    });
```



### <a name="create_item_lookup28"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createItemLookup28") createItemLookup28

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createItemLookup28(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ItemLookupRequestMsg({"key":"value"});

    controller.createItemLookup28(body, function(error, response, context) {

    
    });
```



### <a name="create_item_search27"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createItemSearch27") createItemSearch27

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createItemSearch27(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ItemSearchRequestMsg({"key":"value"});

    controller.createItemSearch27(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_clear26"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartClear26") createCartClear26

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartClear26(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartClearRequestMsg({"key":"value"});

    controller.createCartClear26(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_modify25"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartModify25") createCartModify25

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartModify25(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartModifyRequestMsg({"key":"value"});

    controller.createCartModify25(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_create24"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartCreate24") createCartCreate24

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartCreate24(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartCreateRequestMsg({"key":"value"});

    controller.createCartCreate24(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_add23"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartAdd23") createCartAdd23

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartAdd23(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartAddRequestMsg({"key":"value"});

    controller.createCartAdd23(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_get22"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartGet22") createCartGet22

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartGet22(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartGetRequestMsg({"key":"value"});

    controller.createCartGet22(body, function(error, response, context) {

    
    });
```



### <a name="create_similarity_lookup21"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createSimilarityLookup21") createSimilarityLookup21

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createSimilarityLookup21(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new SimilarityLookupRequestMsg({"key":"value"});

    controller.createSimilarityLookup21(body, function(error, response, context) {

    
    });
```



### <a name="create_browse_node_lookup20"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createBrowseNodeLookup20") createBrowseNodeLookup20

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createBrowseNodeLookup20(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new BrowseNodeLookupRequestMsg({"key":"value"});

    controller.createBrowseNodeLookup20(body, function(error, response, context) {

    
    });
```



### <a name="create_item_lookup19"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createItemLookup19") createItemLookup19

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createItemLookup19(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ItemLookupRequestMsg({"key":"value"});

    controller.createItemLookup19(body, function(error, response, context) {

    
    });
```



### <a name="create_item_search18"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createItemSearch18") createItemSearch18

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createItemSearch18(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ItemSearchRequestMsg({"key":"value"});

    controller.createItemSearch18(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_clear17"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartClear17") createCartClear17

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartClear17(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartClearRequestMsg({"key":"value"});

    controller.createCartClear17(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_modify16"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartModify16") createCartModify16

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartModify16(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartModifyRequestMsg({"key":"value"});

    controller.createCartModify16(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_create15"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartCreate15") createCartCreate15

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartCreate15(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartCreateRequestMsg({"key":"value"});

    controller.createCartCreate15(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_add14"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartAdd14") createCartAdd14

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartAdd14(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartAddRequestMsg({"key":"value"});

    controller.createCartAdd14(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_get13"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartGet13") createCartGet13

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartGet13(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartGetRequestMsg({"key":"value"});

    controller.createCartGet13(body, function(error, response, context) {

    
    });
```



### <a name="create_similarity_lookup12"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createSimilarityLookup12") createSimilarityLookup12

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createSimilarityLookup12(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new SimilarityLookupRequestMsg({"key":"value"});

    controller.createSimilarityLookup12(body, function(error, response, context) {

    
    });
```



### <a name="create_browse_node_lookup11"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createBrowseNodeLookup11") createBrowseNodeLookup11

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createBrowseNodeLookup11(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new BrowseNodeLookupRequestMsg({"key":"value"});

    controller.createBrowseNodeLookup11(body, function(error, response, context) {

    
    });
```



### <a name="create_item_lookup10"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createItemLookup10") createItemLookup10

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createItemLookup10(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ItemLookupRequestMsg({"key":"value"});

    controller.createItemLookup10(body, function(error, response, context) {

    
    });
```



### <a name="create_item_search9"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createItemSearch9") createItemSearch9

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createItemSearch9(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ItemSearchRequestMsg({"key":"value"});

    controller.createItemSearch9(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_clear"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartClear") createCartClear

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartClear(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartClearRequestMsg({"key":"value"});

    controller.createCartClear(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_modify"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartModify") createCartModify

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartModify(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartModifyRequestMsg({"key":"value"});

    controller.createCartModify(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_create"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartCreate") createCartCreate

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartCreate(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartCreateRequestMsg({"key":"value"});

    controller.createCartCreate(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_add"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartAdd") createCartAdd

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartAdd(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartAddRequestMsg({"key":"value"});

    controller.createCartAdd(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_get"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartGet") createCartGet

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartGet(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartGetRequestMsg({"key":"value"});

    controller.createCartGet(body, function(error, response, context) {

    
    });
```



### <a name="create_similarity_lookup"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createSimilarityLookup") createSimilarityLookup

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createSimilarityLookup(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new SimilarityLookupRequestMsg({"key":"value"});

    controller.createSimilarityLookup(body, function(error, response, context) {

    
    });
```



### <a name="create_browse_node_lookup"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createBrowseNodeLookup") createBrowseNodeLookup

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createBrowseNodeLookup(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new BrowseNodeLookupRequestMsg({"key":"value"});

    controller.createBrowseNodeLookup(body, function(error, response, context) {

    
    });
```



### <a name="create_item_lookup"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createItemLookup") createItemLookup

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createItemLookup(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ItemLookupRequestMsg({"key":"value"});

    controller.createItemLookup(body, function(error, response, context) {

    
    });
```



### <a name="create_item_search"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createItemSearch") createItemSearch

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createItemSearch(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ItemSearchRequestMsg({"key":"value"});

    controller.createItemSearch(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_clear71"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartClear71") createCartClear71

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartClear71(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartClearRequestMsg({"key":"value"});

    controller.createCartClear71(body, function(error, response, context) {

    
    });
```



### <a name="create_item_search72"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createItemSearch72") createItemSearch72

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createItemSearch72(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ItemSearchRequestMsg({"key":"value"});

    controller.createItemSearch72(body, function(error, response, context) {

    
    });
```



### <a name="create_item_lookup73"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createItemLookup73") createItemLookup73

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createItemLookup73(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ItemLookupRequestMsg({"key":"value"});

    controller.createItemLookup73(body, function(error, response, context) {

    
    });
```



### <a name="create_browse_node_lookup74"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createBrowseNodeLookup74") createBrowseNodeLookup74

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createBrowseNodeLookup74(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new BrowseNodeLookupRequestMsg({"key":"value"});

    controller.createBrowseNodeLookup74(body, function(error, response, context) {

    
    });
```



### <a name="create_similarity_lookup75"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createSimilarityLookup75") createSimilarityLookup75

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createSimilarityLookup75(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new SimilarityLookupRequestMsg({"key":"value"});

    controller.createSimilarityLookup75(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_get76"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartGet76") createCartGet76

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartGet76(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartGetRequestMsg({"key":"value"});

    controller.createCartGet76(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_add77"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartAdd77") createCartAdd77

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartAdd77(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartAddRequestMsg({"key":"value"});

    controller.createCartAdd77(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_create78"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartCreate78") createCartCreate78

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartCreate78(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartCreateRequestMsg({"key":"value"});

    controller.createCartCreate78(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_modify79"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartModify79") createCartModify79

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartModify79(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartModifyRequestMsg({"key":"value"});

    controller.createCartModify79(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_clear80"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartClear80") createCartClear80

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartClear80(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartClearRequestMsg({"key":"value"});

    controller.createCartClear80(body, function(error, response, context) {

    
    });
```



### <a name="create_item_search81"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createItemSearch81") createItemSearch81

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createItemSearch81(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ItemSearchRequestMsg({"key":"value"});

    controller.createItemSearch81(body, function(error, response, context) {

    
    });
```



### <a name="create_item_lookup82"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createItemLookup82") createItemLookup82

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createItemLookup82(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ItemLookupRequestMsg({"key":"value"});

    controller.createItemLookup82(body, function(error, response, context) {

    
    });
```



### <a name="create_browse_node_lookup83"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createBrowseNodeLookup83") createBrowseNodeLookup83

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createBrowseNodeLookup83(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new BrowseNodeLookupRequestMsg({"key":"value"});

    controller.createBrowseNodeLookup83(body, function(error, response, context) {

    
    });
```



### <a name="create_similarity_lookup84"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createSimilarityLookup84") createSimilarityLookup84

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createSimilarityLookup84(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new SimilarityLookupRequestMsg({"key":"value"});

    controller.createSimilarityLookup84(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_get85"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartGet85") createCartGet85

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartGet85(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartGetRequestMsg({"key":"value"});

    controller.createCartGet85(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_add86"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartAdd86") createCartAdd86

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartAdd86(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartAddRequestMsg({"key":"value"});

    controller.createCartAdd86(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_create87"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartCreate87") createCartCreate87

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartCreate87(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartCreateRequestMsg({"key":"value"});

    controller.createCartCreate87(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_modify88"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartModify88") createCartModify88

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartModify88(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartModifyRequestMsg({"key":"value"});

    controller.createCartModify88(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_clear89"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartClear89") createCartClear89

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartClear89(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartClearRequestMsg({"key":"value"});

    controller.createCartClear89(body, function(error, response, context) {

    
    });
```



### <a name="create_item_search90"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createItemSearch90") createItemSearch90

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createItemSearch90(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ItemSearchRequestMsg({"key":"value"});

    controller.createItemSearch90(body, function(error, response, context) {

    
    });
```



### <a name="create_item_lookup91"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createItemLookup91") createItemLookup91

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createItemLookup91(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new ItemLookupRequestMsg({"key":"value"});

    controller.createItemLookup91(body, function(error, response, context) {

    
    });
```



### <a name="create_browse_node_lookup92"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createBrowseNodeLookup92") createBrowseNodeLookup92

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createBrowseNodeLookup92(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new BrowseNodeLookupRequestMsg({"key":"value"});

    controller.createBrowseNodeLookup92(body, function(error, response, context) {

    
    });
```



### <a name="create_similarity_lookup93"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createSimilarityLookup93") createSimilarityLookup93

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createSimilarityLookup93(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new SimilarityLookupRequestMsg({"key":"value"});

    controller.createSimilarityLookup93(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_get94"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartGet94") createCartGet94

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartGet94(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartGetRequestMsg({"key":"value"});

    controller.createCartGet94(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_add95"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartAdd95") createCartAdd95

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartAdd95(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartAddRequestMsg({"key":"value"});

    controller.createCartAdd95(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_create96"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartCreate96") createCartCreate96

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartCreate96(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartCreateRequestMsg({"key":"value"});

    controller.createCartCreate96(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_modify97"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartModify97") createCartModify97

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartModify97(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartModifyRequestMsg({"key":"value"});

    controller.createCartModify97(body, function(error, response, context) {

    
    });
```



### <a name="create_cart_clear98"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.createCartClear98") createCartClear98

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```javascript
function createCartClear98(body, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var body = new CartClearRequestMsg({"key":"value"});

    controller.createCartClear98(body, function(error, response, context) {

    
    });
```



[Back to List of Controllers](#list_of_controllers)



