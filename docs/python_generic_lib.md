# Getting started

## How to Build


You must have Python 2 >=2.7.9 or Python 3 >=3.4 installed on your system to install and run this SDK. This SDK package depends on other Python packages like nose, jsonpickle etc. 
These dependencies are defined in the ```requirements.txt``` file that comes with the SDK.
To resolve these dependencies, you can use the PIP Dependency manager. Install it by following steps at [https://pip.pypa.io/en/stable/installing/](https://pip.pypa.io/en/stable/installing/).

Python and PIP executables should be defined in your PATH. Open command prompt and type ```pip --version```.
This should display the version of the PIP Dependency Manager installed if your installation was successful and the paths are properly defined.

* Using command line, navigate to the directory containing the generated files (including ```requirements.txt```) for the SDK.
* Run the command ```pip install -r requirements.txt```. This should install all the required dependencies.

![Building SDK - Step 1](https://apidocs.io/illustration/python?step=installDependencies&workspaceFolder=AWSECommerceService-Python)


## How to Use

The following section explains how to use the Awsecommerceservice SDK package in a new project.

### 1. Open Project in an IDE

Open up a Python IDE like PyCharm. The basic workflow presented here is also applicable if you prefer using a different editor or IDE.

![Open project in PyCharm - Step 1](https://apidocs.io/illustration/python?step=pyCharm)

Click on ```Open``` in PyCharm to browse to your generated SDK directory and then click ```OK```.

![Open project in PyCharm - Step 2](https://apidocs.io/illustration/python?step=openProject0&workspaceFolder=AWSECommerceService-Python)     

The project files will be displayed in the side bar as follows:

![Open project in PyCharm - Step 3](https://apidocs.io/illustration/python?step=openProject1&workspaceFolder=AWSECommerceService-Python&projectName=awsecommerceservice)     

### 2. Add a new Test Project

Create a new directory by right clicking on the solution name as shown below:

![Add a new project in PyCharm - Step 1](https://apidocs.io/illustration/python?step=createDirectory&workspaceFolder=AWSECommerceService-Python&projectName=awsecommerceservice)

Name the directory as "test"

![Add a new project in PyCharm - Step 2](https://apidocs.io/illustration/python?step=nameDirectory)
   
Add a python file to this project with the name "testsdk"

![Add a new project in PyCharm - Step 3](https://apidocs.io/illustration/python?step=createFile&workspaceFolder=AWSECommerceService-Python&projectName=awsecommerceservice)

Name it "testsdk"

![Add a new project in PyCharm - Step 4](https://apidocs.io/illustration/python?step=nameFile)

In your python file you will be required to import the generated python library using the following code lines

```Python
from awsecommerceservice.awsecommerceservice_client import AwsecommerceserviceClient
```

![Add a new project in PyCharm - Step 4](https://apidocs.io/illustration/python?step=projectFiles&workspaceFolder=AWSECommerceService-Python&libraryName=awsecommerceservice.awsecommerceservice_client&projectName=awsecommerceservice)

After this you can write code to instantiate an API client object, get a controller object and  make API calls. Sample code is given in the subsequent sections.

### 3. Run the Test Project

To run the file within your test project, right click on your Python file inside your Test project and click on ```Run```

![Run Test Project - Step 1](https://apidocs.io/illustration/python?step=runProject&workspaceFolder=AWSECommerceService-Python&libraryName=awsecommerceservice.awsecommerceservice_client&projectName=awsecommerceservice)


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

client = AwsecommerceserviceClient()
```



# Class Reference

## <a name="list_of_controllers"></a>List of Controllers

* [AWSECommerceServiceBindingController](#awse_commerce_service_binding_controller)

## <a name="awse_commerce_service_binding_controller"></a>![Class: ](https://apidocs.io/img/class.png ".AWSECommerceServiceBindingController") AWSECommerceServiceBindingController

### Get controller instance

An instance of the ``` AWSECommerceServiceBindingController ``` class can be accessed from the API Client.

```python
 awse_commerce_service_binding_client = client.awse_commerce_service_binding
```

### <a name="create_cart_modify_97"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_modify_97") create_cart_modify_97

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_modify_97(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartModifyRequestMsg()

result = awse_commerce_service_binding_client.create_cart_modify_97(body)

```


### <a name="create_cart_clear_98"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_clear_98") create_cart_clear_98

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_clear_98(self,
                             body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartClearRequestMsg()

result = awse_commerce_service_binding_client.create_cart_clear_98(body)

```


### <a name="create_cart_create_96"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_create_96") create_cart_create_96

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_create_96(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartCreateRequestMsg()

result = awse_commerce_service_binding_client.create_cart_create_96(body)

```


### <a name="create_cart_add_95"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_add_95") create_cart_add_95

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_add_95(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartAddRequestMsg()

result = awse_commerce_service_binding_client.create_cart_add_95(body)

```


### <a name="create_cart_get_94"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_get_94") create_cart_get_94

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_get_94(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartGetRequestMsg()

result = awse_commerce_service_binding_client.create_cart_get_94(body)

```


### <a name="create_similarity_lookup_93"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_similarity_lookup_93") create_similarity_lookup_93

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_similarity_lookup_93(self,
                                    body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = SimilarityLookupRequestMsg()

result = awse_commerce_service_binding_client.create_similarity_lookup_93(body)

```


### <a name="create_browse_node_lookup_92"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_browse_node_lookup_92") create_browse_node_lookup_92

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_browse_node_lookup_92(self,
                                     body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = BrowseNodeLookupRequestMsg()

result = awse_commerce_service_binding_client.create_browse_node_lookup_92(body)

```


### <a name="create_item_lookup_91"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_item_lookup_91") create_item_lookup_91

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_item_lookup_91(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ItemLookupRequestMsg()

result = awse_commerce_service_binding_client.create_item_lookup_91(body)

```


### <a name="create_item_search_90"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_item_search_90") create_item_search_90

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_item_search_90(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ItemSearchRequestMsg()

result = awse_commerce_service_binding_client.create_item_search_90(body)

```


### <a name="create_cart_clear_89"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_clear_89") create_cart_clear_89

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_clear_89(self,
                             body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartClearRequestMsg()

result = awse_commerce_service_binding_client.create_cart_clear_89(body)

```


### <a name="create_cart_modify_88"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_modify_88") create_cart_modify_88

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_modify_88(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartModifyRequestMsg()

result = awse_commerce_service_binding_client.create_cart_modify_88(body)

```


### <a name="create_cart_create_87"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_create_87") create_cart_create_87

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_create_87(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartCreateRequestMsg()

result = awse_commerce_service_binding_client.create_cart_create_87(body)

```


### <a name="create_cart_add_86"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_add_86") create_cart_add_86

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_add_86(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartAddRequestMsg()

result = awse_commerce_service_binding_client.create_cart_add_86(body)

```


### <a name="create_cart_get_85"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_get_85") create_cart_get_85

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_get_85(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartGetRequestMsg()

result = awse_commerce_service_binding_client.create_cart_get_85(body)

```


### <a name="create_similarity_lookup_84"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_similarity_lookup_84") create_similarity_lookup_84

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_similarity_lookup_84(self,
                                    body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = SimilarityLookupRequestMsg()

result = awse_commerce_service_binding_client.create_similarity_lookup_84(body)

```


### <a name="create_browse_node_lookup_83"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_browse_node_lookup_83") create_browse_node_lookup_83

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_browse_node_lookup_83(self,
                                     body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = BrowseNodeLookupRequestMsg()

result = awse_commerce_service_binding_client.create_browse_node_lookup_83(body)

```


### <a name="create_item_lookup_82"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_item_lookup_82") create_item_lookup_82

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_item_lookup_82(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ItemLookupRequestMsg()

result = awse_commerce_service_binding_client.create_item_lookup_82(body)

```


### <a name="create_item_search_81"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_item_search_81") create_item_search_81

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_item_search_81(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ItemSearchRequestMsg()

result = awse_commerce_service_binding_client.create_item_search_81(body)

```


### <a name="create_cart_clear_80"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_clear_80") create_cart_clear_80

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_clear_80(self,
                             body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartClearRequestMsg()

result = awse_commerce_service_binding_client.create_cart_clear_80(body)

```


### <a name="create_cart_modify_79"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_modify_79") create_cart_modify_79

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_modify_79(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartModifyRequestMsg()

result = awse_commerce_service_binding_client.create_cart_modify_79(body)

```


### <a name="create_cart_create_78"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_create_78") create_cart_create_78

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_create_78(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartCreateRequestMsg()

result = awse_commerce_service_binding_client.create_cart_create_78(body)

```


### <a name="create_cart_add_77"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_add_77") create_cart_add_77

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_add_77(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartAddRequestMsg()

result = awse_commerce_service_binding_client.create_cart_add_77(body)

```


### <a name="create_cart_get_76"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_get_76") create_cart_get_76

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_get_76(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartGetRequestMsg()

result = awse_commerce_service_binding_client.create_cart_get_76(body)

```


### <a name="create_similarity_lookup_75"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_similarity_lookup_75") create_similarity_lookup_75

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_similarity_lookup_75(self,
                                    body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = SimilarityLookupRequestMsg()

result = awse_commerce_service_binding_client.create_similarity_lookup_75(body)

```


### <a name="create_browse_node_lookup_74"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_browse_node_lookup_74") create_browse_node_lookup_74

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_browse_node_lookup_74(self,
                                     body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = BrowseNodeLookupRequestMsg()

result = awse_commerce_service_binding_client.create_browse_node_lookup_74(body)

```


### <a name="create_item_lookup_73"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_item_lookup_73") create_item_lookup_73

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_item_lookup_73(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ItemLookupRequestMsg()

result = awse_commerce_service_binding_client.create_item_lookup_73(body)

```


### <a name="create_item_search_72"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_item_search_72") create_item_search_72

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_item_search_72(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ItemSearchRequestMsg()

result = awse_commerce_service_binding_client.create_item_search_72(body)

```


### <a name="create_cart_clear_71"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_clear_71") create_cart_clear_71

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_clear_71(self,
                             body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartClearRequestMsg()

result = awse_commerce_service_binding_client.create_cart_clear_71(body)

```


### <a name="create_cart_modify_70"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_modify_70") create_cart_modify_70

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_modify_70(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartModifyRequestMsg()

result = awse_commerce_service_binding_client.create_cart_modify_70(body)

```


### <a name="create_cart_create_69"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_create_69") create_cart_create_69

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_create_69(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartCreateRequestMsg()

result = awse_commerce_service_binding_client.create_cart_create_69(body)

```


### <a name="create_cart_add_68"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_add_68") create_cart_add_68

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_add_68(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartAddRequestMsg()

result = awse_commerce_service_binding_client.create_cart_add_68(body)

```


### <a name="create_cart_get_67"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_get_67") create_cart_get_67

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_get_67(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartGetRequestMsg()

result = awse_commerce_service_binding_client.create_cart_get_67(body)

```


### <a name="create_similarity_lookup_66"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_similarity_lookup_66") create_similarity_lookup_66

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_similarity_lookup_66(self,
                                    body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = SimilarityLookupRequestMsg()

result = awse_commerce_service_binding_client.create_similarity_lookup_66(body)

```


### <a name="create_browse_node_lookup_65"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_browse_node_lookup_65") create_browse_node_lookup_65

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_browse_node_lookup_65(self,
                                     body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = BrowseNodeLookupRequestMsg()

result = awse_commerce_service_binding_client.create_browse_node_lookup_65(body)

```


### <a name="create_item_lookup_64"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_item_lookup_64") create_item_lookup_64

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_item_lookup_64(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ItemLookupRequestMsg()

result = awse_commerce_service_binding_client.create_item_lookup_64(body)

```


### <a name="create_item_search_63"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_item_search_63") create_item_search_63

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_item_search_63(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ItemSearchRequestMsg()

result = awse_commerce_service_binding_client.create_item_search_63(body)

```


### <a name="create_cart_clear_62"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_clear_62") create_cart_clear_62

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_clear_62(self,
                             body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartClearRequestMsg()

result = awse_commerce_service_binding_client.create_cart_clear_62(body)

```


### <a name="create_cart_modify_61"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_modify_61") create_cart_modify_61

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_modify_61(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartModifyRequestMsg()

result = awse_commerce_service_binding_client.create_cart_modify_61(body)

```


### <a name="create_cart_create_60"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_create_60") create_cart_create_60

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_create_60(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartCreateRequestMsg()

result = awse_commerce_service_binding_client.create_cart_create_60(body)

```


### <a name="create_cart_add_59"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_add_59") create_cart_add_59

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_add_59(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartAddRequestMsg()

result = awse_commerce_service_binding_client.create_cart_add_59(body)

```


### <a name="create_cart_get_58"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_get_58") create_cart_get_58

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_get_58(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartGetRequestMsg()

result = awse_commerce_service_binding_client.create_cart_get_58(body)

```


### <a name="create_similarity_lookup_57"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_similarity_lookup_57") create_similarity_lookup_57

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_similarity_lookup_57(self,
                                    body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = SimilarityLookupRequestMsg()

result = awse_commerce_service_binding_client.create_similarity_lookup_57(body)

```


### <a name="create_browse_node_lookup_56"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_browse_node_lookup_56") create_browse_node_lookup_56

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_browse_node_lookup_56(self,
                                     body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = BrowseNodeLookupRequestMsg()

result = awse_commerce_service_binding_client.create_browse_node_lookup_56(body)

```


### <a name="create_item_lookup_55"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_item_lookup_55") create_item_lookup_55

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_item_lookup_55(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ItemLookupRequestMsg()

result = awse_commerce_service_binding_client.create_item_lookup_55(body)

```


### <a name="create_item_search_54"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_item_search_54") create_item_search_54

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_item_search_54(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ItemSearchRequestMsg()

result = awse_commerce_service_binding_client.create_item_search_54(body)

```


### <a name="create_cart_clear_53"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_clear_53") create_cart_clear_53

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_clear_53(self,
                             body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartClearRequestMsg()

result = awse_commerce_service_binding_client.create_cart_clear_53(body)

```


### <a name="create_cart_modify_52"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_modify_52") create_cart_modify_52

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_modify_52(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartModifyRequestMsg()

result = awse_commerce_service_binding_client.create_cart_modify_52(body)

```


### <a name="create_cart_create_51"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_create_51") create_cart_create_51

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_create_51(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartCreateRequestMsg()

result = awse_commerce_service_binding_client.create_cart_create_51(body)

```


### <a name="create_cart_add_50"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_add_50") create_cart_add_50

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_add_50(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartAddRequestMsg()

result = awse_commerce_service_binding_client.create_cart_add_50(body)

```


### <a name="create_cart_get_49"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_get_49") create_cart_get_49

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_get_49(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartGetRequestMsg()

result = awse_commerce_service_binding_client.create_cart_get_49(body)

```


### <a name="create_similarity_lookup_48"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_similarity_lookup_48") create_similarity_lookup_48

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_similarity_lookup_48(self,
                                    body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = SimilarityLookupRequestMsg()

result = awse_commerce_service_binding_client.create_similarity_lookup_48(body)

```


### <a name="create_browse_node_lookup_47"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_browse_node_lookup_47") create_browse_node_lookup_47

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_browse_node_lookup_47(self,
                                     body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = BrowseNodeLookupRequestMsg()

result = awse_commerce_service_binding_client.create_browse_node_lookup_47(body)

```


### <a name="create_item_lookup_46"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_item_lookup_46") create_item_lookup_46

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_item_lookup_46(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ItemLookupRequestMsg()

result = awse_commerce_service_binding_client.create_item_lookup_46(body)

```


### <a name="create_item_search_45"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_item_search_45") create_item_search_45

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_item_search_45(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ItemSearchRequestMsg()

result = awse_commerce_service_binding_client.create_item_search_45(body)

```


### <a name="create_cart_clear_44"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_clear_44") create_cart_clear_44

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_clear_44(self,
                             body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartClearRequestMsg()

result = awse_commerce_service_binding_client.create_cart_clear_44(body)

```


### <a name="create_cart_modify_43"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_modify_43") create_cart_modify_43

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_modify_43(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartModifyRequestMsg()

result = awse_commerce_service_binding_client.create_cart_modify_43(body)

```


### <a name="create_cart_create_42"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_create_42") create_cart_create_42

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_create_42(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartCreateRequestMsg()

result = awse_commerce_service_binding_client.create_cart_create_42(body)

```


### <a name="create_cart_add_41"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_add_41") create_cart_add_41

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_add_41(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartAddRequestMsg()

result = awse_commerce_service_binding_client.create_cart_add_41(body)

```


### <a name="create_cart_get_40"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_get_40") create_cart_get_40

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_get_40(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartGetRequestMsg()

result = awse_commerce_service_binding_client.create_cart_get_40(body)

```


### <a name="create_similarity_lookup_39"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_similarity_lookup_39") create_similarity_lookup_39

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_similarity_lookup_39(self,
                                    body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = SimilarityLookupRequestMsg()

result = awse_commerce_service_binding_client.create_similarity_lookup_39(body)

```


### <a name="create_browse_node_lookup_38"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_browse_node_lookup_38") create_browse_node_lookup_38

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_browse_node_lookup_38(self,
                                     body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = BrowseNodeLookupRequestMsg()

result = awse_commerce_service_binding_client.create_browse_node_lookup_38(body)

```


### <a name="create_item_lookup_37"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_item_lookup_37") create_item_lookup_37

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_item_lookup_37(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ItemLookupRequestMsg()

result = awse_commerce_service_binding_client.create_item_lookup_37(body)

```


### <a name="create_item_search_36"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_item_search_36") create_item_search_36

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_item_search_36(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ItemSearchRequestMsg()

result = awse_commerce_service_binding_client.create_item_search_36(body)

```


### <a name="create_cart_clear_35"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_clear_35") create_cart_clear_35

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_clear_35(self,
                             body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartClearRequestMsg()

result = awse_commerce_service_binding_client.create_cart_clear_35(body)

```


### <a name="create_cart_modify_34"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_modify_34") create_cart_modify_34

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_modify_34(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartModifyRequestMsg()

result = awse_commerce_service_binding_client.create_cart_modify_34(body)

```


### <a name="create_cart_create_33"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_create_33") create_cart_create_33

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_create_33(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartCreateRequestMsg()

result = awse_commerce_service_binding_client.create_cart_create_33(body)

```


### <a name="create_cart_add_32"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_add_32") create_cart_add_32

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_add_32(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartAddRequestMsg()

result = awse_commerce_service_binding_client.create_cart_add_32(body)

```


### <a name="create_cart_get_31"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_get_31") create_cart_get_31

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_get_31(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartGetRequestMsg()

result = awse_commerce_service_binding_client.create_cart_get_31(body)

```


### <a name="create_similarity_lookup_30"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_similarity_lookup_30") create_similarity_lookup_30

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_similarity_lookup_30(self,
                                    body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = SimilarityLookupRequestMsg()

result = awse_commerce_service_binding_client.create_similarity_lookup_30(body)

```


### <a name="create_browse_node_lookup_29"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_browse_node_lookup_29") create_browse_node_lookup_29

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_browse_node_lookup_29(self,
                                     body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = BrowseNodeLookupRequestMsg()

result = awse_commerce_service_binding_client.create_browse_node_lookup_29(body)

```


### <a name="create_item_lookup_28"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_item_lookup_28") create_item_lookup_28

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_item_lookup_28(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ItemLookupRequestMsg()

result = awse_commerce_service_binding_client.create_item_lookup_28(body)

```


### <a name="create_item_search_27"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_item_search_27") create_item_search_27

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_item_search_27(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ItemSearchRequestMsg()

result = awse_commerce_service_binding_client.create_item_search_27(body)

```


### <a name="create_cart_clear_26"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_clear_26") create_cart_clear_26

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_clear_26(self,
                             body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartClearRequestMsg()

result = awse_commerce_service_binding_client.create_cart_clear_26(body)

```


### <a name="create_cart_modify_25"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_modify_25") create_cart_modify_25

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_modify_25(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartModifyRequestMsg()

result = awse_commerce_service_binding_client.create_cart_modify_25(body)

```


### <a name="create_cart_create_24"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_create_24") create_cart_create_24

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_create_24(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartCreateRequestMsg()

result = awse_commerce_service_binding_client.create_cart_create_24(body)

```


### <a name="create_cart_add_23"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_add_23") create_cart_add_23

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_add_23(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartAddRequestMsg()

result = awse_commerce_service_binding_client.create_cart_add_23(body)

```


### <a name="create_cart_get_22"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_get_22") create_cart_get_22

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_get_22(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartGetRequestMsg()

result = awse_commerce_service_binding_client.create_cart_get_22(body)

```


### <a name="create_similarity_lookup_21"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_similarity_lookup_21") create_similarity_lookup_21

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_similarity_lookup_21(self,
                                    body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = SimilarityLookupRequestMsg()

result = awse_commerce_service_binding_client.create_similarity_lookup_21(body)

```


### <a name="create_browse_node_lookup_20"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_browse_node_lookup_20") create_browse_node_lookup_20

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_browse_node_lookup_20(self,
                                     body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = BrowseNodeLookupRequestMsg()

result = awse_commerce_service_binding_client.create_browse_node_lookup_20(body)

```


### <a name="create_item_lookup_19"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_item_lookup_19") create_item_lookup_19

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_item_lookup_19(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ItemLookupRequestMsg()

result = awse_commerce_service_binding_client.create_item_lookup_19(body)

```


### <a name="create_item_search_18"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_item_search_18") create_item_search_18

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_item_search_18(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ItemSearchRequestMsg()

result = awse_commerce_service_binding_client.create_item_search_18(body)

```


### <a name="create_cart_clear_17"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_clear_17") create_cart_clear_17

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_clear_17(self,
                             body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartClearRequestMsg()

result = awse_commerce_service_binding_client.create_cart_clear_17(body)

```


### <a name="create_cart_modify_16"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_modify_16") create_cart_modify_16

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_modify_16(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartModifyRequestMsg()

result = awse_commerce_service_binding_client.create_cart_modify_16(body)

```


### <a name="create_cart_create_15"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_create_15") create_cart_create_15

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_create_15(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartCreateRequestMsg()

result = awse_commerce_service_binding_client.create_cart_create_15(body)

```


### <a name="create_cart_add_14"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_add_14") create_cart_add_14

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_add_14(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartAddRequestMsg()

result = awse_commerce_service_binding_client.create_cart_add_14(body)

```


### <a name="create_cart_get_13"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_get_13") create_cart_get_13

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_get_13(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartGetRequestMsg()

result = awse_commerce_service_binding_client.create_cart_get_13(body)

```


### <a name="create_similarity_lookup_12"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_similarity_lookup_12") create_similarity_lookup_12

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_similarity_lookup_12(self,
                                    body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = SimilarityLookupRequestMsg()

result = awse_commerce_service_binding_client.create_similarity_lookup_12(body)

```


### <a name="create_browse_node_lookup_11"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_browse_node_lookup_11") create_browse_node_lookup_11

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_browse_node_lookup_11(self,
                                     body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = BrowseNodeLookupRequestMsg()

result = awse_commerce_service_binding_client.create_browse_node_lookup_11(body)

```


### <a name="create_item_lookup_10"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_item_lookup_10") create_item_lookup_10

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_item_lookup_10(self,
                              body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ItemLookupRequestMsg()

result = awse_commerce_service_binding_client.create_item_lookup_10(body)

```


### <a name="create_item_search_9"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_item_search_9") create_item_search_9

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_item_search_9(self,
                             body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ItemSearchRequestMsg()

result = awse_commerce_service_binding_client.create_item_search_9(body)

```


### <a name="create_cart_clear"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_clear") create_cart_clear

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_clear(self,
                          body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartClearRequestMsg()

result = awse_commerce_service_binding_client.create_cart_clear(body)

```


### <a name="create_cart_modify"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_modify") create_cart_modify

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_modify(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartModifyRequestMsg()

result = awse_commerce_service_binding_client.create_cart_modify(body)

```


### <a name="create_cart_create"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_create") create_cart_create

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_create(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartCreateRequestMsg()

result = awse_commerce_service_binding_client.create_cart_create(body)

```


### <a name="create_cart_add"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_add") create_cart_add

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_add(self,
                        body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartAddRequestMsg()

result = awse_commerce_service_binding_client.create_cart_add(body)

```


### <a name="create_cart_get"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_cart_get") create_cart_get

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_cart_get(self,
                        body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = CartGetRequestMsg()

result = awse_commerce_service_binding_client.create_cart_get(body)

```


### <a name="create_similarity_lookup"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_similarity_lookup") create_similarity_lookup

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_similarity_lookup(self,
                                 body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = SimilarityLookupRequestMsg()

result = awse_commerce_service_binding_client.create_similarity_lookup(body)

```


### <a name="create_browse_node_lookup"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_browse_node_lookup") create_browse_node_lookup

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_browse_node_lookup(self,
                                  body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = BrowseNodeLookupRequestMsg()

result = awse_commerce_service_binding_client.create_browse_node_lookup(body)

```


### <a name="create_item_lookup"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_item_lookup") create_item_lookup

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_item_lookup(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ItemLookupRequestMsg()

result = awse_commerce_service_binding_client.create_item_lookup(body)

```


### <a name="create_item_search"></a>![Method: ](https://apidocs.io/img/method.png ".AWSECommerceServiceBindingController.create_item_search") create_item_search

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description

```python
def create_item_search(self,
                           body)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```python
body = ItemSearchRequestMsg()

result = awse_commerce_service_binding_client.create_item_search(body)

```


[Back to List of Controllers](#list_of_controllers)



