# 

this is one of the test description



## Server Configuration for Base URLs

This section provides details on the environments available and lists down the servers in each of the environment. The default environment for this API is set to `production` while the default server is set to `AWSECommerceServicePort`.
### Environments

An environment consists of a set of servers with base URL values. The environment can be changed programatically allowing rapid switching between different environments e.g.the user can specify a Production and Testing Environment.The available environments for this API are: 

#### production
The environment comprises of the following servers: 

| Name | Base URL | 
|-----------|-------------|
| AWSECommerceServicePort | https://webservices.amazon.com/onca/soap?Service=AWSECommerceService |
| AWSECommerceServicePortCA | https://webservices.amazon.ca/onca/soap?Service=AWSECommerceService |
| AWSECommerceServicePortCN | https://webservices.amazon.cn/onca/soap?Service=AWSECommerceService |
| AWSECommerceServicePortDE | https://webservices.amazon.de/onca/soap?Service=AWSECommerceService |
| AWSECommerceServicePortES | https://webservices.amazon.es/onca/soap?Service=AWSECommerceService |
| AWSECommerceServicePortFR | https://webservices.amazon.fr/onca/soap?Service=AWSECommerceService |
| AWSECommerceServicePortIN | https://webservices.amazon.in/onca/soap?Service=AWSECommerceService |
| AWSECommerceServicePortIT | https://webservices.amazon.it/onca/soap?Service=AWSECommerceService |
| AWSECommerceServicePortJP | https://webservices.amazon.co.jp/onca/soap?Service=AWSECommerceService |
| AWSECommerceServicePortUK | https://webservices.amazon.co.uk/onca/soap?Service=AWSECommerceService |
| AWSECommerceServicePortUS | https://webservices.amazon.com/onca/soap?Service=AWSECommerceService |




## Authentication
This API uses `OAuth v2.0` with `Authorization Code` grant type.

#### Authorization Endpoint
Authorization grant can be obtained from the authorization endpoint at path `/sedsadasdasd`. It will use server `AWSECommerceServicePort` which will serve as the base URL for this endpoint. 
#### Token Endpoint
Access token can be obtained from the token endpoint at path `/sdsdfsdfsdfsdf`. It will use server `AWSECommerceServicePort` which will serve as the base URL for this endpoint. 





# <a name="api_reference"></a>API Reference

* [AWSECommerceServiceBinding](#awse_commerce_service_binding)
* [OAuth Authorization](#o_auth_authorization)

## <a name="awse_commerce_service_binding"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "AWSECommerceServiceBinding") AWSECommerceServiceBinding


### <a name="item_search"></a>![Endpoint: ](https://apidocs.io/img/method.png "ItemSearch") ItemSearch


**`POST`** `/ItemSearch`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ItemSearchRequestMsg](#item_search_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "XMLEscaping": "XMLEscaping",
    "Validate": "Validate",
    "Shared": {
      "Availability": "Available",
      "Actor": "Actor",
      "Artist": "Artist",
      "AudienceRating": [
        "G"
      ],
      "Author": "Author",
      "Brand": "Brand",
      "BrowseNode": "BrowseNode",
      "Composer": "Composer",
      "Condition": "All",
      "Conductor": "Conductor",
      "Director": "Director",
      "ItemPage": 55,
      "Keywords": "Keywords",
      "Manufacturer": "Manufacturer",
      "MaximumPrice": 55,
      "MerchantId": "MerchantId",
      "MinimumPrice": 55,
      "MinPercentageOff": 55,
      "MusicLabel": "MusicLabel",
      "Orchestra": "Orchestra",
      "Power": "Power",
      "Publisher": "Publisher",
      "RelatedItemPage": "RelatedItemPage",
      "RelationshipType": [
        "RelationshipType"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ],
      "SearchIndex": "SearchIndex",
      "Sort": "Sort",
      "Title": "Title",
      "ReleaseDate": "ReleaseDate",
      "IncludeReviewsSummary": "IncludeReviewsSummary",
      "TruncateReviewsAt": 55
    },
    "Request": [
      {
        "Availability": "Available",
        "Actor": "Actor",
        "Artist": "Artist",
        "AudienceRating": [
          "G"
        ],
        "Author": "Author",
        "Brand": "Brand",
        "BrowseNode": "BrowseNode",
        "Composer": "Composer",
        "Condition": "All",
        "Conductor": "Conductor",
        "Director": "Director",
        "ItemPage": 55,
        "Keywords": "Keywords",
        "Manufacturer": "Manufacturer",
        "MaximumPrice": 55,
        "MerchantId": "MerchantId",
        "MinimumPrice": 55,
        "MinPercentageOff": 55,
        "MusicLabel": "MusicLabel",
        "Orchestra": "Orchestra",
        "Power": "Power",
        "Publisher": "Publisher",
        "RelatedItemPage": "RelatedItemPage",
        "RelationshipType": [
          "RelationshipType"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ],
        "SearchIndex": "SearchIndex",
        "Sort": "Sort",
        "Title": "Title",
        "ReleaseDate": "ReleaseDate",
        "IncludeReviewsSummary": "IncludeReviewsSummary",
        "TruncateReviewsAt": 55
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([ItemSearchResponseMsg](#item_search_response_msg)) 
```
{
  "body": {
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 55,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    },
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 55.1342747733622
    }
  }
}
```


### <a name="item_lookup"></a>![Endpoint: ](https://apidocs.io/img/method.png "ItemLookup") ItemLookup


**`POST`** `/ItemLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ItemLookupRequestMsg](#item_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Condition": "All",
      "IdType": "ASIN",
      "MerchantId": "MerchantId",
      "ItemId": [
        "ItemId"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ],
      "SearchIndex": "SearchIndex",
      "VariationPage": "VariationPage",
      "RelatedItemPage": "RelatedItemPage",
      "RelationshipType": [
        "RelationshipType"
      ],
      "IncludeReviewsSummary": "IncludeReviewsSummary",
      "TruncateReviewsAt": 55
    },
    "Request": [
      {
        "Condition": "All",
        "IdType": "ASIN",
        "MerchantId": "MerchantId",
        "ItemId": [
          "ItemId"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ],
        "SearchIndex": "SearchIndex",
        "VariationPage": "VariationPage",
        "RelatedItemPage": "RelatedItemPage",
        "RelationshipType": [
          "RelationshipType"
        ],
        "IncludeReviewsSummary": "IncludeReviewsSummary",
        "TruncateReviewsAt": 55
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([ItemLookupResponseMsg](#item_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 55.1342747733622
    },
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 55,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    }
  }
}
```


### <a name="browse_node_lookup"></a>![Endpoint: ](https://apidocs.io/img/method.png "BrowseNodeLookup") BrowseNodeLookup


**`POST`** `/BrowseNodeLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [BrowseNodeLookupRequestMsg](#browse_node_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "BrowseNodeId": [
        "BrowseNodeId"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "BrowseNodeId": [
          "BrowseNodeId"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([BrowseNodeLookupResponseMsg](#browse_node_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 55.1342747733622
    },
    "BrowseNodes": [
      {
        "Request": {
          "BrowseNodeLookupRequest": {
            "BrowseNodeId": [
              "BrowseNodeId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "ItemSearchRequest": {
            "Availability": "Available",
            "Actor": "Actor",
            "Artist": "Artist",
            "AudienceRating": [
              "G"
            ],
            "Author": "Author",
            "Brand": "Brand",
            "BrowseNode": "BrowseNode",
            "Composer": "Composer",
            "Condition": "All",
            "Conductor": "Conductor",
            "Director": "Director",
            "ItemPage": 55,
            "Keywords": "Keywords",
            "Manufacturer": "Manufacturer",
            "MaximumPrice": 55,
            "MerchantId": "MerchantId",
            "MinimumPrice": 55,
            "MinPercentageOff": 55,
            "MusicLabel": "MusicLabel",
            "Orchestra": "Orchestra",
            "Power": "Power",
            "Publisher": "Publisher",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "Sort": "Sort",
            "Title": "Title",
            "ReleaseDate": "ReleaseDate",
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 55
          },
          "ItemLookupRequest": {
            "Condition": "All",
            "IdType": "ASIN",
            "MerchantId": "MerchantId",
            "ItemId": [
              "ItemId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "VariationPage": "VariationPage",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 55
          },
          "SimilarityLookupRequest": {
            "Condition": "All",
            "SimilarityType": "Intersection",
            "ItemId": [
              "ItemId"
            ],
            "MerchantId": "MerchantId",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartGetRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartAddRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 146,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartCreateRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 146,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartModifyRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 146,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartClearRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "Errors": {
            "Error": {
              "Code": "Code",
              "Message": "Message"
            }
          },
          "IsValid": "IsValid"
        },
        "BrowseNode": [
          {
            "Properties": {
              "Property": [
                {
                  "Name": "Name",
                  "Value": "Value"
                }
              ]
            },
            "Children": {
              "BrowseNode": []
            },
            "Ancestors": {
              "BrowseNode": []
            },
            "TopSellers": {
              "TopSeller": {
                "ASIN": "ASIN",
                "Title": "Title"
              }
            },
            "NewReleases": {
              "NewRelease": {
                "ASIN": "ASIN",
                "Title": "Title"
              }
            },
            "BrowseNodeId": "BrowseNodeId",
            "Name": "Name",
            "IsCategoryRoot": true,
            "TopItemSet": [
              {
                "TopItem": {
                  "ASIN": "ASIN",
                  "Title": "Title",
                  "DetailPageURL": "DetailPageURL",
                  "ProductGroup": "ProductGroup",
                  "Author": [
                    "Author"
                  ],
                  "Artist": [
                    "Artist"
                  ],
                  "Actor": [
                    "Actor"
                  ]
                },
                "Type": "Type"
              }
            ]
          }
        ]
      }
    ]
  }
}
```


### <a name="similarity_lookup"></a>![Endpoint: ](https://apidocs.io/img/method.png "SimilarityLookup") SimilarityLookup


**`POST`** `/SimilarityLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [SimilarityLookupRequestMsg](#similarity_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Condition": "All",
      "SimilarityType": "Intersection",
      "ItemId": [
        "ItemId"
      ],
      "MerchantId": "MerchantId",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Condition": "All",
        "SimilarityType": "Intersection",
        "ItemId": [
          "ItemId"
        ],
        "MerchantId": "MerchantId",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([SimilarityLookupResponseMsg](#similarity_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 146.629556665025
    },
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 146,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    }
  }
}
```


### <a name="cart_get"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartGet") CartGet


**`POST`** `/CartGet`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartGetRequestMsg](#cart_get_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartGetResponseMsg](#cart_get_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 146.629556665025
    },
    "Cart": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "URLEncodedHMAC": "URLEncodedHMAC",
        "Request": {
          "BrowseNodeLookupRequest": {
            "BrowseNodeId": [
              "BrowseNodeId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "ItemSearchRequest": {
            "Availability": "Available",
            "Actor": "Actor",
            "Artist": "Artist",
            "AudienceRating": [
              "G"
            ],
            "Author": "Author",
            "Brand": "Brand",
            "BrowseNode": "BrowseNode",
            "Composer": "Composer",
            "Condition": "All",
            "Conductor": "Conductor",
            "Director": "Director",
            "ItemPage": 146,
            "Keywords": "Keywords",
            "Manufacturer": "Manufacturer",
            "MaximumPrice": 146,
            "MerchantId": "MerchantId",
            "MinimumPrice": 146,
            "MinPercentageOff": 146,
            "MusicLabel": "MusicLabel",
            "Orchestra": "Orchestra",
            "Power": "Power",
            "Publisher": "Publisher",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "Sort": "Sort",
            "Title": "Title",
            "ReleaseDate": "ReleaseDate",
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 146
          },
          "ItemLookupRequest": {
            "Condition": "All",
            "IdType": "ASIN",
            "MerchantId": "MerchantId",
            "ItemId": [
              "ItemId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "VariationPage": "VariationPage",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 146
          },
          "SimilarityLookupRequest": {
            "Condition": "All",
            "SimilarityType": "Intersection",
            "ItemId": [
              "ItemId"
            ],
            "MerchantId": "MerchantId",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartGetRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartAddRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 238,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartCreateRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 238,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartModifyRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 238,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartClearRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "Errors": {
            "Error": {
              "Code": "Code",
              "Message": "Message"
            }
          },
          "IsValid": "IsValid"
        },
        "PurchaseURL": "PurchaseURL",
        "MobileCartURL": "MobileCartURL",
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 238,
          "CurrencyCode": "CurrencyCode"
        },
        "CartItems": {
          "CartItem": [
            {
              "CartItemId": "CartItemId",
              "Quantity": "Quantity",
              "MetaData": {
                "KeyValuePair": {
                  "Key": "Key",
                  "Value": "Value"
                }
              },
              "Price": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 238,
                "CurrencyCode": "CurrencyCode"
              },
              "ASIN": "ASIN",
              "SellerNickname": "SellerNickname",
              "Title": "Title",
              "ProductGroup": "ProductGroup",
              "ItemTotal": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 238,
                "CurrencyCode": "CurrencyCode"
              }
            }
          ],
          "SubTotal": {
            "FormattedPrice": "FormattedPrice",
            "Amount": 238,
            "CurrencyCode": "CurrencyCode"
          }
        },
        "SavedForLaterItems": {
          "SavedForLaterItem": [
            {
              "CartItemId": "CartItemId",
              "Quantity": "Quantity",
              "MetaData": {
                "KeyValuePair": {
                  "Key": "Key",
                  "Value": "Value"
                }
              },
              "Price": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 238,
                "CurrencyCode": "CurrencyCode"
              },
              "ASIN": "ASIN",
              "SellerNickname": "SellerNickname",
              "Title": "Title",
              "ProductGroup": "ProductGroup",
              "ItemTotal": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 238,
                "CurrencyCode": "CurrencyCode"
              }
            }
          ],
          "SubTotal": {
            "FormattedPrice": "FormattedPrice",
            "Amount": 238,
            "CurrencyCode": "CurrencyCode"
          }
        },
        "SimilarProducts": {
          "SimilarProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "TopSellers": {
          "TopSeller": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "NewReleases": {
          "NewRelease": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "SimilarViewedProducts": {
          "SimilarViewedProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "OtherCategoriesSimilarProducts": {
          "OtherCategoriesSimilarProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        }
      }
    ]
  }
}
```


### <a name="cart_add"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartAdd") CartAdd


**`POST`** `/CartAdd`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartAddRequestMsg](#cart_add_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 238,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 238,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartAddResponseMsg](#cart_add_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 238.124838556687
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 238,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 238,
          "MerchantId": "MerchantId",
          "MinimumPrice": 238,
          "MinPercentageOff": 238,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 238
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 238
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 238,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 238,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 196,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 196,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 196,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 196,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 196,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 196,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 196,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 196,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_create"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartCreate") CartCreate


**`POST`** `/CartCreate`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartCreateRequestMsg](#cart_create_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 196,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 196,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartCreateResponseMsg](#cart_create_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 196.40166533012
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 196,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 196,
          "MerchantId": "MerchantId",
          "MinimumPrice": 196,
          "MinPercentageOff": 196,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 196
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 196
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 196,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 196,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 196,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 32,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 32,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 32,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 32,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 32,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 32,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 32,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_modify"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartModify") CartModify


**`POST`** `/CartModify`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartModifyRequestMsg](#cart_modify_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 32,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 32,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartModifyResponseMsg](#cart_modify_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 32.8969472217825
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 32,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 32,
          "MerchantId": "MerchantId",
          "MinimumPrice": 32,
          "MinPercentageOff": 32,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 32
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 32
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 32,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 32,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 32,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 246,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 246,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 246,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 246,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 246,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 246,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 246,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_clear"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartClear") CartClear


**`POST`** `/CartClear`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description




#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartClearRequestMsg](#cart_clear_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartClearResponseMsg](#cart_clear_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 246.173773995216
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 246,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 246,
          "MerchantId": "MerchantId",
          "MinimumPrice": 246,
          "MinPercentageOff": 246,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 246
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 246
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 246,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 246,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 246,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 82,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 82,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 82,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 82,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 82,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 82,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 82,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="item_search9"></a>![Endpoint: ](https://apidocs.io/img/method.png "ItemSearch9") ItemSearch9


**`POST`** `/ItemSearch`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortCA`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ItemSearchRequestMsg](#item_search_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "XMLEscaping": "XMLEscaping",
    "Validate": "Validate",
    "Shared": {
      "Availability": "Available",
      "Actor": "Actor",
      "Artist": "Artist",
      "AudienceRating": [
        "G"
      ],
      "Author": "Author",
      "Brand": "Brand",
      "BrowseNode": "BrowseNode",
      "Composer": "Composer",
      "Condition": "All",
      "Conductor": "Conductor",
      "Director": "Director",
      "ItemPage": 82,
      "Keywords": "Keywords",
      "Manufacturer": "Manufacturer",
      "MaximumPrice": 82,
      "MerchantId": "MerchantId",
      "MinimumPrice": 82,
      "MinPercentageOff": 82,
      "MusicLabel": "MusicLabel",
      "Orchestra": "Orchestra",
      "Power": "Power",
      "Publisher": "Publisher",
      "RelatedItemPage": "RelatedItemPage",
      "RelationshipType": [
        "RelationshipType"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ],
      "SearchIndex": "SearchIndex",
      "Sort": "Sort",
      "Title": "Title",
      "ReleaseDate": "ReleaseDate",
      "IncludeReviewsSummary": "IncludeReviewsSummary",
      "TruncateReviewsAt": 82
    },
    "Request": [
      {
        "Availability": "Available",
        "Actor": "Actor",
        "Artist": "Artist",
        "AudienceRating": [
          "G"
        ],
        "Author": "Author",
        "Brand": "Brand",
        "BrowseNode": "BrowseNode",
        "Composer": "Composer",
        "Condition": "All",
        "Conductor": "Conductor",
        "Director": "Director",
        "ItemPage": 82,
        "Keywords": "Keywords",
        "Manufacturer": "Manufacturer",
        "MaximumPrice": 82,
        "MerchantId": "MerchantId",
        "MinimumPrice": 82,
        "MinPercentageOff": 82,
        "MusicLabel": "MusicLabel",
        "Orchestra": "Orchestra",
        "Power": "Power",
        "Publisher": "Publisher",
        "RelatedItemPage": "RelatedItemPage",
        "RelationshipType": [
          "RelationshipType"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ],
        "SearchIndex": "SearchIndex",
        "Sort": "Sort",
        "Title": "Title",
        "ReleaseDate": "ReleaseDate",
        "IncludeReviewsSummary": "IncludeReviewsSummary",
        "TruncateReviewsAt": 82
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([ItemSearchResponseMsg](#item_search_response_msg)) 
```
{
  "body": {
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 82,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    },
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 82.6690558868782
    }
  }
}
```


### <a name="item_lookup10"></a>![Endpoint: ](https://apidocs.io/img/method.png "ItemLookup10") ItemLookup10


**`POST`** `/ItemLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortCA`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ItemLookupRequestMsg](#item_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Condition": "All",
      "IdType": "ASIN",
      "MerchantId": "MerchantId",
      "ItemId": [
        "ItemId"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ],
      "SearchIndex": "SearchIndex",
      "VariationPage": "VariationPage",
      "RelatedItemPage": "RelatedItemPage",
      "RelationshipType": [
        "RelationshipType"
      ],
      "IncludeReviewsSummary": "IncludeReviewsSummary",
      "TruncateReviewsAt": 82
    },
    "Request": [
      {
        "Condition": "All",
        "IdType": "ASIN",
        "MerchantId": "MerchantId",
        "ItemId": [
          "ItemId"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ],
        "SearchIndex": "SearchIndex",
        "VariationPage": "VariationPage",
        "RelatedItemPage": "RelatedItemPage",
        "RelationshipType": [
          "RelationshipType"
        ],
        "IncludeReviewsSummary": "IncludeReviewsSummary",
        "TruncateReviewsAt": 82
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([ItemLookupResponseMsg](#item_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 82.6690558868782
    },
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 82,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    }
  }
}
```


### <a name="browse_node_lookup11"></a>![Endpoint: ](https://apidocs.io/img/method.png "BrowseNodeLookup11") BrowseNodeLookup11


**`POST`** `/BrowseNodeLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortCA`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [BrowseNodeLookupRequestMsg](#browse_node_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "BrowseNodeId": [
        "BrowseNodeId"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "BrowseNodeId": [
          "BrowseNodeId"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([BrowseNodeLookupResponseMsg](#browse_node_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 174.16433777854
    },
    "BrowseNodes": [
      {
        "Request": {
          "BrowseNodeLookupRequest": {
            "BrowseNodeId": [
              "BrowseNodeId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "ItemSearchRequest": {
            "Availability": "Available",
            "Actor": "Actor",
            "Artist": "Artist",
            "AudienceRating": [
              "G"
            ],
            "Author": "Author",
            "Brand": "Brand",
            "BrowseNode": "BrowseNode",
            "Composer": "Composer",
            "Condition": "All",
            "Conductor": "Conductor",
            "Director": "Director",
            "ItemPage": 174,
            "Keywords": "Keywords",
            "Manufacturer": "Manufacturer",
            "MaximumPrice": 174,
            "MerchantId": "MerchantId",
            "MinimumPrice": 174,
            "MinPercentageOff": 174,
            "MusicLabel": "MusicLabel",
            "Orchestra": "Orchestra",
            "Power": "Power",
            "Publisher": "Publisher",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "Sort": "Sort",
            "Title": "Title",
            "ReleaseDate": "ReleaseDate",
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 174
          },
          "ItemLookupRequest": {
            "Condition": "All",
            "IdType": "ASIN",
            "MerchantId": "MerchantId",
            "ItemId": [
              "ItemId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "VariationPage": "VariationPage",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 174
          },
          "SimilarityLookupRequest": {
            "Condition": "All",
            "SimilarityType": "Intersection",
            "ItemId": [
              "ItemId"
            ],
            "MerchantId": "MerchantId",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartGetRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartAddRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 174,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartCreateRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 174,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartModifyRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 174,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartClearRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "Errors": {
            "Error": {
              "Code": "Code",
              "Message": "Message"
            }
          },
          "IsValid": "IsValid"
        },
        "BrowseNode": [
          {
            "Properties": {
              "Property": [
                {
                  "Name": "Name",
                  "Value": "Value"
                }
              ]
            },
            "Children": {
              "BrowseNode": []
            },
            "Ancestors": {
              "BrowseNode": []
            },
            "TopSellers": {
              "TopSeller": {
                "ASIN": "ASIN",
                "Title": "Title"
              }
            },
            "NewReleases": {
              "NewRelease": {
                "ASIN": "ASIN",
                "Title": "Title"
              }
            },
            "BrowseNodeId": "BrowseNodeId",
            "Name": "Name",
            "IsCategoryRoot": true,
            "TopItemSet": [
              {
                "TopItem": {
                  "ASIN": "ASIN",
                  "Title": "Title",
                  "DetailPageURL": "DetailPageURL",
                  "ProductGroup": "ProductGroup",
                  "Author": [
                    "Author"
                  ],
                  "Artist": [
                    "Artist"
                  ],
                  "Actor": [
                    "Actor"
                  ]
                },
                "Type": "Type"
              }
            ]
          }
        ]
      }
    ]
  }
}
```


### <a name="similarity_lookup12"></a>![Endpoint: ](https://apidocs.io/img/method.png "SimilarityLookup12") SimilarityLookup12


**`POST`** `/SimilarityLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortCA`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [SimilarityLookupRequestMsg](#similarity_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Condition": "All",
      "SimilarityType": "Intersection",
      "ItemId": [
        "ItemId"
      ],
      "MerchantId": "MerchantId",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Condition": "All",
        "SimilarityType": "Intersection",
        "ItemId": [
          "ItemId"
        ],
        "MerchantId": "MerchantId",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([SimilarityLookupResponseMsg](#similarity_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 174.16433777854
    },
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 174,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    }
  }
}
```


### <a name="cart_get13"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartGet13") CartGet13


**`POST`** `/CartGet`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortCA`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartGetRequestMsg](#cart_get_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartGetResponseMsg](#cart_get_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 174.16433777854
    },
    "Cart": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "URLEncodedHMAC": "URLEncodedHMAC",
        "Request": {
          "BrowseNodeLookupRequest": {
            "BrowseNodeId": [
              "BrowseNodeId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "ItemSearchRequest": {
            "Availability": "Available",
            "Actor": "Actor",
            "Artist": "Artist",
            "AudienceRating": [
              "G"
            ],
            "Author": "Author",
            "Brand": "Brand",
            "BrowseNode": "BrowseNode",
            "Composer": "Composer",
            "Condition": "All",
            "Conductor": "Conductor",
            "Director": "Director",
            "ItemPage": 132,
            "Keywords": "Keywords",
            "Manufacturer": "Manufacturer",
            "MaximumPrice": 132,
            "MerchantId": "MerchantId",
            "MinimumPrice": 132,
            "MinPercentageOff": 132,
            "MusicLabel": "MusicLabel",
            "Orchestra": "Orchestra",
            "Power": "Power",
            "Publisher": "Publisher",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "Sort": "Sort",
            "Title": "Title",
            "ReleaseDate": "ReleaseDate",
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 132
          },
          "ItemLookupRequest": {
            "Condition": "All",
            "IdType": "ASIN",
            "MerchantId": "MerchantId",
            "ItemId": [
              "ItemId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "VariationPage": "VariationPage",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 132
          },
          "SimilarityLookupRequest": {
            "Condition": "All",
            "SimilarityType": "Intersection",
            "ItemId": [
              "ItemId"
            ],
            "MerchantId": "MerchantId",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartGetRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartAddRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 132,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartCreateRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 132,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartModifyRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 132,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartClearRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "Errors": {
            "Error": {
              "Code": "Code",
              "Message": "Message"
            }
          },
          "IsValid": "IsValid"
        },
        "PurchaseURL": "PurchaseURL",
        "MobileCartURL": "MobileCartURL",
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 132,
          "CurrencyCode": "CurrencyCode"
        },
        "CartItems": {
          "CartItem": [
            {
              "CartItemId": "CartItemId",
              "Quantity": "Quantity",
              "MetaData": {
                "KeyValuePair": {
                  "Key": "Key",
                  "Value": "Value"
                }
              },
              "Price": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 132,
                "CurrencyCode": "CurrencyCode"
              },
              "ASIN": "ASIN",
              "SellerNickname": "SellerNickname",
              "Title": "Title",
              "ProductGroup": "ProductGroup",
              "ItemTotal": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 132,
                "CurrencyCode": "CurrencyCode"
              }
            }
          ],
          "SubTotal": {
            "FormattedPrice": "FormattedPrice",
            "Amount": 132,
            "CurrencyCode": "CurrencyCode"
          }
        },
        "SavedForLaterItems": {
          "SavedForLaterItem": [
            {
              "CartItemId": "CartItemId",
              "Quantity": "Quantity",
              "MetaData": {
                "KeyValuePair": {
                  "Key": "Key",
                  "Value": "Value"
                }
              },
              "Price": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 132,
                "CurrencyCode": "CurrencyCode"
              },
              "ASIN": "ASIN",
              "SellerNickname": "SellerNickname",
              "Title": "Title",
              "ProductGroup": "ProductGroup",
              "ItemTotal": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 132,
                "CurrencyCode": "CurrencyCode"
              }
            }
          ],
          "SubTotal": {
            "FormattedPrice": "FormattedPrice",
            "Amount": 132,
            "CurrencyCode": "CurrencyCode"
          }
        },
        "SimilarProducts": {
          "SimilarProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "TopSellers": {
          "TopSeller": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "NewReleases": {
          "NewRelease": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "SimilarViewedProducts": {
          "SimilarViewedProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "OtherCategoriesSimilarProducts": {
          "OtherCategoriesSimilarProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        }
      }
    ]
  }
}
```


### <a name="cart_add14"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartAdd14") CartAdd14


**`POST`** `/CartAdd`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortCA`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartAddRequestMsg](#cart_add_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 132,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 132,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartAddResponseMsg](#cart_add_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 132.441164551974
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 132,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 132,
          "MerchantId": "MerchantId",
          "MinimumPrice": 223,
          "MinPercentageOff": 223,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 223
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 223
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 223,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 223,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 223,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 223,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 223,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 223,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 223,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 223,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 223,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 223,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_create15"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartCreate15") CartCreate15


**`POST`** `/CartCreate`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortCA`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartCreateRequestMsg](#cart_create_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 223,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 223,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartCreateResponseMsg](#cart_create_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 223.936446443636
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 223,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 223,
          "MerchantId": "MerchantId",
          "MinimumPrice": 223,
          "MinPercentageOff": 223,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 223
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 60
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 60,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 60,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 60,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 60,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 60,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 60,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 60,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 60,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 60,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 60,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_modify16"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartModify16") CartModify16


**`POST`** `/CartModify`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortCA`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartModifyRequestMsg](#cart_modify_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 60,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 60,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartModifyResponseMsg](#cart_modify_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 18.7085551087319
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 18,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 18,
          "MerchantId": "MerchantId",
          "MinimumPrice": 18,
          "MinPercentageOff": 18,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 18
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 18
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 18,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 18,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 18,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 18,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 18,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 18,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 18,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 18,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 18,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 18,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_clear17"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartClear17") CartClear17


**`POST`** `/CartClear`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortCA`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartClearRequestMsg](#cart_clear_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartClearResponseMsg](#cart_clear_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 18.7085551087319
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 18,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 18,
          "MerchantId": "MerchantId",
          "MinimumPrice": 18,
          "MinPercentageOff": 18,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 18
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 110
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 110,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 110,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 110,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 110,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 110,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 110,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 110,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 110,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 110,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 110,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="item_search18"></a>![Endpoint: ](https://apidocs.io/img/method.png "ItemSearch18") ItemSearch18


**`POST`** `/ItemSearch`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortCN`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ItemSearchRequestMsg](#item_search_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "XMLEscaping": "XMLEscaping",
    "Validate": "Validate",
    "Shared": {
      "Availability": "Available",
      "Actor": "Actor",
      "Artist": "Artist",
      "AudienceRating": [
        "G"
      ],
      "Author": "Author",
      "Brand": "Brand",
      "BrowseNode": "BrowseNode",
      "Composer": "Composer",
      "Condition": "All",
      "Conductor": "Conductor",
      "Director": "Director",
      "ItemPage": 110,
      "Keywords": "Keywords",
      "Manufacturer": "Manufacturer",
      "MaximumPrice": 110,
      "MerchantId": "MerchantId",
      "MinimumPrice": 110,
      "MinPercentageOff": 110,
      "MusicLabel": "MusicLabel",
      "Orchestra": "Orchestra",
      "Power": "Power",
      "Publisher": "Publisher",
      "RelatedItemPage": "RelatedItemPage",
      "RelationshipType": [
        "RelationshipType"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ],
      "SearchIndex": "SearchIndex",
      "Sort": "Sort",
      "Title": "Title",
      "ReleaseDate": "ReleaseDate",
      "IncludeReviewsSummary": "IncludeReviewsSummary",
      "TruncateReviewsAt": 110
    },
    "Request": [
      {
        "Availability": "Available",
        "Actor": "Actor",
        "Artist": "Artist",
        "AudienceRating": [
          "G"
        ],
        "Author": "Author",
        "Brand": "Brand",
        "BrowseNode": "BrowseNode",
        "Composer": "Composer",
        "Condition": "All",
        "Conductor": "Conductor",
        "Director": "Director",
        "ItemPage": 110,
        "Keywords": "Keywords",
        "Manufacturer": "Manufacturer",
        "MaximumPrice": 110,
        "MerchantId": "MerchantId",
        "MinimumPrice": 110,
        "MinPercentageOff": 110,
        "MusicLabel": "MusicLabel",
        "Orchestra": "Orchestra",
        "Power": "Power",
        "Publisher": "Publisher",
        "RelatedItemPage": "RelatedItemPage",
        "RelationshipType": [
          "RelationshipType"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ],
        "SearchIndex": "SearchIndex",
        "Sort": "Sort",
        "Title": "Title",
        "ReleaseDate": "ReleaseDate",
        "IncludeReviewsSummary": "IncludeReviewsSummary",
        "TruncateReviewsAt": 110
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([ItemSearchResponseMsg](#item_search_response_msg)) 
```
{
  "body": {
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 110,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    },
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 68.4806637738276
    }
  }
}
```


### <a name="item_lookup19"></a>![Endpoint: ](https://apidocs.io/img/method.png "ItemLookup19") ItemLookup19


**`POST`** `/ItemLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortCN`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ItemLookupRequestMsg](#item_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Condition": "All",
      "IdType": "ASIN",
      "MerchantId": "MerchantId",
      "ItemId": [
        "ItemId"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ],
      "SearchIndex": "SearchIndex",
      "VariationPage": "VariationPage",
      "RelatedItemPage": "RelatedItemPage",
      "RelationshipType": [
        "RelationshipType"
      ],
      "IncludeReviewsSummary": "IncludeReviewsSummary",
      "TruncateReviewsAt": 68
    },
    "Request": [
      {
        "Condition": "All",
        "IdType": "ASIN",
        "MerchantId": "MerchantId",
        "ItemId": [
          "ItemId"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ],
        "SearchIndex": "SearchIndex",
        "VariationPage": "VariationPage",
        "RelatedItemPage": "RelatedItemPage",
        "RelationshipType": [
          "RelationshipType"
        ],
        "IncludeReviewsSummary": "IncludeReviewsSummary",
        "TruncateReviewsAt": 68
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([ItemLookupResponseMsg](#item_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 68.4806637738276
    },
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 68,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    }
  }
}
```


### <a name="browse_node_lookup20"></a>![Endpoint: ](https://apidocs.io/img/method.png "BrowseNodeLookup20") BrowseNodeLookup20


**`POST`** `/BrowseNodeLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortCN`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [BrowseNodeLookupRequestMsg](#browse_node_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "BrowseNodeId": [
        "BrowseNodeId"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "BrowseNodeId": [
          "BrowseNodeId"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([BrowseNodeLookupResponseMsg](#browse_node_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 68.4806637738276
    },
    "BrowseNodes": [
      {
        "Request": {
          "BrowseNodeLookupRequest": {
            "BrowseNodeId": [
              "BrowseNodeId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "ItemSearchRequest": {
            "Availability": "Available",
            "Actor": "Actor",
            "Artist": "Artist",
            "AudienceRating": [
              "G"
            ],
            "Author": "Author",
            "Brand": "Brand",
            "BrowseNode": "BrowseNode",
            "Composer": "Composer",
            "Condition": "All",
            "Conductor": "Conductor",
            "Director": "Director",
            "ItemPage": 68,
            "Keywords": "Keywords",
            "Manufacturer": "Manufacturer",
            "MaximumPrice": 68,
            "MerchantId": "MerchantId",
            "MinimumPrice": 68,
            "MinPercentageOff": 68,
            "MusicLabel": "MusicLabel",
            "Orchestra": "Orchestra",
            "Power": "Power",
            "Publisher": "Publisher",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "Sort": "Sort",
            "Title": "Title",
            "ReleaseDate": "ReleaseDate",
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 68
          },
          "ItemLookupRequest": {
            "Condition": "All",
            "IdType": "ASIN",
            "MerchantId": "MerchantId",
            "ItemId": [
              "ItemId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "VariationPage": "VariationPage",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 68
          },
          "SimilarityLookupRequest": {
            "Condition": "All",
            "SimilarityType": "Intersection",
            "ItemId": [
              "ItemId"
            ],
            "MerchantId": "MerchantId",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartGetRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartAddRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 68,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartCreateRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 68,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartModifyRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 68,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartClearRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "Errors": {
            "Error": {
              "Code": "Code",
              "Message": "Message"
            }
          },
          "IsValid": "IsValid"
        },
        "BrowseNode": [
          {
            "Properties": {
              "Property": [
                {
                  "Name": "Name",
                  "Value": "Value"
                }
              ]
            },
            "Children": {
              "BrowseNode": []
            },
            "Ancestors": {
              "BrowseNode": []
            },
            "TopSellers": {
              "TopSeller": {
                "ASIN": "ASIN",
                "Title": "Title"
              }
            },
            "NewReleases": {
              "NewRelease": {
                "ASIN": "ASIN",
                "Title": "Title"
              }
            },
            "BrowseNodeId": "BrowseNodeId",
            "Name": "Name",
            "IsCategoryRoot": false,
            "TopItemSet": [
              {
                "TopItem": {
                  "ASIN": "ASIN",
                  "Title": "Title",
                  "DetailPageURL": "DetailPageURL",
                  "ProductGroup": "ProductGroup",
                  "Author": [
                    "Author"
                  ],
                  "Artist": [
                    "Artist"
                  ],
                  "Actor": [
                    "Actor"
                  ]
                },
                "Type": "Type"
              }
            ]
          }
        ]
      }
    ]
  }
}
```


### <a name="similarity_lookup21"></a>![Endpoint: ](https://apidocs.io/img/method.png "SimilarityLookup21") SimilarityLookup21


**`POST`** `/SimilarityLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortCN`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [SimilarityLookupRequestMsg](#similarity_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Condition": "All",
      "SimilarityType": "Intersection",
      "ItemId": [
        "ItemId"
      ],
      "MerchantId": "MerchantId",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Condition": "All",
        "SimilarityType": "Intersection",
        "ItemId": [
          "ItemId"
        ],
        "MerchantId": "MerchantId",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([SimilarityLookupResponseMsg](#similarity_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 159.97594566549
    },
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 159,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    }
  }
}
```


### <a name="cart_get22"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartGet22") CartGet22


**`POST`** `/CartGet`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortCN`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartGetRequestMsg](#cart_get_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartGetResponseMsg](#cart_get_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 159.97594566549
    },
    "Cart": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "URLEncodedHMAC": "URLEncodedHMAC",
        "Request": {
          "BrowseNodeLookupRequest": {
            "BrowseNodeId": [
              "BrowseNodeId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "ItemSearchRequest": {
            "Availability": "Available",
            "Actor": "Actor",
            "Artist": "Artist",
            "AudienceRating": [
              "G"
            ],
            "Author": "Author",
            "Brand": "Brand",
            "BrowseNode": "BrowseNode",
            "Composer": "Composer",
            "Condition": "All",
            "Conductor": "Conductor",
            "Director": "Director",
            "ItemPage": 159,
            "Keywords": "Keywords",
            "Manufacturer": "Manufacturer",
            "MaximumPrice": 159,
            "MerchantId": "MerchantId",
            "MinimumPrice": 159,
            "MinPercentageOff": 159,
            "MusicLabel": "MusicLabel",
            "Orchestra": "Orchestra",
            "Power": "Power",
            "Publisher": "Publisher",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "Sort": "Sort",
            "Title": "Title",
            "ReleaseDate": "ReleaseDate",
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 159
          },
          "ItemLookupRequest": {
            "Condition": "All",
            "IdType": "ASIN",
            "MerchantId": "MerchantId",
            "ItemId": [
              "ItemId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "VariationPage": "VariationPage",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 159
          },
          "SimilarityLookupRequest": {
            "Condition": "All",
            "SimilarityType": "Intersection",
            "ItemId": [
              "ItemId"
            ],
            "MerchantId": "MerchantId",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartGetRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartAddRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 159,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartCreateRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 159,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartModifyRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 159,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartClearRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "Errors": {
            "Error": {
              "Code": "Code",
              "Message": "Message"
            }
          },
          "IsValid": "IsValid"
        },
        "PurchaseURL": "PurchaseURL",
        "MobileCartURL": "MobileCartURL",
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 159,
          "CurrencyCode": "CurrencyCode"
        },
        "CartItems": {
          "CartItem": [
            {
              "CartItemId": "CartItemId",
              "Quantity": "Quantity",
              "MetaData": {
                "KeyValuePair": {
                  "Key": "Key",
                  "Value": "Value"
                }
              },
              "Price": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 159,
                "CurrencyCode": "CurrencyCode"
              },
              "ASIN": "ASIN",
              "SellerNickname": "SellerNickname",
              "Title": "Title",
              "ProductGroup": "ProductGroup",
              "ItemTotal": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 159,
                "CurrencyCode": "CurrencyCode"
              }
            }
          ],
          "SubTotal": {
            "FormattedPrice": "FormattedPrice",
            "Amount": 159,
            "CurrencyCode": "CurrencyCode"
          }
        },
        "SavedForLaterItems": {
          "SavedForLaterItem": [
            {
              "CartItemId": "CartItemId",
              "Quantity": "Quantity",
              "MetaData": {
                "KeyValuePair": {
                  "Key": "Key",
                  "Value": "Value"
                }
              },
              "Price": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 159,
                "CurrencyCode": "CurrencyCode"
              },
              "ASIN": "ASIN",
              "SellerNickname": "SellerNickname",
              "Title": "Title",
              "ProductGroup": "ProductGroup",
              "ItemTotal": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 159,
                "CurrencyCode": "CurrencyCode"
              }
            }
          ],
          "SubTotal": {
            "FormattedPrice": "FormattedPrice",
            "Amount": 159,
            "CurrencyCode": "CurrencyCode"
          }
        },
        "SimilarProducts": {
          "SimilarProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "TopSellers": {
          "TopSeller": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "NewReleases": {
          "NewRelease": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "SimilarViewedProducts": {
          "SimilarViewedProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "OtherCategoriesSimilarProducts": {
          "OtherCategoriesSimilarProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        }
      }
    ]
  }
}
```


### <a name="cart_add23"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartAdd23") CartAdd23


**`POST`** `/CartAdd`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortCN`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartAddRequestMsg](#cart_add_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 251,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 251,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartAddResponseMsg](#cart_add_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 251.471227557152
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 251,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 251,
          "MerchantId": "MerchantId",
          "MinimumPrice": 251,
          "MinPercentageOff": 251,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 251
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 251
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 251,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 251,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 251,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 251,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 251,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 251,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 251,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 251,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 251,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 251,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_create24"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartCreate24") CartCreate24


**`POST`** `/CartCreate`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortCN`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartCreateRequestMsg](#cart_create_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 209,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 209,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartCreateResponseMsg](#cart_create_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 209.748054330586
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 209,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 209,
          "MerchantId": "MerchantId",
          "MinimumPrice": 209,
          "MinPercentageOff": 209,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 209
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 209
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 209,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 209,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 209,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 209,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 209,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 209,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 209,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 209,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 209,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 209,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_modify25"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartModify25") CartModify25


**`POST`** `/CartModify`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortCN`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartModifyRequestMsg](#cart_modify_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 46,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 46,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartModifyResponseMsg](#cart_modify_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 46.2433362222478
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 46,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 46,
          "MerchantId": "MerchantId",
          "MinimumPrice": 46,
          "MinPercentageOff": 46,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 46
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 46
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 46,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 46,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 46,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 46,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 46,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 46,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 46,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 46,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 46,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 46,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_clear26"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartClear26") CartClear26


**`POST`** `/CartClear`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortCN`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartClearRequestMsg](#cart_clear_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartClearResponseMsg](#cart_clear_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 137.73861811391
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 137,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 137,
          "MerchantId": "MerchantId",
          "MinimumPrice": 137,
          "MinPercentageOff": 137,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 137
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 137
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 137,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 137,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 137,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 137,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 137,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 137,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 137,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 137,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 137,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 137,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="item_search27"></a>![Endpoint: ](https://apidocs.io/img/method.png "ItemSearch27") ItemSearch27


**`POST`** `/ItemSearch`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortDE`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ItemSearchRequestMsg](#item_search_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "XMLEscaping": "XMLEscaping",
    "Validate": "Validate",
    "Shared": {
      "Availability": "Available",
      "Actor": "Actor",
      "Artist": "Artist",
      "AudienceRating": [
        "G"
      ],
      "Author": "Author",
      "Brand": "Brand",
      "BrowseNode": "BrowseNode",
      "Composer": "Composer",
      "Condition": "All",
      "Conductor": "Conductor",
      "Director": "Director",
      "ItemPage": 96,
      "Keywords": "Keywords",
      "Manufacturer": "Manufacturer",
      "MaximumPrice": 96,
      "MerchantId": "MerchantId",
      "MinimumPrice": 96,
      "MinPercentageOff": 96,
      "MusicLabel": "MusicLabel",
      "Orchestra": "Orchestra",
      "Power": "Power",
      "Publisher": "Publisher",
      "RelatedItemPage": "RelatedItemPage",
      "RelationshipType": [
        "RelationshipType"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ],
      "SearchIndex": "SearchIndex",
      "Sort": "Sort",
      "Title": "Title",
      "ReleaseDate": "ReleaseDate",
      "IncludeReviewsSummary": "IncludeReviewsSummary",
      "TruncateReviewsAt": 96
    },
    "Request": [
      {
        "Availability": "Available",
        "Actor": "Actor",
        "Artist": "Artist",
        "AudienceRating": [
          "G"
        ],
        "Author": "Author",
        "Brand": "Brand",
        "BrowseNode": "BrowseNode",
        "Composer": "Composer",
        "Condition": "All",
        "Conductor": "Conductor",
        "Director": "Director",
        "ItemPage": 96,
        "Keywords": "Keywords",
        "Manufacturer": "Manufacturer",
        "MaximumPrice": 96,
        "MerchantId": "MerchantId",
        "MinimumPrice": 96,
        "MinPercentageOff": 96,
        "MusicLabel": "MusicLabel",
        "Orchestra": "Orchestra",
        "Power": "Power",
        "Publisher": "Publisher",
        "RelatedItemPage": "RelatedItemPage",
        "RelationshipType": [
          "RelationshipType"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ],
        "SearchIndex": "SearchIndex",
        "Sort": "Sort",
        "Title": "Title",
        "ReleaseDate": "ReleaseDate",
        "IncludeReviewsSummary": "IncludeReviewsSummary",
        "TruncateReviewsAt": 96
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([ItemSearchResponseMsg](#item_search_response_msg)) 
```
{
  "body": {
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 96,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    },
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 96.0154448873435
    }
  }
}
```


### <a name="item_lookup28"></a>![Endpoint: ](https://apidocs.io/img/method.png "ItemLookup28") ItemLookup28


**`POST`** `/ItemLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortDE`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ItemLookupRequestMsg](#item_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Condition": "All",
      "IdType": "ASIN",
      "MerchantId": "MerchantId",
      "ItemId": [
        "ItemId"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ],
      "SearchIndex": "SearchIndex",
      "VariationPage": "VariationPage",
      "RelatedItemPage": "RelatedItemPage",
      "RelationshipType": [
        "RelationshipType"
      ],
      "IncludeReviewsSummary": "IncludeReviewsSummary",
      "TruncateReviewsAt": 96
    },
    "Request": [
      {
        "Condition": "All",
        "IdType": "ASIN",
        "MerchantId": "MerchantId",
        "ItemId": [
          "ItemId"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ],
        "SearchIndex": "SearchIndex",
        "VariationPage": "VariationPage",
        "RelatedItemPage": "RelatedItemPage",
        "RelationshipType": [
          "RelationshipType"
        ],
        "IncludeReviewsSummary": "IncludeReviewsSummary",
        "TruncateReviewsAt": 96
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([ItemLookupResponseMsg](#item_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 96.0154448873435
    },
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 96,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    }
  }
}
```


### <a name="browse_node_lookup29"></a>![Endpoint: ](https://apidocs.io/img/method.png "BrowseNodeLookup29") BrowseNodeLookup29


**`POST`** `/BrowseNodeLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortDE`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [BrowseNodeLookupRequestMsg](#browse_node_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "BrowseNodeId": [
        "BrowseNodeId"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "BrowseNodeId": [
          "BrowseNodeId"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([BrowseNodeLookupResponseMsg](#browse_node_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 96.0154448873435
    },
    "BrowseNodes": [
      {
        "Request": {
          "BrowseNodeLookupRequest": {
            "BrowseNodeId": [
              "BrowseNodeId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "ItemSearchRequest": {
            "Availability": "Available",
            "Actor": "Actor",
            "Artist": "Artist",
            "AudienceRating": [
              "G"
            ],
            "Author": "Author",
            "Brand": "Brand",
            "BrowseNode": "BrowseNode",
            "Composer": "Composer",
            "Condition": "All",
            "Conductor": "Conductor",
            "Director": "Director",
            "ItemPage": 96,
            "Keywords": "Keywords",
            "Manufacturer": "Manufacturer",
            "MaximumPrice": 96,
            "MerchantId": "MerchantId",
            "MinimumPrice": 96,
            "MinPercentageOff": 96,
            "MusicLabel": "MusicLabel",
            "Orchestra": "Orchestra",
            "Power": "Power",
            "Publisher": "Publisher",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "Sort": "Sort",
            "Title": "Title",
            "ReleaseDate": "ReleaseDate",
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 96
          },
          "ItemLookupRequest": {
            "Condition": "All",
            "IdType": "ASIN",
            "MerchantId": "MerchantId",
            "ItemId": [
              "ItemId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "VariationPage": "VariationPage",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 96
          },
          "SimilarityLookupRequest": {
            "Condition": "All",
            "SimilarityType": "Intersection",
            "ItemId": [
              "ItemId"
            ],
            "MerchantId": "MerchantId",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartGetRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartAddRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 96,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartCreateRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 96,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartModifyRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 187,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartClearRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "Errors": {
            "Error": {
              "Code": "Code",
              "Message": "Message"
            }
          },
          "IsValid": "IsValid"
        },
        "BrowseNode": [
          {
            "Properties": {
              "Property": [
                {
                  "Name": "Name",
                  "Value": "Value"
                }
              ]
            },
            "Children": {
              "BrowseNode": []
            },
            "Ancestors": {
              "BrowseNode": []
            },
            "TopSellers": {
              "TopSeller": {
                "ASIN": "ASIN",
                "Title": "Title"
              }
            },
            "NewReleases": {
              "NewRelease": {
                "ASIN": "ASIN",
                "Title": "Title"
              }
            },
            "BrowseNodeId": "BrowseNodeId",
            "Name": "Name",
            "IsCategoryRoot": true,
            "TopItemSet": [
              {
                "TopItem": {
                  "ASIN": "ASIN",
                  "Title": "Title",
                  "DetailPageURL": "DetailPageURL",
                  "ProductGroup": "ProductGroup",
                  "Author": [
                    "Author"
                  ],
                  "Artist": [
                    "Artist"
                  ],
                  "Actor": [
                    "Actor"
                  ]
                },
                "Type": "Type"
              }
            ]
          }
        ]
      }
    ]
  }
}
```


### <a name="similarity_lookup30"></a>![Endpoint: ](https://apidocs.io/img/method.png "SimilarityLookup30") SimilarityLookup30


**`POST`** `/SimilarityLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortDE`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [SimilarityLookupRequestMsg](#similarity_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Condition": "All",
      "SimilarityType": "Intersection",
      "ItemId": [
        "ItemId"
      ],
      "MerchantId": "MerchantId",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Condition": "All",
        "SimilarityType": "Intersection",
        "ItemId": [
          "ItemId"
        ],
        "MerchantId": "MerchantId",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([SimilarityLookupResponseMsg](#similarity_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 187.510726779006
    },
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 187,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    }
  }
}
```


### <a name="cart_get31"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartGet31") CartGet31


**`POST`** `/CartGet`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortDE`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartGetRequestMsg](#cart_get_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartGetResponseMsg](#cart_get_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 187.510726779006
    },
    "Cart": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "URLEncodedHMAC": "URLEncodedHMAC",
        "Request": {
          "BrowseNodeLookupRequest": {
            "BrowseNodeId": [
              "BrowseNodeId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "ItemSearchRequest": {
            "Availability": "Available",
            "Actor": "Actor",
            "Artist": "Artist",
            "AudienceRating": [
              "G"
            ],
            "Author": "Author",
            "Brand": "Brand",
            "BrowseNode": "BrowseNode",
            "Composer": "Composer",
            "Condition": "All",
            "Conductor": "Conductor",
            "Director": "Director",
            "ItemPage": 187,
            "Keywords": "Keywords",
            "Manufacturer": "Manufacturer",
            "MaximumPrice": 187,
            "MerchantId": "MerchantId",
            "MinimumPrice": 187,
            "MinPercentageOff": 187,
            "MusicLabel": "MusicLabel",
            "Orchestra": "Orchestra",
            "Power": "Power",
            "Publisher": "Publisher",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "Sort": "Sort",
            "Title": "Title",
            "ReleaseDate": "ReleaseDate",
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 187
          },
          "ItemLookupRequest": {
            "Condition": "All",
            "IdType": "ASIN",
            "MerchantId": "MerchantId",
            "ItemId": [
              "ItemId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "VariationPage": "VariationPage",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 187
          },
          "SimilarityLookupRequest": {
            "Condition": "All",
            "SimilarityType": "Intersection",
            "ItemId": [
              "ItemId"
            ],
            "MerchantId": "MerchantId",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartGetRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartAddRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 187,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartCreateRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 187,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartModifyRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 187,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartClearRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "Errors": {
            "Error": {
              "Code": "Code",
              "Message": "Message"
            }
          },
          "IsValid": "IsValid"
        },
        "PurchaseURL": "PurchaseURL",
        "MobileCartURL": "MobileCartURL",
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 187,
          "CurrencyCode": "CurrencyCode"
        },
        "CartItems": {
          "CartItem": [
            {
              "CartItemId": "CartItemId",
              "Quantity": "Quantity",
              "MetaData": {
                "KeyValuePair": {
                  "Key": "Key",
                  "Value": "Value"
                }
              },
              "Price": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 187,
                "CurrencyCode": "CurrencyCode"
              },
              "ASIN": "ASIN",
              "SellerNickname": "SellerNickname",
              "Title": "Title",
              "ProductGroup": "ProductGroup",
              "ItemTotal": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 145,
                "CurrencyCode": "CurrencyCode"
              }
            }
          ],
          "SubTotal": {
            "FormattedPrice": "FormattedPrice",
            "Amount": 145,
            "CurrencyCode": "CurrencyCode"
          }
        },
        "SavedForLaterItems": {
          "SavedForLaterItem": [
            {
              "CartItemId": "CartItemId",
              "Quantity": "Quantity",
              "MetaData": {
                "KeyValuePair": {
                  "Key": "Key",
                  "Value": "Value"
                }
              },
              "Price": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 145,
                "CurrencyCode": "CurrencyCode"
              },
              "ASIN": "ASIN",
              "SellerNickname": "SellerNickname",
              "Title": "Title",
              "ProductGroup": "ProductGroup",
              "ItemTotal": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 145,
                "CurrencyCode": "CurrencyCode"
              }
            }
          ],
          "SubTotal": {
            "FormattedPrice": "FormattedPrice",
            "Amount": 145,
            "CurrencyCode": "CurrencyCode"
          }
        },
        "SimilarProducts": {
          "SimilarProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "TopSellers": {
          "TopSeller": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "NewReleases": {
          "NewRelease": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "SimilarViewedProducts": {
          "SimilarViewedProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "OtherCategoriesSimilarProducts": {
          "OtherCategoriesSimilarProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        }
      }
    ]
  }
}
```


### <a name="cart_add32"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartAdd32") CartAdd32


**`POST`** `/CartAdd`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortDE`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartAddRequestMsg](#cart_add_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 145,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 145,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartAddResponseMsg](#cart_add_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 145.787553552439
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 145,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 145,
          "MerchantId": "MerchantId",
          "MinimumPrice": 145,
          "MinPercentageOff": 145,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 145
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 145
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 145,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 145,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 145,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 237,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 237,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 237,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 237,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 237,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 237,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 237,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_create33"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartCreate33") CartCreate33


**`POST`** `/CartCreate`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortDE`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartCreateRequestMsg](#cart_create_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 237,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 237,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartCreateResponseMsg](#cart_create_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 237.282835444102
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 237,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 237,
          "MerchantId": "MerchantId",
          "MinimumPrice": 237,
          "MinPercentageOff": 237,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 237
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 237
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 237,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 237,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 237,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 237,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 73,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 73,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 73,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 73,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 73,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 73,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_modify34"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartModify34") CartModify34


**`POST`** `/CartModify`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortDE`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartModifyRequestMsg](#cart_modify_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 73,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 73,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartModifyResponseMsg](#cart_modify_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 73.7781173357638
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 73,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 73,
          "MerchantId": "MerchantId",
          "MinimumPrice": 73,
          "MinPercentageOff": 73,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 73
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 73
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 73,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 73,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 73,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 32,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 32,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 32,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 32,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 32,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 32,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 32,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_clear35"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartClear35") CartClear35


**`POST`** `/CartClear`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortDE`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartClearRequestMsg](#cart_clear_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartClearResponseMsg](#cart_clear_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 32.0549441091972
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 32,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 32,
          "MerchantId": "MerchantId",
          "MinimumPrice": 32,
          "MinPercentageOff": 32,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 32
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 32
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 32,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 32,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 32,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 123,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 123,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 123,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 123,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 123,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 123,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 123,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="item_search36"></a>![Endpoint: ](https://apidocs.io/img/method.png "ItemSearch36") ItemSearch36


**`POST`** `/ItemSearch`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortES`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ItemSearchRequestMsg](#item_search_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "XMLEscaping": "XMLEscaping",
    "Validate": "Validate",
    "Shared": {
      "Availability": "Available",
      "Actor": "Actor",
      "Artist": "Artist",
      "AudienceRating": [
        "G"
      ],
      "Author": "Author",
      "Brand": "Brand",
      "BrowseNode": "BrowseNode",
      "Composer": "Composer",
      "Condition": "All",
      "Conductor": "Conductor",
      "Director": "Director",
      "ItemPage": 123,
      "Keywords": "Keywords",
      "Manufacturer": "Manufacturer",
      "MaximumPrice": 123,
      "MerchantId": "MerchantId",
      "MinimumPrice": 123,
      "MinPercentageOff": 123,
      "MusicLabel": "MusicLabel",
      "Orchestra": "Orchestra",
      "Power": "Power",
      "Publisher": "Publisher",
      "RelatedItemPage": "RelatedItemPage",
      "RelationshipType": [
        "RelationshipType"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ],
      "SearchIndex": "SearchIndex",
      "Sort": "Sort",
      "Title": "Title",
      "ReleaseDate": "ReleaseDate",
      "IncludeReviewsSummary": "IncludeReviewsSummary",
      "TruncateReviewsAt": 123
    },
    "Request": [
      {
        "Availability": "Available",
        "Actor": "Actor",
        "Artist": "Artist",
        "AudienceRating": [
          "G"
        ],
        "Author": "Author",
        "Brand": "Brand",
        "BrowseNode": "BrowseNode",
        "Composer": "Composer",
        "Condition": "All",
        "Conductor": "Conductor",
        "Director": "Director",
        "ItemPage": 123,
        "Keywords": "Keywords",
        "Manufacturer": "Manufacturer",
        "MaximumPrice": 123,
        "MerchantId": "MerchantId",
        "MinimumPrice": 123,
        "MinPercentageOff": 123,
        "MusicLabel": "MusicLabel",
        "Orchestra": "Orchestra",
        "Power": "Power",
        "Publisher": "Publisher",
        "RelatedItemPage": "RelatedItemPage",
        "RelationshipType": [
          "RelationshipType"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ],
        "SearchIndex": "SearchIndex",
        "Sort": "Sort",
        "Title": "Title",
        "ReleaseDate": "ReleaseDate",
        "IncludeReviewsSummary": "IncludeReviewsSummary",
        "TruncateReviewsAt": 123
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([ItemSearchResponseMsg](#item_search_response_msg)) 
```
{
  "body": {
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 123,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    },
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 123.55022600086
    }
  }
}
```


### <a name="item_lookup37"></a>![Endpoint: ](https://apidocs.io/img/method.png "ItemLookup37") ItemLookup37


**`POST`** `/ItemLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortES`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ItemLookupRequestMsg](#item_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Condition": "All",
      "IdType": "ASIN",
      "MerchantId": "MerchantId",
      "ItemId": [
        "ItemId"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ],
      "SearchIndex": "SearchIndex",
      "VariationPage": "VariationPage",
      "RelatedItemPage": "RelatedItemPage",
      "RelationshipType": [
        "RelationshipType"
      ],
      "IncludeReviewsSummary": "IncludeReviewsSummary",
      "TruncateReviewsAt": 123
    },
    "Request": [
      {
        "Condition": "All",
        "IdType": "ASIN",
        "MerchantId": "MerchantId",
        "ItemId": [
          "ItemId"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ],
        "SearchIndex": "SearchIndex",
        "VariationPage": "VariationPage",
        "RelatedItemPage": "RelatedItemPage",
        "RelationshipType": [
          "RelationshipType"
        ],
        "IncludeReviewsSummary": "IncludeReviewsSummary",
        "TruncateReviewsAt": 123
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([ItemLookupResponseMsg](#item_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 123.55022600086
    },
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 123,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    }
  }
}
```


### <a name="browse_node_lookup38"></a>![Endpoint: ](https://apidocs.io/img/method.png "BrowseNodeLookup38") BrowseNodeLookup38


**`POST`** `/BrowseNodeLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortES`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [BrowseNodeLookupRequestMsg](#browse_node_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "BrowseNodeId": [
        "BrowseNodeId"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "BrowseNodeId": [
          "BrowseNodeId"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([BrowseNodeLookupResponseMsg](#browse_node_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 215.045507892522
    },
    "BrowseNodes": [
      {
        "Request": {
          "BrowseNodeLookupRequest": {
            "BrowseNodeId": [
              "BrowseNodeId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "ItemSearchRequest": {
            "Availability": "Available",
            "Actor": "Actor",
            "Artist": "Artist",
            "AudienceRating": [
              "G"
            ],
            "Author": "Author",
            "Brand": "Brand",
            "BrowseNode": "BrowseNode",
            "Composer": "Composer",
            "Condition": "All",
            "Conductor": "Conductor",
            "Director": "Director",
            "ItemPage": 215,
            "Keywords": "Keywords",
            "Manufacturer": "Manufacturer",
            "MaximumPrice": 215,
            "MerchantId": "MerchantId",
            "MinimumPrice": 215,
            "MinPercentageOff": 215,
            "MusicLabel": "MusicLabel",
            "Orchestra": "Orchestra",
            "Power": "Power",
            "Publisher": "Publisher",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "Sort": "Sort",
            "Title": "Title",
            "ReleaseDate": "ReleaseDate",
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 215
          },
          "ItemLookupRequest": {
            "Condition": "All",
            "IdType": "ASIN",
            "MerchantId": "MerchantId",
            "ItemId": [
              "ItemId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "VariationPage": "VariationPage",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 215
          },
          "SimilarityLookupRequest": {
            "Condition": "All",
            "SimilarityType": "Intersection",
            "ItemId": [
              "ItemId"
            ],
            "MerchantId": "MerchantId",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartGetRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartAddRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 215,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartCreateRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 215,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartModifyRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 215,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartClearRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "Errors": {
            "Error": {
              "Code": "Code",
              "Message": "Message"
            }
          },
          "IsValid": "IsValid"
        },
        "BrowseNode": [
          {
            "Properties": {
              "Property": [
                {
                  "Name": "Name",
                  "Value": "Value"
                }
              ]
            },
            "Children": {
              "BrowseNode": []
            },
            "Ancestors": {
              "BrowseNode": []
            },
            "TopSellers": {
              "TopSeller": {
                "ASIN": "ASIN",
                "Title": "Title"
              }
            },
            "NewReleases": {
              "NewRelease": {
                "ASIN": "ASIN",
                "Title": "Title"
              }
            },
            "BrowseNodeId": "BrowseNodeId",
            "Name": "Name",
            "IsCategoryRoot": true,
            "TopItemSet": [
              {
                "TopItem": {
                  "ASIN": "ASIN",
                  "Title": "Title",
                  "DetailPageURL": "DetailPageURL",
                  "ProductGroup": "ProductGroup",
                  "Author": [
                    "Author"
                  ],
                  "Artist": [
                    "Artist"
                  ],
                  "Actor": [
                    "Actor"
                  ]
                },
                "Type": "Type"
              }
            ]
          }
        ]
      }
    ]
  }
}
```


### <a name="similarity_lookup39"></a>![Endpoint: ](https://apidocs.io/img/method.png "SimilarityLookup39") SimilarityLookup39


**`POST`** `/SimilarityLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortES`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [SimilarityLookupRequestMsg](#similarity_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Condition": "All",
      "SimilarityType": "Intersection",
      "ItemId": [
        "ItemId"
      ],
      "MerchantId": "MerchantId",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Condition": "All",
        "SimilarityType": "Intersection",
        "ItemId": [
          "ItemId"
        ],
        "MerchantId": "MerchantId",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([SimilarityLookupResponseMsg](#similarity_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 215.045507892522
    },
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 215,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    }
  }
}
```


### <a name="cart_get40"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartGet40") CartGet40


**`POST`** `/CartGet`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortES`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartGetRequestMsg](#cart_get_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartGetResponseMsg](#cart_get_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 215.045507892522
    },
    "Cart": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "URLEncodedHMAC": "URLEncodedHMAC",
        "Request": {
          "BrowseNodeLookupRequest": {
            "BrowseNodeId": [
              "BrowseNodeId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "ItemSearchRequest": {
            "Availability": "Available",
            "Actor": "Actor",
            "Artist": "Artist",
            "AudienceRating": [
              "G"
            ],
            "Author": "Author",
            "Brand": "Brand",
            "BrowseNode": "BrowseNode",
            "Composer": "Composer",
            "Condition": "All",
            "Conductor": "Conductor",
            "Director": "Director",
            "ItemPage": 173,
            "Keywords": "Keywords",
            "Manufacturer": "Manufacturer",
            "MaximumPrice": 173,
            "MerchantId": "MerchantId",
            "MinimumPrice": 173,
            "MinPercentageOff": 173,
            "MusicLabel": "MusicLabel",
            "Orchestra": "Orchestra",
            "Power": "Power",
            "Publisher": "Publisher",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "Sort": "Sort",
            "Title": "Title",
            "ReleaseDate": "ReleaseDate",
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 173
          },
          "ItemLookupRequest": {
            "Condition": "All",
            "IdType": "ASIN",
            "MerchantId": "MerchantId",
            "ItemId": [
              "ItemId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "VariationPage": "VariationPage",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 173
          },
          "SimilarityLookupRequest": {
            "Condition": "All",
            "SimilarityType": "Intersection",
            "ItemId": [
              "ItemId"
            ],
            "MerchantId": "MerchantId",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartGetRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartAddRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 173,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartCreateRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 173,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartModifyRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 173,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartClearRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "Errors": {
            "Error": {
              "Code": "Code",
              "Message": "Message"
            }
          },
          "IsValid": "IsValid"
        },
        "PurchaseURL": "PurchaseURL",
        "MobileCartURL": "MobileCartURL",
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 173,
          "CurrencyCode": "CurrencyCode"
        },
        "CartItems": {
          "CartItem": [
            {
              "CartItemId": "CartItemId",
              "Quantity": "Quantity",
              "MetaData": {
                "KeyValuePair": {
                  "Key": "Key",
                  "Value": "Value"
                }
              },
              "Price": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 173,
                "CurrencyCode": "CurrencyCode"
              },
              "ASIN": "ASIN",
              "SellerNickname": "SellerNickname",
              "Title": "Title",
              "ProductGroup": "ProductGroup",
              "ItemTotal": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 173,
                "CurrencyCode": "CurrencyCode"
              }
            }
          ],
          "SubTotal": {
            "FormattedPrice": "FormattedPrice",
            "Amount": 173,
            "CurrencyCode": "CurrencyCode"
          }
        },
        "SavedForLaterItems": {
          "SavedForLaterItem": [
            {
              "CartItemId": "CartItemId",
              "Quantity": "Quantity",
              "MetaData": {
                "KeyValuePair": {
                  "Key": "Key",
                  "Value": "Value"
                }
              },
              "Price": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 173,
                "CurrencyCode": "CurrencyCode"
              },
              "ASIN": "ASIN",
              "SellerNickname": "SellerNickname",
              "Title": "Title",
              "ProductGroup": "ProductGroup",
              "ItemTotal": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 173,
                "CurrencyCode": "CurrencyCode"
              }
            }
          ],
          "SubTotal": {
            "FormattedPrice": "FormattedPrice",
            "Amount": 173,
            "CurrencyCode": "CurrencyCode"
          }
        },
        "SimilarProducts": {
          "SimilarProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "TopSellers": {
          "TopSeller": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "NewReleases": {
          "NewRelease": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "SimilarViewedProducts": {
          "SimilarViewedProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "OtherCategoriesSimilarProducts": {
          "OtherCategoriesSimilarProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        }
      }
    ]
  }
}
```


### <a name="cart_add41"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartAdd41") CartAdd41


**`POST`** `/CartAdd`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortES`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartAddRequestMsg](#cart_add_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 173,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 173,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartAddResponseMsg](#cart_add_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 173.322334665955
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 9,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 9,
          "MerchantId": "MerchantId",
          "MinimumPrice": 9,
          "MinPercentageOff": 9,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 9
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 9
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 9,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 9,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 9,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 9,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 9,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 9,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 9,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 9,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 9,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 9,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_create42"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartCreate42") CartCreate42


**`POST`** `/CartCreate`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortES`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartCreateRequestMsg](#cart_create_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 9,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 9,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartCreateResponseMsg](#cart_create_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 9.81761655761749
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 9,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 9,
          "MerchantId": "MerchantId",
          "MinimumPrice": 9,
          "MinPercentageOff": 9,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 9
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 9
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 223,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 223,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 223,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 223,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 223,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 223,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 223,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 223,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 223,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 223,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_modify43"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartModify43") CartModify43


**`POST`** `/CartModify`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortES`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartModifyRequestMsg](#cart_modify_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 223,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 223,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartModifyResponseMsg](#cart_modify_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 223.094443331051
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 223,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 223,
          "MerchantId": "MerchantId",
          "MinimumPrice": 223,
          "MinPercentageOff": 223,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 223
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 223
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 223,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 59,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 59,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 59,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 59,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 59,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 59,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 59,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 59,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 59,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_clear44"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartClear44") CartClear44


**`POST`** `/CartClear`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortES`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartClearRequestMsg](#cart_clear_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartClearResponseMsg](#cart_clear_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 59.5897252227132
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 59,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 59,
          "MerchantId": "MerchantId",
          "MinimumPrice": 59,
          "MinPercentageOff": 59,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 59
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 59
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 59,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 59,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 151,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 151,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 151,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 151,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 151,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 151,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 151,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 151,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="item_search45"></a>![Endpoint: ](https://apidocs.io/img/method.png "ItemSearch45") ItemSearch45


**`POST`** `/ItemSearch`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortFR`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ItemSearchRequestMsg](#item_search_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "XMLEscaping": "XMLEscaping",
    "Validate": "Validate",
    "Shared": {
      "Availability": "Available",
      "Actor": "Actor",
      "Artist": "Artist",
      "AudienceRating": [
        "G"
      ],
      "Author": "Author",
      "Brand": "Brand",
      "BrowseNode": "BrowseNode",
      "Composer": "Composer",
      "Condition": "All",
      "Conductor": "Conductor",
      "Director": "Director",
      "ItemPage": 151,
      "Keywords": "Keywords",
      "Manufacturer": "Manufacturer",
      "MaximumPrice": 151,
      "MerchantId": "MerchantId",
      "MinimumPrice": 151,
      "MinPercentageOff": 151,
      "MusicLabel": "MusicLabel",
      "Orchestra": "Orchestra",
      "Power": "Power",
      "Publisher": "Publisher",
      "RelatedItemPage": "RelatedItemPage",
      "RelationshipType": [
        "RelationshipType"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ],
      "SearchIndex": "SearchIndex",
      "Sort": "Sort",
      "Title": "Title",
      "ReleaseDate": "ReleaseDate",
      "IncludeReviewsSummary": "IncludeReviewsSummary",
      "TruncateReviewsAt": 151
    },
    "Request": [
      {
        "Availability": "Available",
        "Actor": "Actor",
        "Artist": "Artist",
        "AudienceRating": [
          "G"
        ],
        "Author": "Author",
        "Brand": "Brand",
        "BrowseNode": "BrowseNode",
        "Composer": "Composer",
        "Condition": "All",
        "Conductor": "Conductor",
        "Director": "Director",
        "ItemPage": 151,
        "Keywords": "Keywords",
        "Manufacturer": "Manufacturer",
        "MaximumPrice": 151,
        "MerchantId": "MerchantId",
        "MinimumPrice": 151,
        "MinPercentageOff": 151,
        "MusicLabel": "MusicLabel",
        "Orchestra": "Orchestra",
        "Power": "Power",
        "Publisher": "Publisher",
        "RelatedItemPage": "RelatedItemPage",
        "RelationshipType": [
          "RelationshipType"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ],
        "SearchIndex": "SearchIndex",
        "Sort": "Sort",
        "Title": "Title",
        "ReleaseDate": "ReleaseDate",
        "IncludeReviewsSummary": "IncludeReviewsSummary",
        "TruncateReviewsAt": 151
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([ItemSearchResponseMsg](#item_search_response_msg)) 
```
{
  "body": {
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 151,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    },
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 151.085007114375
    }
  }
}
```


### <a name="item_lookup46"></a>![Endpoint: ](https://apidocs.io/img/method.png "ItemLookup46") ItemLookup46


**`POST`** `/ItemLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortFR`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ItemLookupRequestMsg](#item_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Condition": "All",
      "IdType": "ASIN",
      "MerchantId": "MerchantId",
      "ItemId": [
        "ItemId"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ],
      "SearchIndex": "SearchIndex",
      "VariationPage": "VariationPage",
      "RelatedItemPage": "RelatedItemPage",
      "RelationshipType": [
        "RelationshipType"
      ],
      "IncludeReviewsSummary": "IncludeReviewsSummary",
      "TruncateReviewsAt": 151
    },
    "Request": [
      {
        "Condition": "All",
        "IdType": "ASIN",
        "MerchantId": "MerchantId",
        "ItemId": [
          "ItemId"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ],
        "SearchIndex": "SearchIndex",
        "VariationPage": "VariationPage",
        "RelatedItemPage": "RelatedItemPage",
        "RelationshipType": [
          "RelationshipType"
        ],
        "IncludeReviewsSummary": "IncludeReviewsSummary",
        "TruncateReviewsAt": 151
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([ItemLookupResponseMsg](#item_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 109.361833887809
    },
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 109,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    }
  }
}
```


### <a name="browse_node_lookup47"></a>![Endpoint: ](https://apidocs.io/img/method.png "BrowseNodeLookup47") BrowseNodeLookup47


**`POST`** `/BrowseNodeLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortFR`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [BrowseNodeLookupRequestMsg](#browse_node_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "BrowseNodeId": [
        "BrowseNodeId"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "BrowseNodeId": [
          "BrowseNodeId"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([BrowseNodeLookupResponseMsg](#browse_node_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 109.361833887809
    },
    "BrowseNodes": [
      {
        "Request": {
          "BrowseNodeLookupRequest": {
            "BrowseNodeId": [
              "BrowseNodeId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "ItemSearchRequest": {
            "Availability": "Available",
            "Actor": "Actor",
            "Artist": "Artist",
            "AudienceRating": [
              "G"
            ],
            "Author": "Author",
            "Brand": "Brand",
            "BrowseNode": "BrowseNode",
            "Composer": "Composer",
            "Condition": "All",
            "Conductor": "Conductor",
            "Director": "Director",
            "ItemPage": 109,
            "Keywords": "Keywords",
            "Manufacturer": "Manufacturer",
            "MaximumPrice": 109,
            "MerchantId": "MerchantId",
            "MinimumPrice": 109,
            "MinPercentageOff": 109,
            "MusicLabel": "MusicLabel",
            "Orchestra": "Orchestra",
            "Power": "Power",
            "Publisher": "Publisher",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "Sort": "Sort",
            "Title": "Title",
            "ReleaseDate": "ReleaseDate",
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 109
          },
          "ItemLookupRequest": {
            "Condition": "All",
            "IdType": "ASIN",
            "MerchantId": "MerchantId",
            "ItemId": [
              "ItemId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "VariationPage": "VariationPage",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 109
          },
          "SimilarityLookupRequest": {
            "Condition": "All",
            "SimilarityType": "Intersection",
            "ItemId": [
              "ItemId"
            ],
            "MerchantId": "MerchantId",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartGetRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartAddRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 109,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartCreateRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 109,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartModifyRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 109,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartClearRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "Errors": {
            "Error": {
              "Code": "Code",
              "Message": "Message"
            }
          },
          "IsValid": "IsValid"
        },
        "BrowseNode": [
          {
            "Properties": {
              "Property": [
                {
                  "Name": "Name",
                  "Value": "Value"
                }
              ]
            },
            "Children": {
              "BrowseNode": []
            },
            "Ancestors": {
              "BrowseNode": []
            },
            "TopSellers": {
              "TopSeller": {
                "ASIN": "ASIN",
                "Title": "Title"
              }
            },
            "NewReleases": {
              "NewRelease": {
                "ASIN": "ASIN",
                "Title": "Title"
              }
            },
            "BrowseNodeId": "BrowseNodeId",
            "Name": "Name",
            "IsCategoryRoot": false,
            "TopItemSet": [
              {
                "TopItem": {
                  "ASIN": "ASIN",
                  "Title": "Title",
                  "DetailPageURL": "DetailPageURL",
                  "ProductGroup": "ProductGroup",
                  "Author": [
                    "Author"
                  ],
                  "Artist": [
                    "Artist"
                  ],
                  "Actor": [
                    "Actor"
                  ]
                },
                "Type": "Type"
              }
            ]
          }
        ]
      }
    ]
  }
}
```


### <a name="similarity_lookup48"></a>![Endpoint: ](https://apidocs.io/img/method.png "SimilarityLookup48") SimilarityLookup48


**`POST`** `/SimilarityLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortFR`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [SimilarityLookupRequestMsg](#similarity_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Condition": "All",
      "SimilarityType": "Intersection",
      "ItemId": [
        "ItemId"
      ],
      "MerchantId": "MerchantId",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Condition": "All",
        "SimilarityType": "Intersection",
        "ItemId": [
          "ItemId"
        ],
        "MerchantId": "MerchantId",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([SimilarityLookupResponseMsg](#similarity_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 109.361833887809
    },
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 109,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    }
  }
}
```


### <a name="cart_get49"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartGet49") CartGet49


**`POST`** `/CartGet`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortFR`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartGetRequestMsg](#cart_get_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartGetResponseMsg](#cart_get_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 200.857115779471
    },
    "Cart": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "URLEncodedHMAC": "URLEncodedHMAC",
        "Request": {
          "BrowseNodeLookupRequest": {
            "BrowseNodeId": [
              "BrowseNodeId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "ItemSearchRequest": {
            "Availability": "Available",
            "Actor": "Actor",
            "Artist": "Artist",
            "AudienceRating": [
              "G"
            ],
            "Author": "Author",
            "Brand": "Brand",
            "BrowseNode": "BrowseNode",
            "Composer": "Composer",
            "Condition": "All",
            "Conductor": "Conductor",
            "Director": "Director",
            "ItemPage": 200,
            "Keywords": "Keywords",
            "Manufacturer": "Manufacturer",
            "MaximumPrice": 200,
            "MerchantId": "MerchantId",
            "MinimumPrice": 200,
            "MinPercentageOff": 200,
            "MusicLabel": "MusicLabel",
            "Orchestra": "Orchestra",
            "Power": "Power",
            "Publisher": "Publisher",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "Sort": "Sort",
            "Title": "Title",
            "ReleaseDate": "ReleaseDate",
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 200
          },
          "ItemLookupRequest": {
            "Condition": "All",
            "IdType": "ASIN",
            "MerchantId": "MerchantId",
            "ItemId": [
              "ItemId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "VariationPage": "VariationPage",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 200
          },
          "SimilarityLookupRequest": {
            "Condition": "All",
            "SimilarityType": "Intersection",
            "ItemId": [
              "ItemId"
            ],
            "MerchantId": "MerchantId",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartGetRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartAddRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 200,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartCreateRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 200,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartModifyRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 200,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartClearRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "Errors": {
            "Error": {
              "Code": "Code",
              "Message": "Message"
            }
          },
          "IsValid": "IsValid"
        },
        "PurchaseURL": "PurchaseURL",
        "MobileCartURL": "MobileCartURL",
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 200,
          "CurrencyCode": "CurrencyCode"
        },
        "CartItems": {
          "CartItem": [
            {
              "CartItemId": "CartItemId",
              "Quantity": "Quantity",
              "MetaData": {
                "KeyValuePair": {
                  "Key": "Key",
                  "Value": "Value"
                }
              },
              "Price": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 200,
                "CurrencyCode": "CurrencyCode"
              },
              "ASIN": "ASIN",
              "SellerNickname": "SellerNickname",
              "Title": "Title",
              "ProductGroup": "ProductGroup",
              "ItemTotal": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 200,
                "CurrencyCode": "CurrencyCode"
              }
            }
          ],
          "SubTotal": {
            "FormattedPrice": "FormattedPrice",
            "Amount": 200,
            "CurrencyCode": "CurrencyCode"
          }
        },
        "SavedForLaterItems": {
          "SavedForLaterItem": [
            {
              "CartItemId": "CartItemId",
              "Quantity": "Quantity",
              "MetaData": {
                "KeyValuePair": {
                  "Key": "Key",
                  "Value": "Value"
                }
              },
              "Price": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 200,
                "CurrencyCode": "CurrencyCode"
              },
              "ASIN": "ASIN",
              "SellerNickname": "SellerNickname",
              "Title": "Title",
              "ProductGroup": "ProductGroup",
              "ItemTotal": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 200,
                "CurrencyCode": "CurrencyCode"
              }
            }
          ],
          "SubTotal": {
            "FormattedPrice": "FormattedPrice",
            "Amount": 200,
            "CurrencyCode": "CurrencyCode"
          }
        },
        "SimilarProducts": {
          "SimilarProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "TopSellers": {
          "TopSeller": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "NewReleases": {
          "NewRelease": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "SimilarViewedProducts": {
          "SimilarViewedProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "OtherCategoriesSimilarProducts": {
          "OtherCategoriesSimilarProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        }
      }
    ]
  }
}
```


### <a name="cart_add50"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartAdd50") CartAdd50


**`POST`** `/CartAdd`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortFR`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartAddRequestMsg](#cart_add_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 200,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 200,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartAddResponseMsg](#cart_add_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 37.3523976711335
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 37,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 37,
          "MerchantId": "MerchantId",
          "MinimumPrice": 37,
          "MinPercentageOff": 37,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 37
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 37
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 37,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 37,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 37,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 37,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 37,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 37,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 37,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 37,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 37,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 37,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_create51"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartCreate51") CartCreate51


**`POST`** `/CartCreate`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortFR`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartCreateRequestMsg](#cart_create_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 37,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 37,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartCreateResponseMsg](#cart_create_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 250.629224444567
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 250,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 250,
          "MerchantId": "MerchantId",
          "MinimumPrice": 250,
          "MinPercentageOff": 250,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 250
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 250
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 250,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 250,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 250,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 250,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 250,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 250,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 250,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 250,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 250,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 250,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_modify52"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartModify52") CartModify52


**`POST`** `/CartModify`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortFR`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartModifyRequestMsg](#cart_modify_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 250,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 250,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartModifyResponseMsg](#cart_modify_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 87.1245063362291
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 87,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 87,
          "MerchantId": "MerchantId",
          "MinimumPrice": 87,
          "MinPercentageOff": 87,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 87
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 87
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 87,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 87,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 87,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 87,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 87,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 87,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 87,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 87,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 87,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 87,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_clear53"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartClear53") CartClear53


**`POST`** `/CartClear`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortFR`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartClearRequestMsg](#cart_clear_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartClearResponseMsg](#cart_clear_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 87.1245063362291
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 87,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 87,
          "MerchantId": "MerchantId",
          "MinimumPrice": 87,
          "MinPercentageOff": 87,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 87
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 87
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 45,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 45,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 45,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 45,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 45,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 45,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 45,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 45,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 45,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 45,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="item_search54"></a>![Endpoint: ](https://apidocs.io/img/method.png "ItemSearch54") ItemSearch54


**`POST`** `/ItemSearch`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortIN`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ItemSearchRequestMsg](#item_search_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "XMLEscaping": "XMLEscaping",
    "Validate": "Validate",
    "Shared": {
      "Availability": "Available",
      "Actor": "Actor",
      "Artist": "Artist",
      "AudienceRating": [
        "G"
      ],
      "Author": "Author",
      "Brand": "Brand",
      "BrowseNode": "BrowseNode",
      "Composer": "Composer",
      "Condition": "All",
      "Conductor": "Conductor",
      "Director": "Director",
      "ItemPage": 45,
      "Keywords": "Keywords",
      "Manufacturer": "Manufacturer",
      "MaximumPrice": 45,
      "MerchantId": "MerchantId",
      "MinimumPrice": 45,
      "MinPercentageOff": 45,
      "MusicLabel": "MusicLabel",
      "Orchestra": "Orchestra",
      "Power": "Power",
      "Publisher": "Publisher",
      "RelatedItemPage": "RelatedItemPage",
      "RelationshipType": [
        "RelationshipType"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ],
      "SearchIndex": "SearchIndex",
      "Sort": "Sort",
      "Title": "Title",
      "ReleaseDate": "ReleaseDate",
      "IncludeReviewsSummary": "IncludeReviewsSummary",
      "TruncateReviewsAt": 45
    },
    "Request": [
      {
        "Availability": "Available",
        "Actor": "Actor",
        "Artist": "Artist",
        "AudienceRating": [
          "G"
        ],
        "Author": "Author",
        "Brand": "Brand",
        "BrowseNode": "BrowseNode",
        "Composer": "Composer",
        "Condition": "All",
        "Conductor": "Conductor",
        "Director": "Director",
        "ItemPage": 45,
        "Keywords": "Keywords",
        "Manufacturer": "Manufacturer",
        "MaximumPrice": 45,
        "MerchantId": "MerchantId",
        "MinimumPrice": 45,
        "MinPercentageOff": 45,
        "MusicLabel": "MusicLabel",
        "Orchestra": "Orchestra",
        "Power": "Power",
        "Publisher": "Publisher",
        "RelatedItemPage": "RelatedItemPage",
        "RelationshipType": [
          "RelationshipType"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ],
        "SearchIndex": "SearchIndex",
        "Sort": "Sort",
        "Title": "Title",
        "ReleaseDate": "ReleaseDate",
        "IncludeReviewsSummary": "IncludeReviewsSummary",
        "TruncateReviewsAt": 45
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([ItemSearchResponseMsg](#item_search_response_msg)) 
```
{
  "body": {
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 45,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    },
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 45.4013331096626
    }
  }
}
```


### <a name="item_lookup55"></a>![Endpoint: ](https://apidocs.io/img/method.png "ItemLookup55") ItemLookup55


**`POST`** `/ItemLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortIN`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ItemLookupRequestMsg](#item_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Condition": "All",
      "IdType": "ASIN",
      "MerchantId": "MerchantId",
      "ItemId": [
        "ItemId"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ],
      "SearchIndex": "SearchIndex",
      "VariationPage": "VariationPage",
      "RelatedItemPage": "RelatedItemPage",
      "RelationshipType": [
        "RelationshipType"
      ],
      "IncludeReviewsSummary": "IncludeReviewsSummary",
      "TruncateReviewsAt": 136
    },
    "Request": [
      {
        "Condition": "All",
        "IdType": "ASIN",
        "MerchantId": "MerchantId",
        "ItemId": [
          "ItemId"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ],
        "SearchIndex": "SearchIndex",
        "VariationPage": "VariationPage",
        "RelatedItemPage": "RelatedItemPage",
        "RelationshipType": [
          "RelationshipType"
        ],
        "IncludeReviewsSummary": "IncludeReviewsSummary",
        "TruncateReviewsAt": 136
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([ItemLookupResponseMsg](#item_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 136.896615001325
    },
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 136,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    }
  }
}
```


### <a name="browse_node_lookup56"></a>![Endpoint: ](https://apidocs.io/img/method.png "BrowseNodeLookup56") BrowseNodeLookup56


**`POST`** `/BrowseNodeLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortIN`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [BrowseNodeLookupRequestMsg](#browse_node_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "BrowseNodeId": [
        "BrowseNodeId"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "BrowseNodeId": [
          "BrowseNodeId"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([BrowseNodeLookupResponseMsg](#browse_node_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 136.896615001325
    },
    "BrowseNodes": [
      {
        "Request": {
          "BrowseNodeLookupRequest": {
            "BrowseNodeId": [
              "BrowseNodeId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "ItemSearchRequest": {
            "Availability": "Available",
            "Actor": "Actor",
            "Artist": "Artist",
            "AudienceRating": [
              "G"
            ],
            "Author": "Author",
            "Brand": "Brand",
            "BrowseNode": "BrowseNode",
            "Composer": "Composer",
            "Condition": "All",
            "Conductor": "Conductor",
            "Director": "Director",
            "ItemPage": 136,
            "Keywords": "Keywords",
            "Manufacturer": "Manufacturer",
            "MaximumPrice": 136,
            "MerchantId": "MerchantId",
            "MinimumPrice": 136,
            "MinPercentageOff": 136,
            "MusicLabel": "MusicLabel",
            "Orchestra": "Orchestra",
            "Power": "Power",
            "Publisher": "Publisher",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "Sort": "Sort",
            "Title": "Title",
            "ReleaseDate": "ReleaseDate",
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 136
          },
          "ItemLookupRequest": {
            "Condition": "All",
            "IdType": "ASIN",
            "MerchantId": "MerchantId",
            "ItemId": [
              "ItemId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "VariationPage": "VariationPage",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 136
          },
          "SimilarityLookupRequest": {
            "Condition": "All",
            "SimilarityType": "Intersection",
            "ItemId": [
              "ItemId"
            ],
            "MerchantId": "MerchantId",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartGetRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartAddRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 136,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartCreateRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 136,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartModifyRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 136,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartClearRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "Errors": {
            "Error": {
              "Code": "Code",
              "Message": "Message"
            }
          },
          "IsValid": "IsValid"
        },
        "BrowseNode": [
          {
            "Properties": {
              "Property": [
                {
                  "Name": "Name",
                  "Value": "Value"
                }
              ]
            },
            "Children": {
              "BrowseNode": []
            },
            "Ancestors": {
              "BrowseNode": []
            },
            "TopSellers": {
              "TopSeller": {
                "ASIN": "ASIN",
                "Title": "Title"
              }
            },
            "NewReleases": {
              "NewRelease": {
                "ASIN": "ASIN",
                "Title": "Title"
              }
            },
            "BrowseNodeId": "BrowseNodeId",
            "Name": "Name",
            "IsCategoryRoot": true,
            "TopItemSet": [
              {
                "TopItem": {
                  "ASIN": "ASIN",
                  "Title": "Title",
                  "DetailPageURL": "DetailPageURL",
                  "ProductGroup": "ProductGroup",
                  "Author": [
                    "Author"
                  ],
                  "Artist": [
                    "Artist"
                  ],
                  "Actor": [
                    "Actor"
                  ]
                },
                "Type": "Type"
              }
            ]
          }
        ]
      }
    ]
  }
}
```


### <a name="similarity_lookup57"></a>![Endpoint: ](https://apidocs.io/img/method.png "SimilarityLookup57") SimilarityLookup57


**`POST`** `/SimilarityLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortIN`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [SimilarityLookupRequestMsg](#similarity_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Condition": "All",
      "SimilarityType": "Intersection",
      "ItemId": [
        "ItemId"
      ],
      "MerchantId": "MerchantId",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Condition": "All",
        "SimilarityType": "Intersection",
        "ItemId": [
          "ItemId"
        ],
        "MerchantId": "MerchantId",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([SimilarityLookupResponseMsg](#similarity_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 228.391896892987
    },
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 228,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    }
  }
}
```


### <a name="cart_get58"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartGet58") CartGet58


**`POST`** `/CartGet`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortIN`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartGetRequestMsg](#cart_get_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartGetResponseMsg](#cart_get_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 228.391896892987
    },
    "Cart": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "URLEncodedHMAC": "URLEncodedHMAC",
        "Request": {
          "BrowseNodeLookupRequest": {
            "BrowseNodeId": [
              "BrowseNodeId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "ItemSearchRequest": {
            "Availability": "Available",
            "Actor": "Actor",
            "Artist": "Artist",
            "AudienceRating": [
              "G"
            ],
            "Author": "Author",
            "Brand": "Brand",
            "BrowseNode": "BrowseNode",
            "Composer": "Composer",
            "Condition": "All",
            "Conductor": "Conductor",
            "Director": "Director",
            "ItemPage": 228,
            "Keywords": "Keywords",
            "Manufacturer": "Manufacturer",
            "MaximumPrice": 228,
            "MerchantId": "MerchantId",
            "MinimumPrice": 228,
            "MinPercentageOff": 228,
            "MusicLabel": "MusicLabel",
            "Orchestra": "Orchestra",
            "Power": "Power",
            "Publisher": "Publisher",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "Sort": "Sort",
            "Title": "Title",
            "ReleaseDate": "ReleaseDate",
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 228
          },
          "ItemLookupRequest": {
            "Condition": "All",
            "IdType": "ASIN",
            "MerchantId": "MerchantId",
            "ItemId": [
              "ItemId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "VariationPage": "VariationPage",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 228
          },
          "SimilarityLookupRequest": {
            "Condition": "All",
            "SimilarityType": "Intersection",
            "ItemId": [
              "ItemId"
            ],
            "MerchantId": "MerchantId",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartGetRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartAddRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 228,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartCreateRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 228,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartModifyRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 228,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartClearRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "Errors": {
            "Error": {
              "Code": "Code",
              "Message": "Message"
            }
          },
          "IsValid": "IsValid"
        },
        "PurchaseURL": "PurchaseURL",
        "MobileCartURL": "MobileCartURL",
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 228,
          "CurrencyCode": "CurrencyCode"
        },
        "CartItems": {
          "CartItem": [
            {
              "CartItemId": "CartItemId",
              "Quantity": "Quantity",
              "MetaData": {
                "KeyValuePair": {
                  "Key": "Key",
                  "Value": "Value"
                }
              },
              "Price": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 228,
                "CurrencyCode": "CurrencyCode"
              },
              "ASIN": "ASIN",
              "SellerNickname": "SellerNickname",
              "Title": "Title",
              "ProductGroup": "ProductGroup",
              "ItemTotal": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 228,
                "CurrencyCode": "CurrencyCode"
              }
            }
          ],
          "SubTotal": {
            "FormattedPrice": "FormattedPrice",
            "Amount": 228,
            "CurrencyCode": "CurrencyCode"
          }
        },
        "SavedForLaterItems": {
          "SavedForLaterItem": [
            {
              "CartItemId": "CartItemId",
              "Quantity": "Quantity",
              "MetaData": {
                "KeyValuePair": {
                  "Key": "Key",
                  "Value": "Value"
                }
              },
              "Price": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 228,
                "CurrencyCode": "CurrencyCode"
              },
              "ASIN": "ASIN",
              "SellerNickname": "SellerNickname",
              "Title": "Title",
              "ProductGroup": "ProductGroup",
              "ItemTotal": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 228,
                "CurrencyCode": "CurrencyCode"
              }
            }
          ],
          "SubTotal": {
            "FormattedPrice": "FormattedPrice",
            "Amount": 228,
            "CurrencyCode": "CurrencyCode"
          }
        },
        "SimilarProducts": {
          "SimilarProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "TopSellers": {
          "TopSeller": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "NewReleases": {
          "NewRelease": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "SimilarViewedProducts": {
          "SimilarViewedProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "OtherCategoriesSimilarProducts": {
          "OtherCategoriesSimilarProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        }
      }
    ]
  }
}
```


### <a name="cart_add59"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartAdd59") CartAdd59


**`POST`** `/CartAdd`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortIN`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartAddRequestMsg](#cart_add_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 186,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 186,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartAddResponseMsg](#cart_add_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 186.668723666421
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 186,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 186,
          "MerchantId": "MerchantId",
          "MinimumPrice": 186,
          "MinPercentageOff": 186,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 186
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 186
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 186,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 186,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 186,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 186,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 186,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 186,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 186,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 186,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 186,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 186,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_create60"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartCreate60") CartCreate60


**`POST`** `/CartCreate`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortIN`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartCreateRequestMsg](#cart_create_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 186,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 186,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartCreateResponseMsg](#cart_create_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 23.1640055580828
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 23,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 23,
          "MerchantId": "MerchantId",
          "MinimumPrice": 23,
          "MinPercentageOff": 23,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 23
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 23
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 23,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 23,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 23,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 23,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 23,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 23,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 23,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 23,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 23,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 23,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_modify61"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartModify61") CartModify61


**`POST`** `/CartModify`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortIN`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartModifyRequestMsg](#cart_modify_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 23,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 23,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartModifyResponseMsg](#cart_modify_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 114.659287449745
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 114,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 114,
          "MerchantId": "MerchantId",
          "MinimumPrice": 114,
          "MinPercentageOff": 114,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 114
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 114
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 114,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 114,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 114,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 114,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 114,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 114,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 114,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 114,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 114,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 114,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_clear62"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartClear62") CartClear62


**`POST`** `/CartClear`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortIN`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartClearRequestMsg](#cart_clear_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartClearResponseMsg](#cart_clear_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 114.659287449745
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 72,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 72,
          "MerchantId": "MerchantId",
          "MinimumPrice": 72,
          "MinPercentageOff": 72,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 72
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 72
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 72,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 72,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 72,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 72,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 72,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 72,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 72,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 72,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 72,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 72,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="item_search63"></a>![Endpoint: ](https://apidocs.io/img/method.png "ItemSearch63") ItemSearch63


**`POST`** `/ItemSearch`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortIT`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ItemSearchRequestMsg](#item_search_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "XMLEscaping": "XMLEscaping",
    "Validate": "Validate",
    "Shared": {
      "Availability": "Available",
      "Actor": "Actor",
      "Artist": "Artist",
      "AudienceRating": [
        "G"
      ],
      "Author": "Author",
      "Brand": "Brand",
      "BrowseNode": "BrowseNode",
      "Composer": "Composer",
      "Condition": "All",
      "Conductor": "Conductor",
      "Director": "Director",
      "ItemPage": 72,
      "Keywords": "Keywords",
      "Manufacturer": "Manufacturer",
      "MaximumPrice": 72,
      "MerchantId": "MerchantId",
      "MinimumPrice": 72,
      "MinPercentageOff": 72,
      "MusicLabel": "MusicLabel",
      "Orchestra": "Orchestra",
      "Power": "Power",
      "Publisher": "Publisher",
      "RelatedItemPage": "RelatedItemPage",
      "RelationshipType": [
        "RelationshipType"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ],
      "SearchIndex": "SearchIndex",
      "Sort": "Sort",
      "Title": "Title",
      "ReleaseDate": "ReleaseDate",
      "IncludeReviewsSummary": "IncludeReviewsSummary",
      "TruncateReviewsAt": 72
    },
    "Request": [
      {
        "Availability": "Available",
        "Actor": "Actor",
        "Artist": "Artist",
        "AudienceRating": [
          "G"
        ],
        "Author": "Author",
        "Brand": "Brand",
        "BrowseNode": "BrowseNode",
        "Composer": "Composer",
        "Condition": "All",
        "Conductor": "Conductor",
        "Director": "Director",
        "ItemPage": 72,
        "Keywords": "Keywords",
        "Manufacturer": "Manufacturer",
        "MaximumPrice": 72,
        "MerchantId": "MerchantId",
        "MinimumPrice": 72,
        "MinPercentageOff": 72,
        "MusicLabel": "MusicLabel",
        "Orchestra": "Orchestra",
        "Power": "Power",
        "Publisher": "Publisher",
        "RelatedItemPage": "RelatedItemPage",
        "RelationshipType": [
          "RelationshipType"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ],
        "SearchIndex": "SearchIndex",
        "Sort": "Sort",
        "Title": "Title",
        "ReleaseDate": "ReleaseDate",
        "IncludeReviewsSummary": "IncludeReviewsSummary",
        "TruncateReviewsAt": 72
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([ItemSearchResponseMsg](#item_search_response_msg)) 
```
{
  "body": {
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 72,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    },
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 164.431396114841
    }
  }
}
```


### <a name="item_lookup64"></a>![Endpoint: ](https://apidocs.io/img/method.png "ItemLookup64") ItemLookup64


**`POST`** `/ItemLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortIT`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ItemLookupRequestMsg](#item_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Condition": "All",
      "IdType": "ASIN",
      "MerchantId": "MerchantId",
      "ItemId": [
        "ItemId"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ],
      "SearchIndex": "SearchIndex",
      "VariationPage": "VariationPage",
      "RelatedItemPage": "RelatedItemPage",
      "RelationshipType": [
        "RelationshipType"
      ],
      "IncludeReviewsSummary": "IncludeReviewsSummary",
      "TruncateReviewsAt": 164
    },
    "Request": [
      {
        "Condition": "All",
        "IdType": "ASIN",
        "MerchantId": "MerchantId",
        "ItemId": [
          "ItemId"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ],
        "SearchIndex": "SearchIndex",
        "VariationPage": "VariationPage",
        "RelatedItemPage": "RelatedItemPage",
        "RelationshipType": [
          "RelationshipType"
        ],
        "IncludeReviewsSummary": "IncludeReviewsSummary",
        "TruncateReviewsAt": 164
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([ItemLookupResponseMsg](#item_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 164.431396114841
    },
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 164,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    }
  }
}
```


### <a name="browse_node_lookup65"></a>![Endpoint: ](https://apidocs.io/img/method.png "BrowseNodeLookup65") BrowseNodeLookup65


**`POST`** `/BrowseNodeLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortIT`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [BrowseNodeLookupRequestMsg](#browse_node_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "BrowseNodeId": [
        "BrowseNodeId"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "BrowseNodeId": [
          "BrowseNodeId"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([BrowseNodeLookupResponseMsg](#browse_node_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 164.431396114841
    },
    "BrowseNodes": [
      {
        "Request": {
          "BrowseNodeLookupRequest": {
            "BrowseNodeId": [
              "BrowseNodeId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "ItemSearchRequest": {
            "Availability": "Available",
            "Actor": "Actor",
            "Artist": "Artist",
            "AudienceRating": [
              "G"
            ],
            "Author": "Author",
            "Brand": "Brand",
            "BrowseNode": "BrowseNode",
            "Composer": "Composer",
            "Condition": "All",
            "Conductor": "Conductor",
            "Director": "Director",
            "ItemPage": 164,
            "Keywords": "Keywords",
            "Manufacturer": "Manufacturer",
            "MaximumPrice": 164,
            "MerchantId": "MerchantId",
            "MinimumPrice": 164,
            "MinPercentageOff": 164,
            "MusicLabel": "MusicLabel",
            "Orchestra": "Orchestra",
            "Power": "Power",
            "Publisher": "Publisher",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "Sort": "Sort",
            "Title": "Title",
            "ReleaseDate": "ReleaseDate",
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 164
          },
          "ItemLookupRequest": {
            "Condition": "All",
            "IdType": "ASIN",
            "MerchantId": "MerchantId",
            "ItemId": [
              "ItemId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "VariationPage": "VariationPage",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 164
          },
          "SimilarityLookupRequest": {
            "Condition": "All",
            "SimilarityType": "Intersection",
            "ItemId": [
              "ItemId"
            ],
            "MerchantId": "MerchantId",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartGetRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartAddRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 164,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartCreateRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 164,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartModifyRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 164,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartClearRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "Errors": {
            "Error": {
              "Code": "Code",
              "Message": "Message"
            }
          },
          "IsValid": "IsValid"
        },
        "BrowseNode": [
          {
            "Properties": {
              "Property": [
                {
                  "Name": "Name",
                  "Value": "Value"
                }
              ]
            },
            "Children": {
              "BrowseNode": []
            },
            "Ancestors": {
              "BrowseNode": []
            },
            "TopSellers": {
              "TopSeller": {
                "ASIN": "ASIN",
                "Title": "Title"
              }
            },
            "NewReleases": {
              "NewRelease": {
                "ASIN": "ASIN",
                "Title": "Title"
              }
            },
            "BrowseNodeId": "BrowseNodeId",
            "Name": "Name",
            "IsCategoryRoot": true,
            "TopItemSet": [
              {
                "TopItem": {
                  "ASIN": "ASIN",
                  "Title": "Title",
                  "DetailPageURL": "DetailPageURL",
                  "ProductGroup": "ProductGroup",
                  "Author": [
                    "Author"
                  ],
                  "Artist": [
                    "Artist"
                  ],
                  "Actor": [
                    "Actor"
                  ]
                },
                "Type": "Type"
              }
            ]
          }
        ]
      }
    ]
  }
}
```


### <a name="similarity_lookup66"></a>![Endpoint: ](https://apidocs.io/img/method.png "SimilarityLookup66") SimilarityLookup66


**`POST`** `/SimilarityLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortIT`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [SimilarityLookupRequestMsg](#similarity_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Condition": "All",
      "SimilarityType": "Intersection",
      "ItemId": [
        "ItemId"
      ],
      "MerchantId": "MerchantId",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Condition": "All",
        "SimilarityType": "Intersection",
        "ItemId": [
          "ItemId"
        ],
        "MerchantId": "MerchantId",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([SimilarityLookupResponseMsg](#similarity_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 122.708222888274
    },
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 122,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    }
  }
}
```


### <a name="cart_get67"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartGet67") CartGet67


**`POST`** `/CartGet`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortIT`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartGetRequestMsg](#cart_get_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartGetResponseMsg](#cart_get_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 122.708222888274
    },
    "Cart": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "URLEncodedHMAC": "URLEncodedHMAC",
        "Request": {
          "BrowseNodeLookupRequest": {
            "BrowseNodeId": [
              "BrowseNodeId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "ItemSearchRequest": {
            "Availability": "Available",
            "Actor": "Actor",
            "Artist": "Artist",
            "AudienceRating": [
              "G"
            ],
            "Author": "Author",
            "Brand": "Brand",
            "BrowseNode": "BrowseNode",
            "Composer": "Composer",
            "Condition": "All",
            "Conductor": "Conductor",
            "Director": "Director",
            "ItemPage": 122,
            "Keywords": "Keywords",
            "Manufacturer": "Manufacturer",
            "MaximumPrice": 122,
            "MerchantId": "MerchantId",
            "MinimumPrice": 122,
            "MinPercentageOff": 122,
            "MusicLabel": "MusicLabel",
            "Orchestra": "Orchestra",
            "Power": "Power",
            "Publisher": "Publisher",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "Sort": "Sort",
            "Title": "Title",
            "ReleaseDate": "ReleaseDate",
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 122
          },
          "ItemLookupRequest": {
            "Condition": "All",
            "IdType": "ASIN",
            "MerchantId": "MerchantId",
            "ItemId": [
              "ItemId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "VariationPage": "VariationPage",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 122
          },
          "SimilarityLookupRequest": {
            "Condition": "All",
            "SimilarityType": "Intersection",
            "ItemId": [
              "ItemId"
            ],
            "MerchantId": "MerchantId",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartGetRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartAddRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 122,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartCreateRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 122,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartModifyRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 122,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartClearRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "Errors": {
            "Error": {
              "Code": "Code",
              "Message": "Message"
            }
          },
          "IsValid": "IsValid"
        },
        "PurchaseURL": "PurchaseURL",
        "MobileCartURL": "MobileCartURL",
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 122,
          "CurrencyCode": "CurrencyCode"
        },
        "CartItems": {
          "CartItem": [
            {
              "CartItemId": "CartItemId",
              "Quantity": "Quantity",
              "MetaData": {
                "KeyValuePair": {
                  "Key": "Key",
                  "Value": "Value"
                }
              },
              "Price": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 122,
                "CurrencyCode": "CurrencyCode"
              },
              "ASIN": "ASIN",
              "SellerNickname": "SellerNickname",
              "Title": "Title",
              "ProductGroup": "ProductGroup",
              "ItemTotal": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 122,
                "CurrencyCode": "CurrencyCode"
              }
            }
          ],
          "SubTotal": {
            "FormattedPrice": "FormattedPrice",
            "Amount": 122,
            "CurrencyCode": "CurrencyCode"
          }
        },
        "SavedForLaterItems": {
          "SavedForLaterItem": [
            {
              "CartItemId": "CartItemId",
              "Quantity": "Quantity",
              "MetaData": {
                "KeyValuePair": {
                  "Key": "Key",
                  "Value": "Value"
                }
              },
              "Price": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 122,
                "CurrencyCode": "CurrencyCode"
              },
              "ASIN": "ASIN",
              "SellerNickname": "SellerNickname",
              "Title": "Title",
              "ProductGroup": "ProductGroup",
              "ItemTotal": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 122,
                "CurrencyCode": "CurrencyCode"
              }
            }
          ],
          "SubTotal": {
            "FormattedPrice": "FormattedPrice",
            "Amount": 122,
            "CurrencyCode": "CurrencyCode"
          }
        },
        "SimilarProducts": {
          "SimilarProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "TopSellers": {
          "TopSeller": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "NewReleases": {
          "NewRelease": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "SimilarViewedProducts": {
          "SimilarViewedProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "OtherCategoriesSimilarProducts": {
          "OtherCategoriesSimilarProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        }
      }
    ]
  }
}
```


### <a name="cart_add68"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartAdd68") CartAdd68


**`POST`** `/CartAdd`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortIT`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartAddRequestMsg](#cart_add_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 214,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 214,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartAddResponseMsg](#cart_add_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 214.203504779937
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 214,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 214,
          "MerchantId": "MerchantId",
          "MinimumPrice": 214,
          "MinPercentageOff": 214,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 214
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 214
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 214,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 214,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 214,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 214,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 214,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 214,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 214,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 214,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 214,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 214,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_create69"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartCreate69") CartCreate69


**`POST`** `/CartCreate`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortIT`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartCreateRequestMsg](#cart_create_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 50,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 50,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartCreateResponseMsg](#cart_create_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 50.6987866715988
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 50,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 50,
          "MerchantId": "MerchantId",
          "MinimumPrice": 50,
          "MinPercentageOff": 50,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 50
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 50
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 50,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 50,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 50,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 50,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 50,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 50,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 50,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 50,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 50,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 50,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_modify70"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartModify70") CartModify70


**`POST`** `/CartModify`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortIT`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartModifyRequestMsg](#cart_modify_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 8,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 8,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartModifyResponseMsg](#cart_modify_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 8.97561344503221
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 8,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 8,
          "MerchantId": "MerchantId",
          "MinimumPrice": 8,
          "MinPercentageOff": 8,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 8
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 8
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 8,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 8,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 8,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 8,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 8,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 8,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 8,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 8,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 8,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 8,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_clear71"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartClear71") CartClear71


**`POST`** `/CartClear`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortIT`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartClearRequestMsg](#cart_clear_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartClearResponseMsg](#cart_clear_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 100.470895336694
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 100,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 100,
          "MerchantId": "MerchantId",
          "MinimumPrice": 100,
          "MinPercentageOff": 100,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 100
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 100
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 100,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 100,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 100,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 100,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 100,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 100,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 100,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 100,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 100,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 100,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="item_search72"></a>![Endpoint: ](https://apidocs.io/img/method.png "ItemSearch72") ItemSearch72


**`POST`** `/ItemSearch`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortJP`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ItemSearchRequestMsg](#item_search_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "XMLEscaping": "XMLEscaping",
    "Validate": "Validate",
    "Shared": {
      "Availability": "Available",
      "Actor": "Actor",
      "Artist": "Artist",
      "AudienceRating": [
        "G"
      ],
      "Author": "Author",
      "Brand": "Brand",
      "BrowseNode": "BrowseNode",
      "Composer": "Composer",
      "Condition": "All",
      "Conductor": "Conductor",
      "Director": "Director",
      "ItemPage": 100,
      "Keywords": "Keywords",
      "Manufacturer": "Manufacturer",
      "MaximumPrice": 100,
      "MerchantId": "MerchantId",
      "MinimumPrice": 100,
      "MinPercentageOff": 100,
      "MusicLabel": "MusicLabel",
      "Orchestra": "Orchestra",
      "Power": "Power",
      "Publisher": "Publisher",
      "RelatedItemPage": "RelatedItemPage",
      "RelationshipType": [
        "RelationshipType"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ],
      "SearchIndex": "SearchIndex",
      "Sort": "Sort",
      "Title": "Title",
      "ReleaseDate": "ReleaseDate",
      "IncludeReviewsSummary": "IncludeReviewsSummary",
      "TruncateReviewsAt": 100
    },
    "Request": [
      {
        "Availability": "Available",
        "Actor": "Actor",
        "Artist": "Artist",
        "AudienceRating": [
          "G"
        ],
        "Author": "Author",
        "Brand": "Brand",
        "BrowseNode": "BrowseNode",
        "Composer": "Composer",
        "Condition": "All",
        "Conductor": "Conductor",
        "Director": "Director",
        "ItemPage": 100,
        "Keywords": "Keywords",
        "Manufacturer": "Manufacturer",
        "MaximumPrice": 100,
        "MerchantId": "MerchantId",
        "MinimumPrice": 100,
        "MinPercentageOff": 100,
        "MusicLabel": "MusicLabel",
        "Orchestra": "Orchestra",
        "Power": "Power",
        "Publisher": "Publisher",
        "RelatedItemPage": "RelatedItemPage",
        "RelationshipType": [
          "RelationshipType"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ],
        "SearchIndex": "SearchIndex",
        "Sort": "Sort",
        "Title": "Title",
        "ReleaseDate": "ReleaseDate",
        "IncludeReviewsSummary": "IncludeReviewsSummary",
        "TruncateReviewsAt": 191
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([ItemSearchResponseMsg](#item_search_response_msg)) 
```
{
  "body": {
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 191,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    },
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 191.966177228357
    }
  }
}
```


### <a name="item_lookup73"></a>![Endpoint: ](https://apidocs.io/img/method.png "ItemLookup73") ItemLookup73


**`POST`** `/ItemLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortJP`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ItemLookupRequestMsg](#item_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Condition": "All",
      "IdType": "ASIN",
      "MerchantId": "MerchantId",
      "ItemId": [
        "ItemId"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ],
      "SearchIndex": "SearchIndex",
      "VariationPage": "VariationPage",
      "RelatedItemPage": "RelatedItemPage",
      "RelationshipType": [
        "RelationshipType"
      ],
      "IncludeReviewsSummary": "IncludeReviewsSummary",
      "TruncateReviewsAt": 191
    },
    "Request": [
      {
        "Condition": "All",
        "IdType": "ASIN",
        "MerchantId": "MerchantId",
        "ItemId": [
          "ItemId"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ],
        "SearchIndex": "SearchIndex",
        "VariationPage": "VariationPage",
        "RelatedItemPage": "RelatedItemPage",
        "RelationshipType": [
          "RelationshipType"
        ],
        "IncludeReviewsSummary": "IncludeReviewsSummary",
        "TruncateReviewsAt": 191
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([ItemLookupResponseMsg](#item_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 191.966177228357
    },
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 191,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    }
  }
}
```


### <a name="browse_node_lookup74"></a>![Endpoint: ](https://apidocs.io/img/method.png "BrowseNodeLookup74") BrowseNodeLookup74


**`POST`** `/BrowseNodeLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortJP`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [BrowseNodeLookupRequestMsg](#browse_node_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "BrowseNodeId": [
        "BrowseNodeId"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "BrowseNodeId": [
          "BrowseNodeId"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([BrowseNodeLookupResponseMsg](#browse_node_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 191.966177228357
    },
    "BrowseNodes": [
      {
        "Request": {
          "BrowseNodeLookupRequest": {
            "BrowseNodeId": [
              "BrowseNodeId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "ItemSearchRequest": {
            "Availability": "Available",
            "Actor": "Actor",
            "Artist": "Artist",
            "AudienceRating": [
              "G"
            ],
            "Author": "Author",
            "Brand": "Brand",
            "BrowseNode": "BrowseNode",
            "Composer": "Composer",
            "Condition": "All",
            "Conductor": "Conductor",
            "Director": "Director",
            "ItemPage": 191,
            "Keywords": "Keywords",
            "Manufacturer": "Manufacturer",
            "MaximumPrice": 191,
            "MerchantId": "MerchantId",
            "MinimumPrice": 191,
            "MinPercentageOff": 191,
            "MusicLabel": "MusicLabel",
            "Orchestra": "Orchestra",
            "Power": "Power",
            "Publisher": "Publisher",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "Sort": "Sort",
            "Title": "Title",
            "ReleaseDate": "ReleaseDate",
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 191
          },
          "ItemLookupRequest": {
            "Condition": "All",
            "IdType": "ASIN",
            "MerchantId": "MerchantId",
            "ItemId": [
              "ItemId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "VariationPage": "VariationPage",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 191
          },
          "SimilarityLookupRequest": {
            "Condition": "All",
            "SimilarityType": "Intersection",
            "ItemId": [
              "ItemId"
            ],
            "MerchantId": "MerchantId",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartGetRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartAddRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 191,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartCreateRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 191,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartModifyRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 191,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartClearRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "Errors": {
            "Error": {
              "Code": "Code",
              "Message": "Message"
            }
          },
          "IsValid": "IsValid"
        },
        "BrowseNode": [
          {
            "Properties": {
              "Property": [
                {
                  "Name": "Name",
                  "Value": "Value"
                }
              ]
            },
            "Children": {
              "BrowseNode": []
            },
            "Ancestors": {
              "BrowseNode": []
            },
            "TopSellers": {
              "TopSeller": {
                "ASIN": "ASIN",
                "Title": "Title"
              }
            },
            "NewReleases": {
              "NewRelease": {
                "ASIN": "ASIN",
                "Title": "Title"
              }
            },
            "BrowseNodeId": "BrowseNodeId",
            "Name": "Name",
            "IsCategoryRoot": true,
            "TopItemSet": [
              {
                "TopItem": {
                  "ASIN": "ASIN",
                  "Title": "Title",
                  "DetailPageURL": "DetailPageURL",
                  "ProductGroup": "ProductGroup",
                  "Author": [
                    "Author"
                  ],
                  "Artist": [
                    "Artist"
                  ],
                  "Actor": [
                    "Actor"
                  ]
                },
                "Type": "Type"
              }
            ]
          }
        ]
      }
    ]
  }
}
```


### <a name="similarity_lookup75"></a>![Endpoint: ](https://apidocs.io/img/method.png "SimilarityLookup75") SimilarityLookup75


**`POST`** `/SimilarityLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortJP`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [SimilarityLookupRequestMsg](#similarity_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Condition": "All",
      "SimilarityType": "Intersection",
      "ItemId": [
        "ItemId"
      ],
      "MerchantId": "MerchantId",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Condition": "All",
        "SimilarityType": "Intersection",
        "ItemId": [
          "ItemId"
        ],
        "MerchantId": "MerchantId",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([SimilarityLookupResponseMsg](#similarity_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 150.24300400179
    },
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 150,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    }
  }
}
```


### <a name="cart_get76"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartGet76") CartGet76


**`POST`** `/CartGet`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortJP`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartGetRequestMsg](#cart_get_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartGetResponseMsg](#cart_get_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 150.24300400179
    },
    "Cart": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "URLEncodedHMAC": "URLEncodedHMAC",
        "Request": {
          "BrowseNodeLookupRequest": {
            "BrowseNodeId": [
              "BrowseNodeId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "ItemSearchRequest": {
            "Availability": "Available",
            "Actor": "Actor",
            "Artist": "Artist",
            "AudienceRating": [
              "G"
            ],
            "Author": "Author",
            "Brand": "Brand",
            "BrowseNode": "BrowseNode",
            "Composer": "Composer",
            "Condition": "All",
            "Conductor": "Conductor",
            "Director": "Director",
            "ItemPage": 150,
            "Keywords": "Keywords",
            "Manufacturer": "Manufacturer",
            "MaximumPrice": 150,
            "MerchantId": "MerchantId",
            "MinimumPrice": 150,
            "MinPercentageOff": 150,
            "MusicLabel": "MusicLabel",
            "Orchestra": "Orchestra",
            "Power": "Power",
            "Publisher": "Publisher",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "Sort": "Sort",
            "Title": "Title",
            "ReleaseDate": "ReleaseDate",
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 150
          },
          "ItemLookupRequest": {
            "Condition": "All",
            "IdType": "ASIN",
            "MerchantId": "MerchantId",
            "ItemId": [
              "ItemId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "VariationPage": "VariationPage",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 150
          },
          "SimilarityLookupRequest": {
            "Condition": "All",
            "SimilarityType": "Intersection",
            "ItemId": [
              "ItemId"
            ],
            "MerchantId": "MerchantId",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartGetRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartAddRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 150,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartCreateRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 150,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartModifyRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 150,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartClearRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "Errors": {
            "Error": {
              "Code": "Code",
              "Message": "Message"
            }
          },
          "IsValid": "IsValid"
        },
        "PurchaseURL": "PurchaseURL",
        "MobileCartURL": "MobileCartURL",
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 150,
          "CurrencyCode": "CurrencyCode"
        },
        "CartItems": {
          "CartItem": [
            {
              "CartItemId": "CartItemId",
              "Quantity": "Quantity",
              "MetaData": {
                "KeyValuePair": {
                  "Key": "Key",
                  "Value": "Value"
                }
              },
              "Price": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 150,
                "CurrencyCode": "CurrencyCode"
              },
              "ASIN": "ASIN",
              "SellerNickname": "SellerNickname",
              "Title": "Title",
              "ProductGroup": "ProductGroup",
              "ItemTotal": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 150,
                "CurrencyCode": "CurrencyCode"
              }
            }
          ],
          "SubTotal": {
            "FormattedPrice": "FormattedPrice",
            "Amount": 150,
            "CurrencyCode": "CurrencyCode"
          }
        },
        "SavedForLaterItems": {
          "SavedForLaterItem": [
            {
              "CartItemId": "CartItemId",
              "Quantity": "Quantity",
              "MetaData": {
                "KeyValuePair": {
                  "Key": "Key",
                  "Value": "Value"
                }
              },
              "Price": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 150,
                "CurrencyCode": "CurrencyCode"
              },
              "ASIN": "ASIN",
              "SellerNickname": "SellerNickname",
              "Title": "Title",
              "ProductGroup": "ProductGroup",
              "ItemTotal": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 150,
                "CurrencyCode": "CurrencyCode"
              }
            }
          ],
          "SubTotal": {
            "FormattedPrice": "FormattedPrice",
            "Amount": 150,
            "CurrencyCode": "CurrencyCode"
          }
        },
        "SimilarProducts": {
          "SimilarProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "TopSellers": {
          "TopSeller": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "NewReleases": {
          "NewRelease": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "SimilarViewedProducts": {
          "SimilarViewedProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "OtherCategoriesSimilarProducts": {
          "OtherCategoriesSimilarProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        }
      }
    ]
  }
}
```


### <a name="cart_add77"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartAdd77") CartAdd77


**`POST`** `/CartAdd`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortJP`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartAddRequestMsg](#cart_add_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 241,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 241,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartAddResponseMsg](#cart_add_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 241.738285893452
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 241,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 241,
          "MerchantId": "MerchantId",
          "MinimumPrice": 241,
          "MinPercentageOff": 241,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 241
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 241
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 241,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 241,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 241,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 241,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 241,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 241,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 241,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 241,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 241,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 241,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_create78"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartCreate78") CartCreate78


**`POST`** `/CartCreate`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortJP`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartCreateRequestMsg](#cart_create_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 200,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 200,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartCreateResponseMsg](#cart_create_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 200.015112666886
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 200,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 200,
          "MerchantId": "MerchantId",
          "MinimumPrice": 200,
          "MinPercentageOff": 200,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 200
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 200
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 200,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 200,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 200,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 200,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 200,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 200,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 200,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 200,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 200,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 200,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_modify79"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartModify79") CartModify79


**`POST`** `/CartModify`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortJP`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartModifyRequestMsg](#cart_modify_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 36,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 36,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartModifyResponseMsg](#cart_modify_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 36.5103945585482
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 36,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 36,
          "MerchantId": "MerchantId",
          "MinimumPrice": 36,
          "MinPercentageOff": 36,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 36
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 36
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 36,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 36,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 36,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 36,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 36,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 36,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 36,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 36,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 36,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 36,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_clear80"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartClear80") CartClear80


**`POST`** `/CartClear`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortJP`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartClearRequestMsg](#cart_clear_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartClearResponseMsg](#cart_clear_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 128.00567645021
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 128,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 128,
          "MerchantId": "MerchantId",
          "MinimumPrice": 128,
          "MinPercentageOff": 128,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 128
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 128
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 128,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 128,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 128,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 128,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 128,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 128,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 128,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 128,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 128,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 128,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="item_search81"></a>![Endpoint: ](https://apidocs.io/img/method.png "ItemSearch81") ItemSearch81


**`POST`** `/ItemSearch`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortUK`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ItemSearchRequestMsg](#item_search_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "XMLEscaping": "XMLEscaping",
    "Validate": "Validate",
    "Shared": {
      "Availability": "Available",
      "Actor": "Actor",
      "Artist": "Artist",
      "AudienceRating": [
        "G"
      ],
      "Author": "Author",
      "Brand": "Brand",
      "BrowseNode": "BrowseNode",
      "Composer": "Composer",
      "Condition": "All",
      "Conductor": "Conductor",
      "Director": "Director",
      "ItemPage": 86,
      "Keywords": "Keywords",
      "Manufacturer": "Manufacturer",
      "MaximumPrice": 86,
      "MerchantId": "MerchantId",
      "MinimumPrice": 86,
      "MinPercentageOff": 86,
      "MusicLabel": "MusicLabel",
      "Orchestra": "Orchestra",
      "Power": "Power",
      "Publisher": "Publisher",
      "RelatedItemPage": "RelatedItemPage",
      "RelationshipType": [
        "RelationshipType"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ],
      "SearchIndex": "SearchIndex",
      "Sort": "Sort",
      "Title": "Title",
      "ReleaseDate": "ReleaseDate",
      "IncludeReviewsSummary": "IncludeReviewsSummary",
      "TruncateReviewsAt": 86
    },
    "Request": [
      {
        "Availability": "Available",
        "Actor": "Actor",
        "Artist": "Artist",
        "AudienceRating": [
          "G"
        ],
        "Author": "Author",
        "Brand": "Brand",
        "BrowseNode": "BrowseNode",
        "Composer": "Composer",
        "Condition": "All",
        "Conductor": "Conductor",
        "Director": "Director",
        "ItemPage": 86,
        "Keywords": "Keywords",
        "Manufacturer": "Manufacturer",
        "MaximumPrice": 86,
        "MerchantId": "MerchantId",
        "MinimumPrice": 86,
        "MinPercentageOff": 86,
        "MusicLabel": "MusicLabel",
        "Orchestra": "Orchestra",
        "Power": "Power",
        "Publisher": "Publisher",
        "RelatedItemPage": "RelatedItemPage",
        "RelationshipType": [
          "RelationshipType"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ],
        "SearchIndex": "SearchIndex",
        "Sort": "Sort",
        "Title": "Title",
        "ReleaseDate": "ReleaseDate",
        "IncludeReviewsSummary": "IncludeReviewsSummary",
        "TruncateReviewsAt": 86
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([ItemSearchResponseMsg](#item_search_response_msg)) 
```
{
  "body": {
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 86,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    },
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 86.2825032236439
    }
  }
}
```


### <a name="item_lookup82"></a>![Endpoint: ](https://apidocs.io/img/method.png "ItemLookup82") ItemLookup82


**`POST`** `/ItemLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortUK`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ItemLookupRequestMsg](#item_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Condition": "All",
      "IdType": "ASIN",
      "MerchantId": "MerchantId",
      "ItemId": [
        "ItemId"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ],
      "SearchIndex": "SearchIndex",
      "VariationPage": "VariationPage",
      "RelatedItemPage": "RelatedItemPage",
      "RelationshipType": [
        "RelationshipType"
      ],
      "IncludeReviewsSummary": "IncludeReviewsSummary",
      "TruncateReviewsAt": 86
    },
    "Request": [
      {
        "Condition": "All",
        "IdType": "ASIN",
        "MerchantId": "MerchantId",
        "ItemId": [
          "ItemId"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ],
        "SearchIndex": "SearchIndex",
        "VariationPage": "VariationPage",
        "RelatedItemPage": "RelatedItemPage",
        "RelationshipType": [
          "RelationshipType"
        ],
        "IncludeReviewsSummary": "IncludeReviewsSummary",
        "TruncateReviewsAt": 86
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([ItemLookupResponseMsg](#item_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 86.2825032236439
    },
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 86,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    }
  }
}
```


### <a name="browse_node_lookup83"></a>![Endpoint: ](https://apidocs.io/img/method.png "BrowseNodeLookup83") BrowseNodeLookup83


**`POST`** `/BrowseNodeLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortUK`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [BrowseNodeLookupRequestMsg](#browse_node_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "BrowseNodeId": [
        "BrowseNodeId"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "BrowseNodeId": [
          "BrowseNodeId"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([BrowseNodeLookupResponseMsg](#browse_node_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 86.2825032236439
    },
    "BrowseNodes": [
      {
        "Request": {
          "BrowseNodeLookupRequest": {
            "BrowseNodeId": [
              "BrowseNodeId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "ItemSearchRequest": {
            "Availability": "Available",
            "Actor": "Actor",
            "Artist": "Artist",
            "AudienceRating": [
              "G"
            ],
            "Author": "Author",
            "Brand": "Brand",
            "BrowseNode": "BrowseNode",
            "Composer": "Composer",
            "Condition": "All",
            "Conductor": "Conductor",
            "Director": "Director",
            "ItemPage": 14,
            "Keywords": "Keywords",
            "Manufacturer": "Manufacturer",
            "MaximumPrice": 14,
            "MerchantId": "MerchantId",
            "MinimumPrice": 14,
            "MinPercentageOff": 14,
            "MusicLabel": "MusicLabel",
            "Orchestra": "Orchestra",
            "Power": "Power",
            "Publisher": "Publisher",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "Sort": "Sort",
            "Title": "Title",
            "ReleaseDate": "ReleaseDate",
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 14
          },
          "ItemLookupRequest": {
            "Condition": "All",
            "IdType": "ASIN",
            "MerchantId": "MerchantId",
            "ItemId": [
              "ItemId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "VariationPage": "VariationPage",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 14
          },
          "SimilarityLookupRequest": {
            "Condition": "All",
            "SimilarityType": "Intersection",
            "ItemId": [
              "ItemId"
            ],
            "MerchantId": "MerchantId",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartGetRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartAddRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 14,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartCreateRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 14,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartModifyRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 14,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartClearRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "Errors": {
            "Error": {
              "Code": "Code",
              "Message": "Message"
            }
          },
          "IsValid": "IsValid"
        },
        "BrowseNode": [
          {
            "Properties": {
              "Property": [
                {
                  "Name": "Name",
                  "Value": "Value"
                }
              ]
            },
            "Children": {
              "BrowseNode": []
            },
            "Ancestors": {
              "BrowseNode": []
            },
            "TopSellers": {
              "TopSeller": {
                "ASIN": "ASIN",
                "Title": "Title"
              }
            },
            "NewReleases": {
              "NewRelease": {
                "ASIN": "ASIN",
                "Title": "Title"
              }
            },
            "BrowseNodeId": "BrowseNodeId",
            "Name": "Name",
            "IsCategoryRoot": false,
            "TopItemSet": [
              {
                "TopItem": {
                  "ASIN": "ASIN",
                  "Title": "Title",
                  "DetailPageURL": "DetailPageURL",
                  "ProductGroup": "ProductGroup",
                  "Author": [
                    "Author"
                  ],
                  "Artist": [
                    "Artist"
                  ],
                  "Actor": [
                    "Actor"
                  ]
                },
                "Type": "Type"
              }
            ]
          }
        ]
      }
    ]
  }
}
```


### <a name="similarity_lookup84"></a>![Endpoint: ](https://apidocs.io/img/method.png "SimilarityLookup84") SimilarityLookup84


**`POST`** `/SimilarityLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortUK`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [SimilarityLookupRequestMsg](#similarity_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Condition": "All",
      "SimilarityType": "Intersection",
      "ItemId": [
        "ItemId"
      ],
      "MerchantId": "MerchantId",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Condition": "All",
        "SimilarityType": "Intersection",
        "ItemId": [
          "ItemId"
        ],
        "MerchantId": "MerchantId",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([SimilarityLookupResponseMsg](#similarity_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 14.2730670069685
    },
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 14,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    }
  }
}
```


### <a name="cart_get85"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartGet85") CartGet85


**`POST`** `/CartGet`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortUK`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartGetRequestMsg](#cart_get_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartGetResponseMsg](#cart_get_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 14.2730670069685
    },
    "Cart": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "URLEncodedHMAC": "URLEncodedHMAC",
        "Request": {
          "BrowseNodeLookupRequest": {
            "BrowseNodeId": [
              "BrowseNodeId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "ItemSearchRequest": {
            "Availability": "Available",
            "Actor": "Actor",
            "Artist": "Artist",
            "AudienceRating": [
              "G"
            ],
            "Author": "Author",
            "Brand": "Brand",
            "BrowseNode": "BrowseNode",
            "Composer": "Composer",
            "Condition": "All",
            "Conductor": "Conductor",
            "Director": "Director",
            "ItemPage": 14,
            "Keywords": "Keywords",
            "Manufacturer": "Manufacturer",
            "MaximumPrice": 14,
            "MerchantId": "MerchantId",
            "MinimumPrice": 14,
            "MinPercentageOff": 14,
            "MusicLabel": "MusicLabel",
            "Orchestra": "Orchestra",
            "Power": "Power",
            "Publisher": "Publisher",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "Sort": "Sort",
            "Title": "Title",
            "ReleaseDate": "ReleaseDate",
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 14
          },
          "ItemLookupRequest": {
            "Condition": "All",
            "IdType": "ASIN",
            "MerchantId": "MerchantId",
            "ItemId": [
              "ItemId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "VariationPage": "VariationPage",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 14
          },
          "SimilarityLookupRequest": {
            "Condition": "All",
            "SimilarityType": "Intersection",
            "ItemId": [
              "ItemId"
            ],
            "MerchantId": "MerchantId",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartGetRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartAddRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 14,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartCreateRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 14,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartModifyRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 14,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartClearRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "Errors": {
            "Error": {
              "Code": "Code",
              "Message": "Message"
            }
          },
          "IsValid": "IsValid"
        },
        "PurchaseURL": "PurchaseURL",
        "MobileCartURL": "MobileCartURL",
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 14,
          "CurrencyCode": "CurrencyCode"
        },
        "CartItems": {
          "CartItem": [
            {
              "CartItemId": "CartItemId",
              "Quantity": "Quantity",
              "MetaData": {
                "KeyValuePair": {
                  "Key": "Key",
                  "Value": "Value"
                }
              },
              "Price": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 14,
                "CurrencyCode": "CurrencyCode"
              },
              "ASIN": "ASIN",
              "SellerNickname": "SellerNickname",
              "Title": "Title",
              "ProductGroup": "ProductGroup",
              "ItemTotal": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 14,
                "CurrencyCode": "CurrencyCode"
              }
            }
          ],
          "SubTotal": {
            "FormattedPrice": "FormattedPrice",
            "Amount": 14,
            "CurrencyCode": "CurrencyCode"
          }
        },
        "SavedForLaterItems": {
          "SavedForLaterItem": [
            {
              "CartItemId": "CartItemId",
              "Quantity": "Quantity",
              "MetaData": {
                "KeyValuePair": {
                  "Key": "Key",
                  "Value": "Value"
                }
              },
              "Price": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 14,
                "CurrencyCode": "CurrencyCode"
              },
              "ASIN": "ASIN",
              "SellerNickname": "SellerNickname",
              "Title": "Title",
              "ProductGroup": "ProductGroup",
              "ItemTotal": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 14,
                "CurrencyCode": "CurrencyCode"
              }
            }
          ],
          "SubTotal": {
            "FormattedPrice": "FormattedPrice",
            "Amount": 14,
            "CurrencyCode": "CurrencyCode"
          }
        },
        "SimilarProducts": {
          "SimilarProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "TopSellers": {
          "TopSeller": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "NewReleases": {
          "NewRelease": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "SimilarViewedProducts": {
          "SimilarViewedProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "OtherCategoriesSimilarProducts": {
          "OtherCategoriesSimilarProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        }
      }
    ]
  }
}
```


### <a name="cart_add86"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartAdd86") CartAdd86


**`POST`** `/CartAdd`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortUK`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartAddRequestMsg](#cart_add_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 227,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 227,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartAddResponseMsg](#cart_add_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 227.549893780402
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 227,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 227,
          "MerchantId": "MerchantId",
          "MinimumPrice": 227,
          "MinPercentageOff": 227,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 227
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 227
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 227,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 227,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 227,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 227,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 227,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 227,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 227,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 227,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 227,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 227,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_create87"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartCreate87") CartCreate87


**`POST`** `/CartCreate`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortUK`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartCreateRequestMsg](#cart_create_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 64,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 64,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartCreateResponseMsg](#cart_create_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 64.0451756720641
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 64,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 64,
          "MerchantId": "MerchantId",
          "MinimumPrice": 64,
          "MinPercentageOff": 64,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 64
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 64
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 64,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 64,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 64,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 64,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 64,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 64,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 64,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 64,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 64,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 64,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_modify88"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartModify88") CartModify88


**`POST`** `/CartModify`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortUK`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartModifyRequestMsg](#cart_modify_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 64,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 22,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartModifyResponseMsg](#cart_modify_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 22.3220024454975
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 22,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 22,
          "MerchantId": "MerchantId",
          "MinimumPrice": 22,
          "MinPercentageOff": 22,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 22
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 22
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 22,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 22,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 22,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 22,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 22,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 22,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 22,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 22,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 22,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 22,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_clear89"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartClear89") CartClear89


**`POST`** `/CartClear`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortUK`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartClearRequestMsg](#cart_clear_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartClearResponseMsg](#cart_clear_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 113.81728433716
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 113,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 113,
          "MerchantId": "MerchantId",
          "MinimumPrice": 113,
          "MinPercentageOff": 113,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 113
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 113
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 113,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 113,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 113,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 113,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 113,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 113,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 113,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 113,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 113,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 113,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="item_search90"></a>![Endpoint: ](https://apidocs.io/img/method.png "ItemSearch90") ItemSearch90


**`POST`** `/ItemSearch`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortUS`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ItemSearchRequestMsg](#item_search_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "XMLEscaping": "XMLEscaping",
    "Validate": "Validate",
    "Shared": {
      "Availability": "Available",
      "Actor": "Actor",
      "Artist": "Artist",
      "AudienceRating": [
        "G"
      ],
      "Author": "Author",
      "Brand": "Brand",
      "BrowseNode": "BrowseNode",
      "Composer": "Composer",
      "Condition": "All",
      "Conductor": "Conductor",
      "Director": "Director",
      "ItemPage": 113,
      "Keywords": "Keywords",
      "Manufacturer": "Manufacturer",
      "MaximumPrice": 113,
      "MerchantId": "MerchantId",
      "MinimumPrice": 113,
      "MinPercentageOff": 113,
      "MusicLabel": "MusicLabel",
      "Orchestra": "Orchestra",
      "Power": "Power",
      "Publisher": "Publisher",
      "RelatedItemPage": "RelatedItemPage",
      "RelationshipType": [
        "RelationshipType"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ],
      "SearchIndex": "SearchIndex",
      "Sort": "Sort",
      "Title": "Title",
      "ReleaseDate": "ReleaseDate",
      "IncludeReviewsSummary": "IncludeReviewsSummary",
      "TruncateReviewsAt": 113
    },
    "Request": [
      {
        "Availability": "Available",
        "Actor": "Actor",
        "Artist": "Artist",
        "AudienceRating": [
          "G"
        ],
        "Author": "Author",
        "Brand": "Brand",
        "BrowseNode": "BrowseNode",
        "Composer": "Composer",
        "Condition": "All",
        "Conductor": "Conductor",
        "Director": "Director",
        "ItemPage": 113,
        "Keywords": "Keywords",
        "Manufacturer": "Manufacturer",
        "MaximumPrice": 113,
        "MerchantId": "MerchantId",
        "MinimumPrice": 113,
        "MinPercentageOff": 113,
        "MusicLabel": "MusicLabel",
        "Orchestra": "Orchestra",
        "Power": "Power",
        "Publisher": "Publisher",
        "RelatedItemPage": "RelatedItemPage",
        "RelationshipType": [
          "RelationshipType"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ],
        "SearchIndex": "SearchIndex",
        "Sort": "Sort",
        "Title": "Title",
        "ReleaseDate": "ReleaseDate",
        "IncludeReviewsSummary": "IncludeReviewsSummary",
        "TruncateReviewsAt": 113
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([ItemSearchResponseMsg](#item_search_response_msg)) 
```
{
  "body": {
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 205,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    },
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 205.312566228822
    }
  }
}
```


### <a name="item_lookup91"></a>![Endpoint: ](https://apidocs.io/img/method.png "ItemLookup91") ItemLookup91


**`POST`** `/ItemLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortUS`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [ItemLookupRequestMsg](#item_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Condition": "All",
      "IdType": "ASIN",
      "MerchantId": "MerchantId",
      "ItemId": [
        "ItemId"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ],
      "SearchIndex": "SearchIndex",
      "VariationPage": "VariationPage",
      "RelatedItemPage": "RelatedItemPage",
      "RelationshipType": [
        "RelationshipType"
      ],
      "IncludeReviewsSummary": "IncludeReviewsSummary",
      "TruncateReviewsAt": 205
    },
    "Request": [
      {
        "Condition": "All",
        "IdType": "ASIN",
        "MerchantId": "MerchantId",
        "ItemId": [
          "ItemId"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ],
        "SearchIndex": "SearchIndex",
        "VariationPage": "VariationPage",
        "RelatedItemPage": "RelatedItemPage",
        "RelationshipType": [
          "RelationshipType"
        ],
        "IncludeReviewsSummary": "IncludeReviewsSummary",
        "TruncateReviewsAt": 205
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([ItemLookupResponseMsg](#item_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 205.312566228822
    },
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 205,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    }
  }
}
```


### <a name="browse_node_lookup92"></a>![Endpoint: ](https://apidocs.io/img/method.png "BrowseNodeLookup92") BrowseNodeLookup92


**`POST`** `/BrowseNodeLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortUS`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [BrowseNodeLookupRequestMsg](#browse_node_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "BrowseNodeId": [
        "BrowseNodeId"
      ],
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "BrowseNodeId": [
          "BrowseNodeId"
        ],
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([BrowseNodeLookupResponseMsg](#browse_node_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 205.312566228822
    },
    "BrowseNodes": [
      {
        "Request": {
          "BrowseNodeLookupRequest": {
            "BrowseNodeId": [
              "BrowseNodeId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "ItemSearchRequest": {
            "Availability": "Available",
            "Actor": "Actor",
            "Artist": "Artist",
            "AudienceRating": [
              "G"
            ],
            "Author": "Author",
            "Brand": "Brand",
            "BrowseNode": "BrowseNode",
            "Composer": "Composer",
            "Condition": "All",
            "Conductor": "Conductor",
            "Director": "Director",
            "ItemPage": 205,
            "Keywords": "Keywords",
            "Manufacturer": "Manufacturer",
            "MaximumPrice": 205,
            "MerchantId": "MerchantId",
            "MinimumPrice": 205,
            "MinPercentageOff": 205,
            "MusicLabel": "MusicLabel",
            "Orchestra": "Orchestra",
            "Power": "Power",
            "Publisher": "Publisher",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "Sort": "Sort",
            "Title": "Title",
            "ReleaseDate": "ReleaseDate",
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 205
          },
          "ItemLookupRequest": {
            "Condition": "All",
            "IdType": "ASIN",
            "MerchantId": "MerchantId",
            "ItemId": [
              "ItemId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "VariationPage": "VariationPage",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 205
          },
          "SimilarityLookupRequest": {
            "Condition": "All",
            "SimilarityType": "Intersection",
            "ItemId": [
              "ItemId"
            ],
            "MerchantId": "MerchantId",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartGetRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartAddRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 205,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartCreateRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 205,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartModifyRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 205,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartClearRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "Errors": {
            "Error": {
              "Code": "Code",
              "Message": "Message"
            }
          },
          "IsValid": "IsValid"
        },
        "BrowseNode": [
          {
            "Properties": {
              "Property": [
                {
                  "Name": "Name",
                  "Value": "Value"
                }
              ]
            },
            "Children": {
              "BrowseNode": []
            },
            "Ancestors": {
              "BrowseNode": []
            },
            "TopSellers": {
              "TopSeller": {
                "ASIN": "ASIN",
                "Title": "Title"
              }
            },
            "NewReleases": {
              "NewRelease": {
                "ASIN": "ASIN",
                "Title": "Title"
              }
            },
            "BrowseNodeId": "BrowseNodeId",
            "Name": "Name",
            "IsCategoryRoot": true,
            "TopItemSet": [
              {
                "TopItem": {
                  "ASIN": "ASIN",
                  "Title": "Title",
                  "DetailPageURL": "DetailPageURL",
                  "ProductGroup": "ProductGroup",
                  "Author": [
                    "Author"
                  ],
                  "Artist": [
                    "Artist"
                  ],
                  "Actor": [
                    "Actor"
                  ]
                },
                "Type": "Type"
              }
            ]
          }
        ]
      }
    ]
  }
}
```


### <a name="similarity_lookup93"></a>![Endpoint: ](https://apidocs.io/img/method.png "SimilarityLookup93") SimilarityLookup93


**`POST`** `/SimilarityLookup`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortUS`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [SimilarityLookupRequestMsg](#similarity_lookup_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Condition": "All",
      "SimilarityType": "Intersection",
      "ItemId": [
        "ItemId"
      ],
      "MerchantId": "MerchantId",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Condition": "All",
        "SimilarityType": "Intersection",
        "ItemId": [
          "ItemId"
        ],
        "MerchantId": "MerchantId",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([SimilarityLookupResponseMsg](#similarity_lookup_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 163.589393002256
    },
    "Items": {
      "Item": {
        "ASIN": "ASIN",
        "OfferListingId": "OfferListingId",
        "Quantity": 163,
        "AssociateTag": "AssociateTag",
        "ListItemId": "ListItemId"
      }
    }
  }
}
```


### <a name="cart_get94"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartGet94") CartGet94


**`POST`** `/CartGet`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortUS`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartGetRequestMsg](#cart_get_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartGetResponseMsg](#cart_get_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 163.589393002256
    },
    "Cart": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "URLEncodedHMAC": "URLEncodedHMAC",
        "Request": {
          "BrowseNodeLookupRequest": {
            "BrowseNodeId": [
              "BrowseNodeId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "ItemSearchRequest": {
            "Availability": "Available",
            "Actor": "Actor",
            "Artist": "Artist",
            "AudienceRating": [
              "G"
            ],
            "Author": "Author",
            "Brand": "Brand",
            "BrowseNode": "BrowseNode",
            "Composer": "Composer",
            "Condition": "All",
            "Conductor": "Conductor",
            "Director": "Director",
            "ItemPage": 163,
            "Keywords": "Keywords",
            "Manufacturer": "Manufacturer",
            "MaximumPrice": 163,
            "MerchantId": "MerchantId",
            "MinimumPrice": 163,
            "MinPercentageOff": 163,
            "MusicLabel": "MusicLabel",
            "Orchestra": "Orchestra",
            "Power": "Power",
            "Publisher": "Publisher",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "Sort": "Sort",
            "Title": "Title",
            "ReleaseDate": "ReleaseDate",
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 163
          },
          "ItemLookupRequest": {
            "Condition": "All",
            "IdType": "ASIN",
            "MerchantId": "MerchantId",
            "ItemId": [
              "ItemId"
            ],
            "ResponseGroup": [
              "ResponseGroup"
            ],
            "SearchIndex": "SearchIndex",
            "VariationPage": "VariationPage",
            "RelatedItemPage": "RelatedItemPage",
            "RelationshipType": [
              "RelationshipType"
            ],
            "IncludeReviewsSummary": "IncludeReviewsSummary",
            "TruncateReviewsAt": 163
          },
          "SimilarityLookupRequest": {
            "Condition": "All",
            "SimilarityType": "Intersection",
            "ItemId": [
              "ItemId"
            ],
            "MerchantId": "MerchantId",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartGetRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartAddRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 163,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartCreateRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 163,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartModifyRequest": {
            "Items": {
              "Item": {
                "ASIN": "ASIN",
                "OfferListingId": "OfferListingId",
                "Quantity": 163,
                "AssociateTag": "AssociateTag",
                "ListItemId": "ListItemId"
              }
            },
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "CartClearRequest": {
            "CartId": "CartId",
            "HMAC": "HMAC",
            "MergeCart": "MergeCart",
            "ResponseGroup": [
              "ResponseGroup"
            ]
          },
          "Errors": {
            "Error": {
              "Code": "Code",
              "Message": "Message"
            }
          },
          "IsValid": "IsValid"
        },
        "PurchaseURL": "PurchaseURL",
        "MobileCartURL": "MobileCartURL",
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 163,
          "CurrencyCode": "CurrencyCode"
        },
        "CartItems": {
          "CartItem": [
            {
              "CartItemId": "CartItemId",
              "Quantity": "Quantity",
              "MetaData": {
                "KeyValuePair": {
                  "Key": "Key",
                  "Value": "Value"
                }
              },
              "Price": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 163,
                "CurrencyCode": "CurrencyCode"
              },
              "ASIN": "ASIN",
              "SellerNickname": "SellerNickname",
              "Title": "Title",
              "ProductGroup": "ProductGroup",
              "ItemTotal": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 163,
                "CurrencyCode": "CurrencyCode"
              }
            }
          ],
          "SubTotal": {
            "FormattedPrice": "FormattedPrice",
            "Amount": 163,
            "CurrencyCode": "CurrencyCode"
          }
        },
        "SavedForLaterItems": {
          "SavedForLaterItem": [
            {
              "CartItemId": "CartItemId",
              "Quantity": "Quantity",
              "MetaData": {
                "KeyValuePair": {
                  "Key": "Key",
                  "Value": "Value"
                }
              },
              "Price": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 163,
                "CurrencyCode": "CurrencyCode"
              },
              "ASIN": "ASIN",
              "SellerNickname": "SellerNickname",
              "Title": "Title",
              "ProductGroup": "ProductGroup",
              "ItemTotal": {
                "FormattedPrice": "FormattedPrice",
                "Amount": 163,
                "CurrencyCode": "CurrencyCode"
              }
            }
          ],
          "SubTotal": {
            "FormattedPrice": "FormattedPrice",
            "Amount": 163,
            "CurrencyCode": "CurrencyCode"
          }
        },
        "SimilarProducts": {
          "SimilarProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "TopSellers": {
          "TopSeller": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "NewReleases": {
          "NewRelease": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "SimilarViewedProducts": {
          "SimilarViewedProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        },
        "OtherCategoriesSimilarProducts": {
          "OtherCategoriesSimilarProduct": {
            "ASIN": "ASIN",
            "Title": "Title"
          }
        }
      }
    ]
  }
}
```


### <a name="cart_add95"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartAdd95") CartAdd95


**`POST`** `/CartAdd`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortUS`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartAddRequestMsg](#cart_add_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 0,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 0,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartAddResponseMsg](#cart_add_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 0.0846748939178301
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 0,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 0,
          "MerchantId": "MerchantId",
          "MinimumPrice": 0,
          "MinPercentageOff": 0,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 0
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 0
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 0,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 0,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 0,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 0,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 0,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 0,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 0,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 0,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 0,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 0,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_create96"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartCreate96") CartCreate96


**`POST`** `/CartCreate`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortUS`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartCreateRequestMsg](#cart_create_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 91,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 91,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartCreateResponseMsg](#cart_create_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 91.5799567855801
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 91,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 91,
          "MerchantId": "MerchantId",
          "MinimumPrice": 91,
          "MinPercentageOff": 91,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 91
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 91
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 91,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 91,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 91,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 91,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 91,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 91,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 91,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 91,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 91,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 91,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_modify97"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartModify97") CartModify97


**`POST`** `/CartModify`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortUS`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartModifyRequestMsg](#cart_modify_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "Items": {
        "Item": {
          "ASIN": "ASIN",
          "OfferListingId": "OfferListingId",
          "Quantity": 49,
          "AssociateTag": "AssociateTag",
          "ListItemId": "ListItemId"
        }
      },
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "Items": {
          "Item": {
            "ASIN": "ASIN",
            "OfferListingId": "OfferListingId",
            "Quantity": 49,
            "AssociateTag": "AssociateTag",
            "ListItemId": "ListItemId"
          }
        },
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartModifyResponseMsg](#cart_modify_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 49.8567835590135
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 49,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 49,
          "MerchantId": "MerchantId",
          "MinimumPrice": 49,
          "MinPercentageOff": 49,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 49
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 49
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 49,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 49,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 49,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 49,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 49,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 49,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 49,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 49,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 49,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 49,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


### <a name="cart_clear98"></a>![Endpoint: ](https://apidocs.io/img/method.png "CartClear98") CartClear98


**`POST`** `/CartClear`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


#### Base URL
This endpoint uses server `AWSECommerceServicePortUS`.


#### Request Headers
>Accept=application/json;
>Content-Type=application/json;

#### Request Body
Raw 

|  Type | Tags | Description |
| ------| ---- |-------------| 
| [CartClearRequestMsg](#cart_clear_request_msg) |  ``` Required ```  | TODO: Add description | 

 Example 
``` 
{
  "body": {
    "MarketplaceDomain": "MarketplaceDomain",
    "AWSAccessKeyId": "AWSAccessKeyId",
    "AssociateTag": "AssociateTag",
    "Validate": "Validate",
    "XMLEscaping": "XMLEscaping",
    "Shared": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "MergeCart": "MergeCart",
      "ResponseGroup": [
        "ResponseGroup"
      ]
    },
    "Request": [
      {
        "CartId": "CartId",
        "HMAC": "HMAC",
        "MergeCart": "MergeCart",
        "ResponseGroup": [
          "ResponseGroup"
        ]
      }
    ]
  }
}
``` 

#### Responses
**200** 


Body ([CartClearResponseMsg](#cart_clear_response_msg)) 
```
{
  "body": {
    "OperationRequest": {
      "HTTPHeaders": {
        "Header": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "RequestId": "RequestId",
      "Arguments": {
        "Argument": {
          "Name": "Name",
          "Value": "Value"
        }
      },
      "Errors": {
        "Error": {
          "Code": "Code",
          "Message": "Message"
        }
      },
      "RequestProcessingTime": 141.352065450676
    },
    "Cart": {
      "CartId": "CartId",
      "HMAC": "HMAC",
      "URLEncodedHMAC": "URLEncodedHMAC",
      "Request": {
        "BrowseNodeLookupRequest": {
          "BrowseNodeId": [
            "BrowseNodeId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "ItemSearchRequest": {
          "Availability": "Available",
          "Actor": "Actor",
          "Artist": "Artist",
          "AudienceRating": [
            "G"
          ],
          "Author": "Author",
          "Brand": "Brand",
          "BrowseNode": "BrowseNode",
          "Composer": "Composer",
          "Condition": "All",
          "Conductor": "Conductor",
          "Director": "Director",
          "ItemPage": 141,
          "Keywords": "Keywords",
          "Manufacturer": "Manufacturer",
          "MaximumPrice": 141,
          "MerchantId": "MerchantId",
          "MinimumPrice": 141,
          "MinPercentageOff": 141,
          "MusicLabel": "MusicLabel",
          "Orchestra": "Orchestra",
          "Power": "Power",
          "Publisher": "Publisher",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "Sort": "Sort",
          "Title": "Title",
          "ReleaseDate": "ReleaseDate",
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 141
        },
        "ItemLookupRequest": {
          "Condition": "All",
          "IdType": "ASIN",
          "MerchantId": "MerchantId",
          "ItemId": [
            "ItemId"
          ],
          "ResponseGroup": [
            "ResponseGroup"
          ],
          "SearchIndex": "SearchIndex",
          "VariationPage": "VariationPage",
          "RelatedItemPage": "RelatedItemPage",
          "RelationshipType": [
            "RelationshipType"
          ],
          "IncludeReviewsSummary": "IncludeReviewsSummary",
          "TruncateReviewsAt": 141
        },
        "SimilarityLookupRequest": {
          "Condition": "All",
          "SimilarityType": "Intersection",
          "ItemId": [
            "ItemId"
          ],
          "MerchantId": "MerchantId",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartGetRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartAddRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 141,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartCreateRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 141,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartModifyRequest": {
          "Items": {
            "Item": {
              "ASIN": "ASIN",
              "OfferListingId": "OfferListingId",
              "Quantity": 141,
              "AssociateTag": "AssociateTag",
              "ListItemId": "ListItemId"
            }
          },
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "CartClearRequest": {
          "CartId": "CartId",
          "HMAC": "HMAC",
          "MergeCart": "MergeCart",
          "ResponseGroup": [
            "ResponseGroup"
          ]
        },
        "Errors": {
          "Error": {
            "Code": "Code",
            "Message": "Message"
          }
        },
        "IsValid": "IsValid"
      },
      "PurchaseURL": "PurchaseURL",
      "MobileCartURL": "MobileCartURL",
      "SubTotal": {
        "FormattedPrice": "FormattedPrice",
        "Amount": 141,
        "CurrencyCode": "CurrencyCode"
      },
      "CartItems": {
        "CartItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 141,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 141,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 141,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SavedForLaterItems": {
        "SavedForLaterItem": [
          {
            "CartItemId": "CartItemId",
            "Quantity": "Quantity",
            "MetaData": {
              "KeyValuePair": {
                "Key": "Key",
                "Value": "Value"
              }
            },
            "Price": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 141,
              "CurrencyCode": "CurrencyCode"
            },
            "ASIN": "ASIN",
            "SellerNickname": "SellerNickname",
            "Title": "Title",
            "ProductGroup": "ProductGroup",
            "ItemTotal": {
              "FormattedPrice": "FormattedPrice",
              "Amount": 141,
              "CurrencyCode": "CurrencyCode"
            }
          }
        ],
        "SubTotal": {
          "FormattedPrice": "FormattedPrice",
          "Amount": 141,
          "CurrencyCode": "CurrencyCode"
        }
      },
      "SimilarProducts": {
        "SimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "TopSellers": {
        "TopSeller": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "NewReleases": {
        "NewRelease": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "SimilarViewedProducts": {
        "SimilarViewedProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      },
      "OtherCategoriesSimilarProducts": {
        "OtherCategoriesSimilarProduct": {
          "ASIN": "ASIN",
          "Title": "Title"
        }
      }
    }
  }
}
```


[Back to API Reference](#api_reference)

## <a name="o_auth_authorization"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "OAuth Authorization") OAuth Authorization


### <a name="request_token"></a>![Endpoint: ](https://apidocs.io/img/method.png "request token") request token


**`POST`** `/sdsdfsdfsdfsdf`

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"authorization_code"` | 
| code | [string](#api_types) |  ``` Required ```  | Authorization Code |  | 
| redirect_uri | [string](#api_types) |  ``` Required ```  | Redirect Uri |  | 

##### Example
```
 grant_type = authorization_code 
 code = "code" 
 redirect_uri = "redirect_uri" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 141,
  "scope": "scope",
  "expiry": 141,
  "refresh_token": "refresh_token"
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="refresh_token"></a>![Endpoint: ](https://apidocs.io/img/method.png "refresh token") refresh token


**`POST`** `/sdsdfsdfsdfsdf`

> *Tags:*  ``` Skips Authentication ``` 

> Obtain a new access token using a refresh token




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"refresh_token"` | 
| refresh_token | [string](#api_types) |  ``` Required ```  | Refresh token |  | 
| scope | [string](#api_types) |  ``` Optional ```  | Requested scopes as a space-delimited list. |  | 

##### Example
```
 grant_type = refresh_token 
 refresh_token = "refresh_token" 
 scope = "scope" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 141,
  "scope": "scope",
  "expiry": 141,
  "refresh_token": "refresh_token"
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="request_token1"></a>![Endpoint: ](https://apidocs.io/img/method.png "request token1") request token1


**`POST`** `/sdsdfsdfsdfsdf`

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"authorization_code"` | 
| code | [string](#api_types) |  ``` Required ```  | Authorization Code |  | 
| redirect_uri | [string](#api_types) |  ``` Required ```  | Redirect Uri |  | 

##### Example
```
 grant_type = authorization_code 
 code = "code" 
 redirect_uri = "redirect_uri" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 141,
  "scope": "scope",
  "expiry": 141,
  "refresh_token": "refresh_token"
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="refresh_token1"></a>![Endpoint: ](https://apidocs.io/img/method.png "refresh token1") refresh token1


**`POST`** `/sdsdfsdfsdfsdf`

> *Tags:*  ``` Skips Authentication ``` 

> Obtain a new access token using a refresh token




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"refresh_token"` | 
| refresh_token | [string](#api_types) |  ``` Required ```  | Refresh token |  | 
| scope | [string](#api_types) |  ``` Optional ```  | Requested scopes as a space-delimited list. |  | 

##### Example
```
 grant_type = refresh_token 
 refresh_token = "refresh_token" 
 scope = "scope" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 141,
  "scope": "scope",
  "expiry": 141,
  "refresh_token": "refresh_token"
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="request_token2"></a>![Endpoint: ](https://apidocs.io/img/method.png "request token2") request token2


**`POST`** `/sdsdfsdfsdfsdf`

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"authorization_code"` | 
| code | [string](#api_types) |  ``` Required ```  | Authorization Code |  | 
| redirect_uri | [string](#api_types) |  ``` Required ```  | Redirect Uri |  | 

##### Example
```
 grant_type = authorization_code 
 code = "code" 
 redirect_uri = "redirect_uri" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 141,
  "scope": "scope",
  "expiry": 141,
  "refresh_token": "refresh_token"
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="refresh_token2"></a>![Endpoint: ](https://apidocs.io/img/method.png "refresh token2") refresh token2


**`POST`** `/sdsdfsdfsdfsdf`

> *Tags:*  ``` Skips Authentication ``` 

> Obtain a new access token using a refresh token




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"refresh_token"` | 
| refresh_token | [string](#api_types) |  ``` Required ```  | Refresh token |  | 
| scope | [string](#api_types) |  ``` Optional ```  | Requested scopes as a space-delimited list. |  | 

##### Example
```
 grant_type = refresh_token 
 refresh_token = "refresh_token" 
 scope = "scope" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 141,
  "scope": "scope",
  "expiry": 141,
  "refresh_token": "refresh_token"
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="request_token11"></a>![Endpoint: ](https://apidocs.io/img/method.png "request token11") request token11


**`POST`** `/sdsdfsdfsdfsdf`

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"authorization_code"` | 
| code | [string](#api_types) |  ``` Required ```  | Authorization Code |  | 
| redirect_uri | [string](#api_types) |  ``` Required ```  | Redirect Uri |  | 

##### Example
```
 grant_type = authorization_code 
 code = "code" 
 redirect_uri = "redirect_uri" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 99,
  "scope": "scope",
  "expiry": 99,
  "refresh_token": "refresh_token"
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="refresh_token11"></a>![Endpoint: ](https://apidocs.io/img/method.png "refresh token11") refresh token11


**`POST`** `/sdsdfsdfsdfsdf`

> *Tags:*  ``` Skips Authentication ``` 

> Obtain a new access token using a refresh token




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"refresh_token"` | 
| refresh_token | [string](#api_types) |  ``` Required ```  | Refresh token |  | 
| scope | [string](#api_types) |  ``` Optional ```  | Requested scopes as a space-delimited list. |  | 

##### Example
```
 grant_type = refresh_token 
 refresh_token = "refresh_token" 
 scope = "scope" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 99,
  "scope": "scope",
  "expiry": 99,
  "refresh_token": "refresh_token"
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="request_token21"></a>![Endpoint: ](https://apidocs.io/img/method.png "request token21") request token21


**`POST`** `/sdsdfsdfsdfsdf`

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"authorization_code"` | 
| code | [string](#api_types) |  ``` Required ```  | Authorization Code |  | 
| redirect_uri | [string](#api_types) |  ``` Required ```  | Redirect Uri |  | 

##### Example
```
 grant_type = authorization_code 
 code = "code" 
 redirect_uri = "redirect_uri" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 99,
  "scope": "scope",
  "expiry": 99,
  "refresh_token": "refresh_token"
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="refresh_token21"></a>![Endpoint: ](https://apidocs.io/img/method.png "refresh token21") refresh token21


**`POST`** `/sdsdfsdfsdfsdf`

> *Tags:*  ``` Skips Authentication ``` 

> Obtain a new access token using a refresh token




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"refresh_token"` | 
| refresh_token | [string](#api_types) |  ``` Required ```  | Refresh token |  | 
| scope | [string](#api_types) |  ``` Optional ```  | Requested scopes as a space-delimited list. |  | 

##### Example
```
 grant_type = refresh_token 
 refresh_token = "refresh_token" 
 scope = "scope" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 99,
  "scope": "scope",
  "expiry": 99,
  "refresh_token": "refresh_token"
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="request_token11"></a>![Endpoint: ](https://apidocs.io/img/method.png "request token11") request token11


**`POST`** `/sdsdfsdfsdfsdf`

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"authorization_code"` | 
| code | [string](#api_types) |  ``` Required ```  | Authorization Code |  | 
| redirect_uri | [string](#api_types) |  ``` Required ```  | Redirect Uri |  | 

##### Example
```
 grant_type = authorization_code 
 code = "code" 
 redirect_uri = "redirect_uri" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 99,
  "scope": "scope",
  "expiry": 99,
  "refresh_token": "refresh_token"
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="refresh_token11"></a>![Endpoint: ](https://apidocs.io/img/method.png "refresh token11") refresh token11


**`POST`** `/sdsdfsdfsdfsdf`

> *Tags:*  ``` Skips Authentication ``` 

> Obtain a new access token using a refresh token




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"refresh_token"` | 
| refresh_token | [string](#api_types) |  ``` Required ```  | Refresh token |  | 
| scope | [string](#api_types) |  ``` Optional ```  | Requested scopes as a space-delimited list. |  | 

##### Example
```
 grant_type = refresh_token 
 refresh_token = "refresh_token" 
 scope = "scope" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 99,
  "scope": "scope",
  "expiry": 99,
  "refresh_token": "refresh_token"
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="request_token1"></a>![Endpoint: ](https://apidocs.io/img/method.png "request token1") request token1


**`POST`** `/sdsdfsdfsdfsdf`

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"authorization_code"` | 
| code | [string](#api_types) |  ``` Required ```  | Authorization Code |  | 
| redirect_uri | [string](#api_types) |  ``` Required ```  | Redirect Uri |  | 

##### Example
```
 grant_type = authorization_code 
 code = "code" 
 redirect_uri = "redirect_uri" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 99,
  "scope": "scope",
  "expiry": 99,
  "refresh_token": "refresh_token"
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="refresh_token1"></a>![Endpoint: ](https://apidocs.io/img/method.png "refresh token1") refresh token1


**`POST`** `/sdsdfsdfsdfsdf`

> *Tags:*  ``` Skips Authentication ``` 

> Obtain a new access token using a refresh token




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"refresh_token"` | 
| refresh_token | [string](#api_types) |  ``` Required ```  | Refresh token |  | 
| scope | [string](#api_types) |  ``` Optional ```  | Requested scopes as a space-delimited list. |  | 

##### Example
```
 grant_type = refresh_token 
 refresh_token = "refresh_token" 
 scope = "scope" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 99,
  "scope": "scope",
  "expiry": 99,
  "refresh_token": "refresh_token"
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="request_token2"></a>![Endpoint: ](https://apidocs.io/img/method.png "request token2") request token2


**`POST`** `/sdsdfsdfsdfsdf`

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"authorization_code"` | 
| code | [string](#api_types) |  ``` Required ```  | Authorization Code |  | 
| redirect_uri | [string](#api_types) |  ``` Required ```  | Redirect Uri |  | 

##### Example
```
 grant_type = authorization_code 
 code = "code" 
 redirect_uri = "redirect_uri" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 99,
  "scope": "scope",
  "expiry": 99,
  "refresh_token": "refresh_token"
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="refresh_token2"></a>![Endpoint: ](https://apidocs.io/img/method.png "refresh token2") refresh token2


**`POST`** `/sdsdfsdfsdfsdf`

> *Tags:*  ``` Skips Authentication ``` 

> Obtain a new access token using a refresh token




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"refresh_token"` | 
| refresh_token | [string](#api_types) |  ``` Required ```  | Refresh token |  | 
| scope | [string](#api_types) |  ``` Optional ```  | Requested scopes as a space-delimited list. |  | 

##### Example
```
 grant_type = refresh_token 
 refresh_token = "refresh_token" 
 scope = "scope" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 99,
  "scope": "scope",
  "expiry": 99,
  "refresh_token": "refresh_token"
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="request_token3"></a>![Endpoint: ](https://apidocs.io/img/method.png "request token3") request token3


**`POST`** `/sdsdfsdfsdfsdf`

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"authorization_code"` | 
| code | [string](#api_types) |  ``` Required ```  | Authorization Code |  | 
| redirect_uri | [string](#api_types) |  ``` Required ```  | Redirect Uri |  | 

##### Example
```
 grant_type = authorization_code 
 code = "code" 
 redirect_uri = "redirect_uri" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 99,
  "scope": "scope",
  "expiry": 99,
  "refresh_token": "refresh_token"
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="refresh_token3"></a>![Endpoint: ](https://apidocs.io/img/method.png "refresh token3") refresh token3


**`POST`** `/sdsdfsdfsdfsdf`

> *Tags:*  ``` Skips Authentication ``` 

> Obtain a new access token using a refresh token




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"refresh_token"` | 
| refresh_token | [string](#api_types) |  ``` Required ```  | Refresh token |  | 
| scope | [string](#api_types) |  ``` Optional ```  | Requested scopes as a space-delimited list. |  | 

##### Example
```
 grant_type = refresh_token 
 refresh_token = "refresh_token" 
 scope = "scope" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 99,
  "scope": "scope",
  "expiry": 99,
  "refresh_token": "refresh_token"
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="request_token"></a>![Endpoint: ](https://apidocs.io/img/method.png "request token") request token


**`POST`** `/sdsdfsdfsdfsdf`

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"authorization_code"` | 
| code | [string](#api_types) |  ``` Required ```  | Authorization Code |  | 
| redirect_uri | [string](#api_types) |  ``` Required ```  | Redirect Uri |  | 

##### Example
```
 grant_type = authorization_code 
 code = "code" 
 redirect_uri = "redirect_uri" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 99,
  "scope": "scope",
  "expiry": 99,
  "refresh_token": "refresh_token"
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="refresh_token"></a>![Endpoint: ](https://apidocs.io/img/method.png "refresh token") refresh token


**`POST`** `/sdsdfsdfsdfsdf`

> *Tags:*  ``` Skips Authentication ``` 

> Obtain a new access token using a refresh token




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"refresh_token"` | 
| refresh_token | [string](#api_types) |  ``` Required ```  | Refresh token |  | 
| scope | [string](#api_types) |  ``` Optional ```  | Requested scopes as a space-delimited list. |  | 

##### Example
```
 grant_type = refresh_token 
 refresh_token = "refresh_token" 
 scope = "scope" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 191,
  "scope": "scope",
  "expiry": 191,
  "refresh_token": "refresh_token"
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


[Back to API Reference](#api_reference)

## <a name="api_types"></a>![Models: ](https://apidocs.io/img/class.png "API Types") API Types

This section provides details on the available types. The primitive types available are:

| Type | Example |
| ---- | -------- |
| **string** | `hello world` |
| **boolean** |	`true` |
| **number** | `1` |
| **precision** | `1.5` |
| **datetime** | `2016-03-13T12:52:32.123Z` |
| **date** | `2016-03-13` |
|**void** | |
| **dynamic** | |
| **binary** | |
| **long** | `12345678910` |
| **file** | |
| **uuid** | `0f8fad5b-d9cb-469f-a165-70867728950e` |


In addition to the above types, the following complex types are also available:
### <a name="bin_parameter"></a>![Model: ](https://apidocs.io/img/method.png "BinParameter") BinParameter



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Name | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| Value | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 




### <a name="bin"></a>![Model: ](https://apidocs.io/img/method.png "Bin") Bin



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| BinName | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| BinItemCount | [number](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| BinParameter | [BinParameter](#bin_parameter) |  ``` Required ```  | TODO: Add a property description | 




### <a name="search_bin_set"></a>![Model: ](https://apidocs.io/img/method.png "SearchBinSet") SearchBinSet



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| NarrowBy | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| Bin | [Bin](#bin) |  ``` Required ```  | TODO: Add a property description | 




### <a name="search_bin_sets"></a>![Model: ](https://apidocs.io/img/method.png "SearchBinSets") SearchBinSets



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| SearchBinSet | [SearchBinSet](#search_bin_set) |  ``` Required ```  | TODO: Add a property description | 




### <a name="availability"></a>![Model: ](https://apidocs.io/img/method.png "Availability") Availability



> TODO: Add a method description




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `Available` | TODO: Add description | 




### <a name="audience_rating"></a>![Model: ](https://apidocs.io/img/method.png "AudienceRating") AudienceRating



> TODO: Add a method description




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `G` | TODO: Add description | 
| `PG` | TODO: Add description | 
| `PG-13` | TODO: Add description | 
| `R` | TODO: Add description | 
| `NC-17` | TODO: Add description | 
| `NR` | TODO: Add description | 
| `Unrated` | TODO: Add description | 
| `6` | TODO: Add description | 
| `12` | TODO: Add description | 
| `16` | TODO: Add description | 
| `18` | TODO: Add description | 
| `FamilyViewing` | TODO: Add description | 




### <a name="condition"></a>![Model: ](https://apidocs.io/img/method.png "Condition") Condition



> TODO: Add a method description




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `All` | TODO: Add description | 
| `New` | TODO: Add description | 
| `Used` | TODO: Add description | 
| `Collectible` | TODO: Add description | 
| `Refurbished` | TODO: Add description | 




### <a name="item_search_request"></a>![Model: ](https://apidocs.io/img/method.png "ItemSearchRequest") ItemSearchRequest



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Availability | [Availability](#availability) |  ``` Required ```  | TODO: Add a property description | 
| Actor | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Artist | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| AudienceRating | [AudienceRating](#audience_rating) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| Author | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Brand | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| BrowseNode | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Composer | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Condition | [Condition](#condition) |  ``` Optional ```  | TODO: Add a property description | 
| Conductor | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Director | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ItemPage | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Keywords | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Manufacturer | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| MaximumPrice | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| MerchantId | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| MinimumPrice | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| MinPercentageOff | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| MusicLabel | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Orchestra | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Power | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Publisher | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| RelatedItemPage | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| RelationshipType | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| ResponseGroup | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| SearchIndex | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Sort | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Title | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ReleaseDate | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| IncludeReviewsSummary | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| TruncateReviewsAt | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="item_search"></a>![Model: ](https://apidocs.io/img/method.png "ItemSearch") ItemSearch



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| MarketplaceDomain | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| AWSAccessKeyId | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| AssociateTag | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| XMLEscaping | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Validate | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Shared | [ItemSearchRequest](#item_search_request) |  ``` Optional ```  | TODO: Add a property description | 
| Request | [ItemSearchRequest](#item_search_request) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="id_type"></a>![Model: ](https://apidocs.io/img/method.png "IdType") IdType



> TODO: Add a method description




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `ASIN` | TODO: Add description | 
| `UPC` | TODO: Add description | 
| `SKU` | TODO: Add description | 
| `EAN` | TODO: Add description | 
| `ISBN` | TODO: Add description | 




### <a name="item_lookup_request"></a>![Model: ](https://apidocs.io/img/method.png "ItemLookupRequest") ItemLookupRequest



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Condition | [Condition](#condition) |  ``` Required ```  | TODO: Add a property description | 
| IdType | [IdType](#id_type) |  ``` Required ```  | TODO: Add a property description | 
| MerchantId | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ItemId | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| ResponseGroup | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| SearchIndex | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| VariationPage | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| RelatedItemPage | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| RelationshipType | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| IncludeReviewsSummary | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| TruncateReviewsAt | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="item_lookup"></a>![Model: ](https://apidocs.io/img/method.png "ItemLookup") ItemLookup



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| MarketplaceDomain | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| AWSAccessKeyId | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| AssociateTag | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Validate | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| XMLEscaping | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Shared | [ItemLookupRequest](#item_lookup_request) |  ``` Optional ```  | TODO: Add a property description | 
| Request | [ItemLookupRequest](#item_lookup_request) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="similarity_type"></a>![Model: ](https://apidocs.io/img/method.png "SimilarityType") SimilarityType



> TODO: Add a method description




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `Intersection` | TODO: Add description | 
| `Random` | TODO: Add description | 




### <a name="similarity_lookup_request"></a>![Model: ](https://apidocs.io/img/method.png "SimilarityLookupRequest") SimilarityLookupRequest



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Condition | [Condition](#condition) |  ``` Required ```  | TODO: Add a property description | 
| SimilarityType | [SimilarityType](#similarity_type) |  ``` Required ```  | TODO: Add a property description | 
| ItemId | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| MerchantId | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ResponseGroup | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="similarity_lookup"></a>![Model: ](https://apidocs.io/img/method.png "SimilarityLookup") SimilarityLookup



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| MarketplaceDomain | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| AWSAccessKeyId | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| AssociateTag | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Validate | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| XMLEscaping | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Shared | [SimilarityLookupRequest](#similarity_lookup_request) |  ``` Optional ```  | TODO: Add a property description | 
| Request | [SimilarityLookupRequest](#similarity_lookup_request) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="cart_get_request"></a>![Model: ](https://apidocs.io/img/method.png "CartGetRequest") CartGetRequest



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| CartId | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| HMAC | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| MergeCart | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ResponseGroup | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="cart_get"></a>![Model: ](https://apidocs.io/img/method.png "CartGet") CartGet



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| MarketplaceDomain | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| AWSAccessKeyId | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| AssociateTag | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Validate | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| XMLEscaping | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Shared | [CartGetRequest](#cart_get_request) |  ``` Optional ```  | TODO: Add a property description | 
| Request | [CartGetRequest](#cart_get_request) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="item"></a>![Model: ](https://apidocs.io/img/method.png "Item") Item



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| ASIN | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| OfferListingId | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Quantity | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| AssociateTag | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ListItemId | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="items"></a>![Model: ](https://apidocs.io/img/method.png "Items") Items



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Item | [Item](#item) |  ``` Required ```  | TODO: Add a property description | 




### <a name="cart_add_request"></a>![Model: ](https://apidocs.io/img/method.png "CartAddRequest") CartAddRequest



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Items | [Items](#items) |  ``` Required ```  | TODO: Add a property description | 
| CartId | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| HMAC | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| MergeCart | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ResponseGroup | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="cart_add"></a>![Model: ](https://apidocs.io/img/method.png "CartAdd") CartAdd



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| MarketplaceDomain | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| AWSAccessKeyId | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| AssociateTag | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Validate | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| XMLEscaping | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Shared | [CartAddRequest](#cart_add_request) |  ``` Optional ```  | TODO: Add a property description | 
| Request | [CartAddRequest](#cart_add_request) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="cart_create_request"></a>![Model: ](https://apidocs.io/img/method.png "CartCreateRequest") CartCreateRequest



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Items | [Items](#items) |  ``` Required ```  | TODO: Add a property description | 
| MergeCart | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ResponseGroup | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="cart_create"></a>![Model: ](https://apidocs.io/img/method.png "CartCreate") CartCreate



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| MarketplaceDomain | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| AWSAccessKeyId | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| AssociateTag | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Validate | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| XMLEscaping | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Shared | [CartCreateRequest](#cart_create_request) |  ``` Optional ```  | TODO: Add a property description | 
| Request | [CartCreateRequest](#cart_create_request) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="cart_modify_request"></a>![Model: ](https://apidocs.io/img/method.png "CartModifyRequest") CartModifyRequest



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Items | [Items](#items) |  ``` Required ```  | TODO: Add a property description | 
| CartId | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| HMAC | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| MergeCart | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ResponseGroup | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="cart_modify"></a>![Model: ](https://apidocs.io/img/method.png "CartModify") CartModify



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| MarketplaceDomain | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| AWSAccessKeyId | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| AssociateTag | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Validate | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| XMLEscaping | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Shared | [CartModifyRequest](#cart_modify_request) |  ``` Optional ```  | TODO: Add a property description | 
| Request | [CartModifyRequest](#cart_modify_request) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="cart_clear_request"></a>![Model: ](https://apidocs.io/img/method.png "CartClearRequest") CartClearRequest



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| CartId | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| HMAC | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| MergeCart | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ResponseGroup | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="cart_clear"></a>![Model: ](https://apidocs.io/img/method.png "CartClear") CartClear



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| MarketplaceDomain | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| AWSAccessKeyId | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| AssociateTag | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Validate | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| XMLEscaping | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Shared | [CartClearRequest](#cart_clear_request) |  ``` Optional ```  | TODO: Add a property description | 
| Request | [CartClearRequest](#cart_clear_request) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="browse_node_lookup_request"></a>![Model: ](https://apidocs.io/img/method.png "BrowseNodeLookupRequest") BrowseNodeLookupRequest



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| BrowseNodeId | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| ResponseGroup | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="browse_node_lookup"></a>![Model: ](https://apidocs.io/img/method.png "BrowseNodeLookup") BrowseNodeLookup



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| MarketplaceDomain | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| AWSAccessKeyId | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| AssociateTag | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Validate | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| XMLEscaping | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Shared | [BrowseNodeLookupRequest](#browse_node_lookup_request) |  ``` Optional ```  | TODO: Add a property description | 
| Request | [BrowseNodeLookupRequest](#browse_node_lookup_request) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="header"></a>![Model: ](https://apidocs.io/img/method.png "Header") Header



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Name | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| Value | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 




### <a name="http_headers"></a>![Model: ](https://apidocs.io/img/method.png "HTTPHeaders") HTTPHeaders



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Header | [Header](#header) |  ``` Required ```  | TODO: Add a property description | 




### <a name="argument"></a>![Model: ](https://apidocs.io/img/method.png "Argument") Argument



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Name | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| Value | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="arguments"></a>![Model: ](https://apidocs.io/img/method.png "Arguments") Arguments



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Argument | [Argument](#argument) |  ``` Required ```  | TODO: Add a property description | 




### <a name="error"></a>![Model: ](https://apidocs.io/img/method.png "Error") Error



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Code | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| Message | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 




### <a name="errors"></a>![Model: ](https://apidocs.io/img/method.png "Errors") Errors



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Error | [Error](#error) |  ``` Required ```  | TODO: Add a property description | 




### <a name="operation_request"></a>![Model: ](https://apidocs.io/img/method.png "OperationRequest") OperationRequest



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| HTTPHeaders | [HTTPHeaders](#http_headers) |  ``` Optional ```  | TODO: Add a property description | 
| RequestId | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Arguments | [Arguments](#arguments) |  ``` Optional ```  | TODO: Add a property description | 
| Errors | [Errors](#errors) |  ``` Optional ```  | TODO: Add a property description | 
| RequestProcessingTime | [precision](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="item_search_response"></a>![Model: ](https://apidocs.io/img/method.png "ItemSearchResponse") ItemSearchResponse



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Items | [Items](#items) |  ``` Required ```  | TODO: Add a property description | 
| OperationRequest | [OperationRequest](#operation_request) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="item_lookup_response"></a>![Model: ](https://apidocs.io/img/method.png "ItemLookupResponse") ItemLookupResponse



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| OperationRequest | [OperationRequest](#operation_request) |  ``` Required ```  | TODO: Add a property description | 
| Items | [Items](#items) |  ``` Required ```  | TODO: Add a property description | 




### <a name="similarity_lookup_response"></a>![Model: ](https://apidocs.io/img/method.png "SimilarityLookupResponse") SimilarityLookupResponse



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| OperationRequest | [OperationRequest](#operation_request) |  ``` Required ```  | TODO: Add a property description | 
| Items | [Items](#items) |  ``` Required ```  | TODO: Add a property description | 




### <a name="request"></a>![Model: ](https://apidocs.io/img/method.png "Request") Request



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| BrowseNodeLookupRequest | [BrowseNodeLookupRequest](#browse_node_lookup_request) |  ``` Required ```  | TODO: Add a property description | 
| ItemSearchRequest | [ItemSearchRequest](#item_search_request) |  ``` Required ```  | TODO: Add a property description | 
| ItemLookupRequest | [ItemLookupRequest](#item_lookup_request) |  ``` Required ```  | TODO: Add a property description | 
| SimilarityLookupRequest | [SimilarityLookupRequest](#similarity_lookup_request) |  ``` Required ```  | TODO: Add a property description | 
| CartGetRequest | [CartGetRequest](#cart_get_request) |  ``` Required ```  | TODO: Add a property description | 
| CartAddRequest | [CartAddRequest](#cart_add_request) |  ``` Required ```  | TODO: Add a property description | 
| CartCreateRequest | [CartCreateRequest](#cart_create_request) |  ``` Required ```  | TODO: Add a property description | 
| CartModifyRequest | [CartModifyRequest](#cart_modify_request) |  ``` Required ```  | TODO: Add a property description | 
| CartClearRequest | [CartClearRequest](#cart_clear_request) |  ``` Required ```  | TODO: Add a property description | 
| Errors | [Errors](#errors) |  ``` Required ```  | TODO: Add a property description | 
| IsValid | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="price"></a>![Model: ](https://apidocs.io/img/method.png "Price") Price



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| FormattedPrice | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| Amount | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| CurrencyCode | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="key_value_pair"></a>![Model: ](https://apidocs.io/img/method.png "KeyValuePair") KeyValuePair



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Key | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| Value | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 




### <a name="meta_data"></a>![Model: ](https://apidocs.io/img/method.png "MetaData") MetaData



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| KeyValuePair | [KeyValuePair](#key_value_pair) |  ``` Required ```  | TODO: Add a property description | 




### <a name="cart_item"></a>![Model: ](https://apidocs.io/img/method.png "CartItem") CartItem



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| CartItemId | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| Quantity | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| MetaData | [MetaData](#meta_data) |  ``` Required ```  | TODO: Add a property description | 
| Price | [Price](#price) |  ``` Required ```  | TODO: Add a property description | 
| ASIN | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| SellerNickname | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Title | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ProductGroup | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ItemTotal | [Price](#price) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="cart_items"></a>![Model: ](https://apidocs.io/img/method.png "CartItems") CartItems



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| CartItem | [CartItem](#cart_item) |  ``` Required ```  ``` Collection ```  | TODO: Add a property description | 
| SubTotal | [Price](#price) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="saved_for_later_items"></a>![Model: ](https://apidocs.io/img/method.png "SavedForLaterItems") SavedForLaterItems



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| SavedForLaterItem | [CartItem](#cart_item) |  ``` Required ```  ``` Collection ```  | TODO: Add a property description | 
| SubTotal | [Price](#price) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="similar_product"></a>![Model: ](https://apidocs.io/img/method.png "SimilarProduct") SimilarProduct



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| ASIN | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Title | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="similar_products"></a>![Model: ](https://apidocs.io/img/method.png "SimilarProducts") SimilarProducts



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| SimilarProduct | [SimilarProduct](#similar_product) |  ``` Required ```  | TODO: Add a property description | 




### <a name="top_seller"></a>![Model: ](https://apidocs.io/img/method.png "TopSeller") TopSeller



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| ASIN | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Title | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="top_sellers"></a>![Model: ](https://apidocs.io/img/method.png "TopSellers") TopSellers



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| TopSeller | [TopSeller](#top_seller) |  ``` Required ```  | TODO: Add a property description | 




### <a name="new_release"></a>![Model: ](https://apidocs.io/img/method.png "NewRelease") NewRelease



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| ASIN | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Title | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="new_releases"></a>![Model: ](https://apidocs.io/img/method.png "NewReleases") NewReleases



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| NewRelease | [NewRelease](#new_release) |  ``` Required ```  | TODO: Add a property description | 




### <a name="similar_viewed_product"></a>![Model: ](https://apidocs.io/img/method.png "SimilarViewedProduct") SimilarViewedProduct



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| ASIN | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Title | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="similar_viewed_products"></a>![Model: ](https://apidocs.io/img/method.png "SimilarViewedProducts") SimilarViewedProducts



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| SimilarViewedProduct | [SimilarViewedProduct](#similar_viewed_product) |  ``` Required ```  | TODO: Add a property description | 




### <a name="other_categories_similar_product"></a>![Model: ](https://apidocs.io/img/method.png "OtherCategoriesSimilarProduct") OtherCategoriesSimilarProduct



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| ASIN | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Title | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="other_categories_similar_products"></a>![Model: ](https://apidocs.io/img/method.png "OtherCategoriesSimilarProducts") OtherCategoriesSimilarProducts



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| OtherCategoriesSimilarProduct | [OtherCategoriesSimilarProduct](#other_categories_similar_product) |  ``` Required ```  | TODO: Add a property description | 




### <a name="cart"></a>![Model: ](https://apidocs.io/img/method.png "Cart") Cart



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| CartId | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| HMAC | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| URLEncodedHMAC | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| Request | [Request](#request) |  ``` Optional ```  | TODO: Add a property description | 
| PurchaseURL | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| MobileCartURL | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| SubTotal | [Price](#price) |  ``` Optional ```  | TODO: Add a property description | 
| CartItems | [CartItems](#cart_items) |  ``` Optional ```  | TODO: Add a property description | 
| SavedForLaterItems | [SavedForLaterItems](#saved_for_later_items) |  ``` Optional ```  | TODO: Add a property description | 
| SimilarProducts | [SimilarProducts](#similar_products) |  ``` Optional ```  | TODO: Add a property description | 
| TopSellers | [TopSellers](#top_sellers) |  ``` Optional ```  | TODO: Add a property description | 
| NewReleases | [NewReleases](#new_releases) |  ``` Optional ```  | TODO: Add a property description | 
| SimilarViewedProducts | [SimilarViewedProducts](#similar_viewed_products) |  ``` Optional ```  | TODO: Add a property description | 
| OtherCategoriesSimilarProducts | [OtherCategoriesSimilarProducts](#other_categories_similar_products) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="cart_get_response"></a>![Model: ](https://apidocs.io/img/method.png "CartGetResponse") CartGetResponse



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| OperationRequest | [OperationRequest](#operation_request) |  ``` Required ```  | TODO: Add a property description | 
| Cart | [Cart](#cart) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="cart_add_response"></a>![Model: ](https://apidocs.io/img/method.png "CartAddResponse") CartAddResponse



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| OperationRequest | [OperationRequest](#operation_request) |  ``` Required ```  | TODO: Add a property description | 
| Cart | [Cart](#cart) |  ``` Required ```  | TODO: Add a property description | 




### <a name="cart_create_response"></a>![Model: ](https://apidocs.io/img/method.png "CartCreateResponse") CartCreateResponse



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| OperationRequest | [OperationRequest](#operation_request) |  ``` Required ```  | TODO: Add a property description | 
| Cart | [Cart](#cart) |  ``` Required ```  | TODO: Add a property description | 




### <a name="cart_modify_response"></a>![Model: ](https://apidocs.io/img/method.png "CartModifyResponse") CartModifyResponse



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| OperationRequest | [OperationRequest](#operation_request) |  ``` Required ```  | TODO: Add a property description | 
| Cart | [Cart](#cart) |  ``` Required ```  | TODO: Add a property description | 




### <a name="cart_clear_response"></a>![Model: ](https://apidocs.io/img/method.png "CartClearResponse") CartClearResponse



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| OperationRequest | [OperationRequest](#operation_request) |  ``` Required ```  | TODO: Add a property description | 
| Cart | [Cart](#cart) |  ``` Required ```  | TODO: Add a property description | 




### <a name="property"></a>![Model: ](https://apidocs.io/img/method.png "Property") Property



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Name | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Value | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="properties"></a>![Model: ](https://apidocs.io/img/method.png "Properties") Properties



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Property | [Property](#property) |  ``` Required ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="children"></a>![Model: ](https://apidocs.io/img/method.png "Children") Children



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| BrowseNode | [BrowseNode](#browse_node) |  ``` Required ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="ancestors"></a>![Model: ](https://apidocs.io/img/method.png "Ancestors") Ancestors



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| BrowseNode | [BrowseNode](#browse_node) |  ``` Required ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="top_item"></a>![Model: ](https://apidocs.io/img/method.png "TopItem") TopItem



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| ASIN | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Title | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| DetailPageURL | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ProductGroup | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Author | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| Artist | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| Actor | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="top_item_set"></a>![Model: ](https://apidocs.io/img/method.png "TopItemSet") TopItemSet



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| TopItem | [TopItem](#top_item) |  ``` Required ```  | TODO: Add a property description | 
| Type | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="browse_node"></a>![Model: ](https://apidocs.io/img/method.png "BrowseNode") BrowseNode



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Properties | [Properties](#properties) |  ``` Required ```  | TODO: Add a property description | 
| Children | [Children](#children) |  ``` Required ```  | TODO: Add a property description | 
| Ancestors | [Ancestors](#ancestors) |  ``` Required ```  | TODO: Add a property description | 
| TopSellers | [TopSellers](#top_sellers) |  ``` Required ```  | TODO: Add a property description | 
| NewReleases | [NewReleases](#new_releases) |  ``` Required ```  | TODO: Add a property description | 
| BrowseNodeId | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Name | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| IsCategoryRoot | [boolean](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| TopItemSet | [TopItemSet](#top_item_set) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="browse_nodes"></a>![Model: ](https://apidocs.io/img/method.png "BrowseNodes") BrowseNodes



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Request | [Request](#request) |  ``` Required ```  | TODO: Add a property description | 
| BrowseNode | [BrowseNode](#browse_node) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="browse_node_lookup_response"></a>![Model: ](https://apidocs.io/img/method.png "BrowseNodeLookupResponse") BrowseNodeLookupResponse



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| OperationRequest | [OperationRequest](#operation_request) |  ``` Required ```  | TODO: Add a property description | 
| BrowseNodes | [BrowseNodes](#browse_nodes) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="corrected_query"></a>![Model: ](https://apidocs.io/img/method.png "CorrectedQuery") CorrectedQuery



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Keywords | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Message | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="search_index"></a>![Model: ](https://apidocs.io/img/method.png "SearchIndex") SearchIndex



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| IndexName | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| CorrectedQuery | [CorrectedQuery](#corrected_query) |  ``` Required ```  | TODO: Add a property description | 
| RelevanceRank | [number](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| ASIN | [string](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add a property description | 
| Results | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Pages | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="search_results_map"></a>![Model: ](https://apidocs.io/img/method.png "SearchResultsMap") SearchResultsMap



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| SearchIndex | [SearchIndex](#search_index) |  ``` Required ```  | TODO: Add a property description | 




### <a name="merchant"></a>![Model: ](https://apidocs.io/img/method.png "Merchant") Merchant



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Name | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="non_negative_integer_with_units"></a>![Model: ](https://apidocs.io/img/method.png "NonNegativeIntegerWithUnits") NonNegativeIntegerWithUnits



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Units | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 




### <a name="rental_listing"></a>![Model: ](https://apidocs.io/img/method.png "RentalListing") RentalListing



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Price | [Price](#price) |  ``` Required ```  | TODO: Add a property description | 
| Period | [NonNegativeIntegerWithUnits](#non_negative_integer_with_units) |  ``` Optional ```  | TODO: Add a property description | 
| IsFulfilledByAmazon | [boolean](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Disclaimer | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="rental_offer"></a>![Model: ](https://apidocs.io/img/method.png "RentalOffer") RentalOffer



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Merchant | [Merchant](#merchant) |  ``` Optional ```  | TODO: Add a property description | 
| RentalListing | [RentalListing](#rental_listing) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="rental_offers"></a>![Model: ](https://apidocs.io/img/method.png "RentalOffers") RentalOffers



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| RentalOffer | [RentalOffer](#rental_offer) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="item_link"></a>![Model: ](https://apidocs.io/img/method.png "ItemLink") ItemLink



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Description | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| URL | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="item_links"></a>![Model: ](https://apidocs.io/img/method.png "ItemLinks") ItemLinks



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| ItemLink | [ItemLink](#item_link) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="relationship"></a>![Model: ](https://apidocs.io/img/method.png "Relationship") Relationship



> TODO: Add a method description




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `Parents` | TODO: Add description | 
| `Children` | TODO: Add description | 




### <a name="related_item"></a>![Model: ](https://apidocs.io/img/method.png "RelatedItem") RelatedItem



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Item | [Item](#item) |  ``` Required ```  | TODO: Add a property description | 




### <a name="related_items"></a>![Model: ](https://apidocs.io/img/method.png "RelatedItems") RelatedItems



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Relationship | [Relationship](#relationship) |  ``` Required ```  | TODO: Add a property description | 
| RelationshipType | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| RelatedItemCount | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| RelatedItemPageCount | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| RelatedItemPage | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| RelatedItem | [RelatedItem](#related_item) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="offer_summary"></a>![Model: ](https://apidocs.io/img/method.png "OfferSummary") OfferSummary



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| LowestNewPrice | [Price](#price) |  ``` Optional ```  | TODO: Add a property description | 
| LowestUsedPrice | [Price](#price) |  ``` Optional ```  | TODO: Add a property description | 
| LowestCollectiblePrice | [Price](#price) |  ``` Optional ```  | TODO: Add a property description | 
| LowestRefurbishedPrice | [Price](#price) |  ``` Optional ```  | TODO: Add a property description | 
| TotalNew | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| TotalUsed | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| TotalCollectible | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| TotalRefurbished | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="offer_attributes"></a>![Model: ](https://apidocs.io/img/method.png "OfferAttributes") OfferAttributes



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Condition | [Condition](#condition) |  ``` Required ```  | TODO: Add a property description | 




### <a name="availability_attributes"></a>![Model: ](https://apidocs.io/img/method.png "AvailabilityAttributes") AvailabilityAttributes



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| AvailabilityType | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| IsPreorder | [boolean](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| MinimumHours | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| MaximumHours | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="offer_listing"></a>![Model: ](https://apidocs.io/img/method.png "OfferListing") OfferListing



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Price | [Price](#price) |  ``` Required ```  | TODO: Add a property description | 
| Availability | [Availability](#availability) |  ``` Required ```  | TODO: Add a property description | 
| AvailabilityAttributes | [AvailabilityAttributes](#availability_attributes) |  ``` Required ```  | TODO: Add a property description | 
| OfferListingId | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| PricePerUnit | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| SalePrice | [Price](#price) |  ``` Optional ```  | TODO: Add a property description | 
| AmountSaved | [Price](#price) |  ``` Optional ```  | TODO: Add a property description | 
| PercentageSaved | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| IsEligibleForSuperSaverShipping | [boolean](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| IsEligibleForPrimeFreeDigitalVideo | [boolean](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| IsEligibleForPrime | [boolean](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="loyalty_points"></a>![Model: ](https://apidocs.io/img/method.png "LoyaltyPoints") LoyaltyPoints



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Points | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| TypicalRedemptionValue | [Price](#price) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="summary"></a>![Model: ](https://apidocs.io/img/method.png "Summary") Summary



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| PromotionId | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| Message | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Category | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| StartDate | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| EndDate | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| EligibilityRequirementDescription | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| BenefitDescription | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| TermsAndConditions | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="promotion"></a>![Model: ](https://apidocs.io/img/method.png "Promotion") Promotion



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Summary | [Summary](#summary) |  ``` Required ```  | TODO: Add a property description | 




### <a name="promotions"></a>![Model: ](https://apidocs.io/img/method.png "Promotions") Promotions



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Promotion | [Promotion](#promotion) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="offer"></a>![Model: ](https://apidocs.io/img/method.png "Offer") Offer



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Merchant | [Merchant](#merchant) |  ``` Required ```  | TODO: Add a property description | 
| OfferAttributes | [OfferAttributes](#offer_attributes) |  ``` Optional ```  | TODO: Add a property description | 
| OfferListing | [OfferListing](#offer_listing) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| LoyaltyPoints | [LoyaltyPoints](#loyalty_points) |  ``` Optional ```  | TODO: Add a property description | 
| Promotions | [Promotions](#promotions) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="offers"></a>![Model: ](https://apidocs.io/img/method.png "Offers") Offers



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| TotalOffers | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| TotalOfferPages | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| MoreOffersUrl | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Offer | [Offer](#offer) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="variation_attribute"></a>![Model: ](https://apidocs.io/img/method.png "VariationAttribute") VariationAttribute



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Name | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| Value | [string](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="variation_summary"></a>![Model: ](https://apidocs.io/img/method.png "VariationSummary") VariationSummary



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| LowestPrice | [Price](#price) |  ``` Optional ```  | TODO: Add a property description | 
| HighestPrice | [Price](#price) |  ``` Optional ```  | TODO: Add a property description | 
| LowestSalePrice | [Price](#price) |  ``` Optional ```  | TODO: Add a property description | 
| HighestSalePrice | [Price](#price) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="variation_dimensions"></a>![Model: ](https://apidocs.io/img/method.png "VariationDimensions") VariationDimensions



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| VariationDimension | [string](#api_types) |  ``` Required ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="variations"></a>![Model: ](https://apidocs.io/img/method.png "Variations") Variations



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Item | [Item](#item) |  ``` Required ```  | TODO: Add a property description | 
| TotalVariations | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| TotalVariationPages | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| VariationDimensions | [VariationDimensions](#variation_dimensions) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="editorial_review"></a>![Model: ](https://apidocs.io/img/method.png "EditorialReview") EditorialReview



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Source | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Content | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| IsLinkSuppressed | [boolean](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="editorial_reviews"></a>![Model: ](https://apidocs.io/img/method.png "EditorialReviews") EditorialReviews



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| EditorialReview | [EditorialReview](#editorial_review) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="collection_summary"></a>![Model: ](https://apidocs.io/img/method.png "CollectionSummary") CollectionSummary



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| LowestListPrice | [Price](#price) |  ``` Optional ```  | TODO: Add a property description | 
| HighestListPrice | [Price](#price) |  ``` Optional ```  | TODO: Add a property description | 
| LowestSalePrice | [Price](#price) |  ``` Optional ```  | TODO: Add a property description | 
| HighestSalePrice | [Price](#price) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="collection_parent"></a>![Model: ](https://apidocs.io/img/method.png "CollectionParent") CollectionParent



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| ASIN | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Title | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="collection_item"></a>![Model: ](https://apidocs.io/img/method.png "CollectionItem") CollectionItem



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| ASIN | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Title | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="collection"></a>![Model: ](https://apidocs.io/img/method.png "Collection") Collection



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| CollectionSummary | [CollectionSummary](#collection_summary) |  ``` Required ```  | TODO: Add a property description | 
| CollectionParent | [CollectionParent](#collection_parent) |  ``` Required ```  | TODO: Add a property description | 
| CollectionItem | [CollectionItem](#collection_item) |  ``` Required ```  | TODO: Add a property description | 




### <a name="collections"></a>![Model: ](https://apidocs.io/img/method.png "Collections") Collections



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Collection | [Collection](#collection) |  ``` Required ```  | TODO: Add a property description | 




### <a name="customer_reviews"></a>![Model: ](https://apidocs.io/img/method.png "CustomerReviews") CustomerReviews



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| IFrameURL | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| HasReviews | [boolean](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="track"></a>![Model: ](https://apidocs.io/img/method.png "Track") Track



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Number | [number](#api_types) |  ``` Required ```  | TODO: Add a property description | 




### <a name="disc"></a>![Model: ](https://apidocs.io/img/method.png "Disc") Disc



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Number | [number](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| Track | [Track](#track) |  ``` Required ```  | TODO: Add a property description | 




### <a name="tracks"></a>![Model: ](https://apidocs.io/img/method.png "Tracks") Tracks



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Disc | [Disc](#disc) |  ``` Required ```  | TODO: Add a property description | 




### <a name="accessory"></a>![Model: ](https://apidocs.io/img/method.png "Accessory") Accessory



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| ASIN | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Title | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="accessories"></a>![Model: ](https://apidocs.io/img/method.png "Accessories") Accessories



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Accessory | [Accessory](#accessory) |  ``` Required ```  | TODO: Add a property description | 




### <a name="decimal_with_units"></a>![Model: ](https://apidocs.io/img/method.png "DecimalWithUnits") DecimalWithUnits



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Units | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 




### <a name="image"></a>![Model: ](https://apidocs.io/img/method.png "Image") Image



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| URL | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| Height | [DecimalWithUnits](#decimal_with_units) |  ``` Required ```  | TODO: Add a property description | 
| Width | [DecimalWithUnits](#decimal_with_units) |  ``` Required ```  | TODO: Add a property description | 
| IsVerified | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="image_set"></a>![Model: ](https://apidocs.io/img/method.png "ImageSet") ImageSet



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Category | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| SwatchImage | [Image](#image) |  ``` Optional ```  | TODO: Add a property description | 
| SmallImage | [Image](#image) |  ``` Optional ```  | TODO: Add a property description | 
| ThumbnailImage | [Image](#image) |  ``` Optional ```  | TODO: Add a property description | 
| TinyImage | [Image](#image) |  ``` Optional ```  | TODO: Add a property description | 
| MediumImage | [Image](#image) |  ``` Optional ```  | TODO: Add a property description | 
| LargeImage | [Image](#image) |  ``` Optional ```  | TODO: Add a property description | 
| HiResImage | [Image](#image) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="catalog_number_list"></a>![Model: ](https://apidocs.io/img/method.png "CatalogNumberList") CatalogNumberList



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| CatalogNumberListElement | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="creator"></a>![Model: ](https://apidocs.io/img/method.png "Creator") Creator



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Role | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 




### <a name="ean_list"></a>![Model: ](https://apidocs.io/img/method.png "EANList") EANList



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| EANListElement | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="item_dimensions"></a>![Model: ](https://apidocs.io/img/method.png "ItemDimensions") ItemDimensions



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Height | [DecimalWithUnits](#decimal_with_units) |  ``` Optional ```  | TODO: Add a property description | 
| Length | [DecimalWithUnits](#decimal_with_units) |  ``` Optional ```  | TODO: Add a property description | 
| Weight | [DecimalWithUnits](#decimal_with_units) |  ``` Optional ```  | TODO: Add a property description | 
| Width | [DecimalWithUnits](#decimal_with_units) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="language"></a>![Model: ](https://apidocs.io/img/method.png "Language") Language



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Name | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 
| Type | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| AudioFormat | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="languages"></a>![Model: ](https://apidocs.io/img/method.png "Languages") Languages



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Language | [Language](#language) |  ``` Required ```  | TODO: Add a property description | 




### <a name="package_dimensions"></a>![Model: ](https://apidocs.io/img/method.png "PackageDimensions") PackageDimensions



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Height | [DecimalWithUnits](#decimal_with_units) |  ``` Optional ```  | TODO: Add a property description | 
| Length | [DecimalWithUnits](#decimal_with_units) |  ``` Optional ```  | TODO: Add a property description | 
| Weight | [DecimalWithUnits](#decimal_with_units) |  ``` Optional ```  | TODO: Add a property description | 
| Width | [DecimalWithUnits](#decimal_with_units) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="upc_list"></a>![Model: ](https://apidocs.io/img/method.png "UPCList") UPCList



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| UPCListElement | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 




### <a name="item_attributes"></a>![Model: ](https://apidocs.io/img/method.png "ItemAttributes") ItemAttributes



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| AudienceRating | [AudienceRating](#audience_rating) |  ``` Required ```  | TODO: Add a property description | 
| CatalogNumberList | [CatalogNumberList](#catalog_number_list) |  ``` Required ```  | TODO: Add a property description | 
| Creator | [Creator](#creator) |  ``` Required ```  | TODO: Add a property description | 
| EANList | [EANList](#ean_list) |  ``` Required ```  | TODO: Add a property description | 
| ItemDimensions | [ItemDimensions](#item_dimensions) |  ``` Required ```  | TODO: Add a property description | 
| Languages | [Languages](#languages) |  ``` Required ```  | TODO: Add a property description | 
| PackageDimensions | [PackageDimensions](#package_dimensions) |  ``` Required ```  | TODO: Add a property description | 
| UPCList | [UPCList](#upc_list) |  ``` Required ```  | TODO: Add a property description | 
| Actor | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| Artist | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| AspectRatio | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| AudioFormat | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| Author | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| Binding | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Brand | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Category | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| CEROAgeRating | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ClothingSize | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Color | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Department | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Director | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| EAN | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Edition | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| EISBN | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| EnergyEfficiencyClass | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| EpisodeSequence | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ESRBAgeRating | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Feature | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| Format | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| Genre | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| HardwarePlatform | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| HazardousMaterialType | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| IsAdultProduct | [boolean](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| IsAutographed | [boolean](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ISBN | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| IsEligibleForTradeIn | [boolean](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| IsMemorabilia | [boolean](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| IssuesPerYear | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ItemPartNumber | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Label | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| LegalDisclaimer | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ListPrice | [Price](#price) |  ``` Optional ```  | TODO: Add a property description | 
| MagazineType | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Manufacturer | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ManufacturerMaximumAge | [DecimalWithUnits](#decimal_with_units) |  ``` Optional ```  | TODO: Add a property description | 
| ManufacturerMinimumAge | [DecimalWithUnits](#decimal_with_units) |  ``` Optional ```  | TODO: Add a property description | 
| ManufacturerPartsWarrantyDescription | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| MediaType | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Model | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ModelYear | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| MPN | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| NumberOfDiscs | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| NumberOfIssues | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| NumberOfItems | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| NumberOfPages | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| NumberOfTracks | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| OperatingSystem | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| PackageQuantity | [number](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| PartNumber | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| PictureFormat | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| Platform | [string](#api_types) |  ``` Optional ```  ``` Collection ```  | TODO: Add a property description | 
| ProductGroup | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ProductTypeName | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ProductTypeSubcategory | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| PublicationDate | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Publisher | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| RegionCode | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| ReleaseDate | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| SeasonSequence | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| RunningTime | [DecimalWithUnits](#decimal_with_units) |  ``` Optional ```  | TODO: Add a property description | 
| SeikodoProductCode | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Size | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| SKU | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Studio | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| SubscriptionLength | [NonNegativeIntegerWithUnits](#non_negative_integer_with_units) |  ``` Optional ```  | TODO: Add a property description | 
| Title | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| TrackSequence | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| TradeInValue | [Price](#price) |  ``` Optional ```  | TODO: Add a property description | 
| UPC | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| Warranty | [string](#api_types) |  ``` Optional ```  | TODO: Add a property description | 
| WEEETaxValue | [Price](#price) |  ``` Optional ```  | TODO: Add a property description | 




### <a name="string_with_units"></a>![Model: ](https://apidocs.io/img/method.png "StringWithUnits") StringWithUnits



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| Units | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 




### <a name="item_search_response_msg"></a>![Model: ](https://apidocs.io/img/method.png "ItemSearchResponseMsg") ItemSearchResponseMsg



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| body | [ItemSearchResponse](#item_search_response) |  ``` Required ```  | TODO: Add a property description | 




### <a name="item_lookup_response_msg"></a>![Model: ](https://apidocs.io/img/method.png "ItemLookupResponseMsg") ItemLookupResponseMsg



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| body | [ItemLookupResponse](#item_lookup_response) |  ``` Required ```  | TODO: Add a property description | 




### <a name="browse_node_lookup_response_msg"></a>![Model: ](https://apidocs.io/img/method.png "BrowseNodeLookupResponseMsg") BrowseNodeLookupResponseMsg



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| body | [BrowseNodeLookupResponse](#browse_node_lookup_response) |  ``` Required ```  | TODO: Add a property description | 




### <a name="similarity_lookup_response_msg"></a>![Model: ](https://apidocs.io/img/method.png "SimilarityLookupResponseMsg") SimilarityLookupResponseMsg



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| body | [SimilarityLookupResponse](#similarity_lookup_response) |  ``` Required ```  | TODO: Add a property description | 




### <a name="cart_get_response_msg"></a>![Model: ](https://apidocs.io/img/method.png "CartGetResponseMsg") CartGetResponseMsg



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| body | [CartGetResponse](#cart_get_response) |  ``` Required ```  | TODO: Add a property description | 




### <a name="cart_add_response_msg"></a>![Model: ](https://apidocs.io/img/method.png "CartAddResponseMsg") CartAddResponseMsg



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| body | [CartAddResponse](#cart_add_response) |  ``` Required ```  | TODO: Add a property description | 




### <a name="cart_create_response_msg"></a>![Model: ](https://apidocs.io/img/method.png "CartCreateResponseMsg") CartCreateResponseMsg



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| body | [CartCreateResponse](#cart_create_response) |  ``` Required ```  | TODO: Add a property description | 




### <a name="cart_modify_response_msg"></a>![Model: ](https://apidocs.io/img/method.png "CartModifyResponseMsg") CartModifyResponseMsg



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| body | [CartModifyResponse](#cart_modify_response) |  ``` Required ```  | TODO: Add a property description | 




### <a name="cart_clear_response_msg"></a>![Model: ](https://apidocs.io/img/method.png "CartClearResponseMsg") CartClearResponseMsg



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| body | [CartClearResponse](#cart_clear_response) |  ``` Required ```  | TODO: Add a property description | 




### <a name="item_search_request_msg"></a>![Model: ](https://apidocs.io/img/method.png "ItemSearchRequestMsg") ItemSearchRequestMsg



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| body | [ItemSearch](#item_search) |  ``` Required ```  | TODO: Add a property description | 




### <a name="item_lookup_request_msg"></a>![Model: ](https://apidocs.io/img/method.png "ItemLookupRequestMsg") ItemLookupRequestMsg



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| body | [ItemLookup](#item_lookup) |  ``` Required ```  | TODO: Add a property description | 




### <a name="browse_node_lookup_request_msg"></a>![Model: ](https://apidocs.io/img/method.png "BrowseNodeLookupRequestMsg") BrowseNodeLookupRequestMsg



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| body | [BrowseNodeLookup](#browse_node_lookup) |  ``` Required ```  | TODO: Add a property description | 




### <a name="similarity_lookup_request_msg"></a>![Model: ](https://apidocs.io/img/method.png "SimilarityLookupRequestMsg") SimilarityLookupRequestMsg



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| body | [SimilarityLookup](#similarity_lookup) |  ``` Required ```  | TODO: Add a property description | 




### <a name="cart_get_request_msg"></a>![Model: ](https://apidocs.io/img/method.png "CartGetRequestMsg") CartGetRequestMsg



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| body | [CartGet](#cart_get) |  ``` Required ```  | TODO: Add a property description | 




### <a name="cart_add_request_msg"></a>![Model: ](https://apidocs.io/img/method.png "CartAddRequestMsg") CartAddRequestMsg



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| body | [CartAdd](#cart_add) |  ``` Required ```  | TODO: Add a property description | 




### <a name="cart_create_request_msg"></a>![Model: ](https://apidocs.io/img/method.png "CartCreateRequestMsg") CartCreateRequestMsg



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| body | [CartCreate](#cart_create) |  ``` Required ```  | TODO: Add a property description | 




### <a name="cart_modify_request_msg"></a>![Model: ](https://apidocs.io/img/method.png "CartModifyRequestMsg") CartModifyRequestMsg



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| body | [CartModify](#cart_modify) |  ``` Required ```  | TODO: Add a property description | 




### <a name="cart_clear_request_msg"></a>![Model: ](https://apidocs.io/img/method.png "CartClearRequestMsg") CartClearRequestMsg



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| body | [CartClear](#cart_clear) |  ``` Required ```  | TODO: Add a property description | 




### <a name="o_auth_token"></a>![Model: ](https://apidocs.io/img/method.png "OAuthToken") OAuthToken



> OAuth 2 Authorization endpoint response




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| access_token | [string](#api_types) |  ``` Required ```  | Access token | 
| token_type | [string](#api_types) |  ``` Required ```  | Type of access token | 
| expires_in | [long](#api_types) |  ``` Optional ```  | Time in seconds before the access token expires | 
| scope | [string](#api_types) |  ``` Optional ```  | List of scopes granted<br>This is a space-delimited list of strings. | 
| expiry | [long](#api_types) |  ``` Optional ```  | Time of token expiry as unix timestamp (UTC) | 
| refresh_token | [string](#api_types) |  ``` Optional ```  | Refresh token<br>Used to get a new access token when it expires. | 




### <a name="o_auth_provider"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProvider") OAuthProvider



> OAuth 2 Authorization endpoint exception




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| error | [OAuthProviderError](#o_auth_provider_error) |  ``` Required ```  | Error code | 
| error_description | [string](#api_types) |  ``` Optional ```  | Human-readable text providing additional information on error.<br>Used to assist the client developer in understanding the error that occurred. | 
| error_uri | [string](#api_types) |  ``` Optional ```  | A URI identifying a human-readable web page with information about the error, used to provide the client developer with additional information about the error | 




### <a name="o_auth_provider_error"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProviderError") OAuthProviderError



> OAuth 2 Authorization error codes




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `invalid_request` | The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed. | 
| `invalid_client` | Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method). | 
| `invalid_grant` | The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client. | 
| `unauthorized_client` | The authenticated client is not authorized to use this authorization grant type. | 
| `unsupported_grant_type` | The authorization grant type is not supported by the authorization server. | 
| `invalid_scope` | The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner. | 




### <a name="o_auth_token"></a>![Model: ](https://apidocs.io/img/method.png "OAuthToken") OAuthToken



> OAuth 2 Authorization endpoint response




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| access_token | [string](#api_types) |  ``` Required ```  | Access token | 
| token_type | [string](#api_types) |  ``` Required ```  | Type of access token | 
| expires_in | [long](#api_types) |  ``` Optional ```  | Time in seconds before the access token expires | 
| scope | [string](#api_types) |  ``` Optional ```  | List of scopes granted<br>This is a space-delimited list of strings. | 
| expiry | [long](#api_types) |  ``` Optional ```  | Time of token expiry as unix timestamp (UTC) | 
| refresh_token | [string](#api_types) |  ``` Optional ```  | Refresh token<br>Used to get a new access token when it expires. | 




### <a name="o_auth_provider"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProvider") OAuthProvider



> OAuth 2 Authorization endpoint exception




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| error | [OAuthProviderError](#o_auth_provider_error) |  ``` Required ```  | Error code | 
| error_description | [string](#api_types) |  ``` Optional ```  | Human-readable text providing additional information on error.<br>Used to assist the client developer in understanding the error that occurred. | 
| error_uri | [string](#api_types) |  ``` Optional ```  | A URI identifying a human-readable web page with information about the error, used to provide the client developer with additional information about the error | 




### <a name="o_auth_provider_error"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProviderError") OAuthProviderError



> OAuth 2 Authorization error codes




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `invalid_request` | The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed. | 
| `invalid_client` | Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method). | 
| `invalid_grant` | The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client. | 
| `unauthorized_client` | The authenticated client is not authorized to use this authorization grant type. | 
| `unsupported_grant_type` | The authorization grant type is not supported by the authorization server. | 
| `invalid_scope` | The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner. | 




### <a name="o_auth_token"></a>![Model: ](https://apidocs.io/img/method.png "OAuthToken") OAuthToken



> OAuth 2 Authorization endpoint response




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| access_token | [string](#api_types) |  ``` Required ```  | Access token | 
| token_type | [string](#api_types) |  ``` Required ```  | Type of access token | 
| expires_in | [long](#api_types) |  ``` Optional ```  | Time in seconds before the access token expires | 
| scope | [string](#api_types) |  ``` Optional ```  | List of scopes granted<br>This is a space-delimited list of strings. | 
| expiry | [long](#api_types) |  ``` Optional ```  | Time of token expiry as unix timestamp (UTC) | 
| refresh_token | [string](#api_types) |  ``` Optional ```  | Refresh token<br>Used to get a new access token when it expires. | 




### <a name="o_auth_provider"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProvider") OAuthProvider



> OAuth 2 Authorization endpoint exception




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| error | [OAuthProviderError](#o_auth_provider_error) |  ``` Required ```  | Error code | 
| error_description | [string](#api_types) |  ``` Optional ```  | Human-readable text providing additional information on error.<br>Used to assist the client developer in understanding the error that occurred. | 
| error_uri | [string](#api_types) |  ``` Optional ```  | A URI identifying a human-readable web page with information about the error, used to provide the client developer with additional information about the error | 




### <a name="o_auth_provider_error"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProviderError") OAuthProviderError



> OAuth 2 Authorization error codes




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `invalid_request` | The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed. | 
| `invalid_client` | Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method). | 
| `invalid_grant` | The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client. | 
| `unauthorized_client` | The authenticated client is not authorized to use this authorization grant type. | 
| `unsupported_grant_type` | The authorization grant type is not supported by the authorization server. | 
| `invalid_scope` | The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner. | 




### <a name="o_auth_token"></a>![Model: ](https://apidocs.io/img/method.png "OAuthToken") OAuthToken



> OAuth 2 Authorization endpoint response




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| access_token | [string](#api_types) |  ``` Required ```  | Access token | 
| token_type | [string](#api_types) |  ``` Required ```  | Type of access token | 
| expires_in | [long](#api_types) |  ``` Optional ```  | Time in seconds before the access token expires | 
| scope | [string](#api_types) |  ``` Optional ```  | List of scopes granted<br>This is a space-delimited list of strings. | 
| expiry | [long](#api_types) |  ``` Optional ```  | Time of token expiry as unix timestamp (UTC) | 
| refresh_token | [string](#api_types) |  ``` Optional ```  | Refresh token<br>Used to get a new access token when it expires. | 




### <a name="o_auth_provider"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProvider") OAuthProvider



> OAuth 2 Authorization endpoint exception




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| error | [OAuthProviderError](#o_auth_provider_error) |  ``` Required ```  | Error code | 
| error_description | [string](#api_types) |  ``` Optional ```  | Human-readable text providing additional information on error.<br>Used to assist the client developer in understanding the error that occurred. | 
| error_uri | [string](#api_types) |  ``` Optional ```  | A URI identifying a human-readable web page with information about the error, used to provide the client developer with additional information about the error | 




### <a name="o_auth_provider_error"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProviderError") OAuthProviderError



> OAuth 2 Authorization error codes




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `invalid_request` | The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed. | 
| `invalid_client` | Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method). | 
| `invalid_grant` | The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client. | 
| `unauthorized_client` | The authenticated client is not authorized to use this authorization grant type. | 
| `unsupported_grant_type` | The authorization grant type is not supported by the authorization server. | 
| `invalid_scope` | The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner. | 




### <a name="o_auth_token"></a>![Model: ](https://apidocs.io/img/method.png "OAuthToken") OAuthToken



> OAuth 2 Authorization endpoint response




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| access_token | [string](#api_types) |  ``` Required ```  | Access token | 
| token_type | [string](#api_types) |  ``` Required ```  | Type of access token | 
| expires_in | [long](#api_types) |  ``` Optional ```  | Time in seconds before the access token expires | 
| scope | [string](#api_types) |  ``` Optional ```  | List of scopes granted<br>This is a space-delimited list of strings. | 
| expiry | [long](#api_types) |  ``` Optional ```  | Time of token expiry as unix timestamp (UTC) | 
| refresh_token | [string](#api_types) |  ``` Optional ```  | Refresh token<br>Used to get a new access token when it expires. | 




### <a name="o_auth_provider"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProvider") OAuthProvider



> OAuth 2 Authorization endpoint exception




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| error | [OAuthProviderError](#o_auth_provider_error) |  ``` Required ```  | Error code | 
| error_description | [string](#api_types) |  ``` Optional ```  | Human-readable text providing additional information on error.<br>Used to assist the client developer in understanding the error that occurred. | 
| error_uri | [string](#api_types) |  ``` Optional ```  | A URI identifying a human-readable web page with information about the error, used to provide the client developer with additional information about the error | 




### <a name="o_auth_provider_error"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProviderError") OAuthProviderError



> OAuth 2 Authorization error codes




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `invalid_request` | The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed. | 
| `invalid_client` | Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method). | 
| `invalid_grant` | The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client. | 
| `unauthorized_client` | The authenticated client is not authorized to use this authorization grant type. | 
| `unsupported_grant_type` | The authorization grant type is not supported by the authorization server. | 
| `invalid_scope` | The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner. | 




### <a name="o_auth_token"></a>![Model: ](https://apidocs.io/img/method.png "OAuthToken") OAuthToken



> OAuth 2 Authorization endpoint response




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| access_token | [string](#api_types) |  ``` Required ```  | Access token | 
| token_type | [string](#api_types) |  ``` Required ```  | Type of access token | 
| expires_in | [long](#api_types) |  ``` Optional ```  | Time in seconds before the access token expires | 
| scope | [string](#api_types) |  ``` Optional ```  | List of scopes granted<br>This is a space-delimited list of strings. | 
| expiry | [long](#api_types) |  ``` Optional ```  | Time of token expiry as unix timestamp (UTC) | 
| refresh_token | [string](#api_types) |  ``` Optional ```  | Refresh token<br>Used to get a new access token when it expires. | 




### <a name="o_auth_provider"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProvider") OAuthProvider



> OAuth 2 Authorization endpoint exception




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| error | [OAuthProviderError](#o_auth_provider_error) |  ``` Required ```  | Error code | 
| error_description | [string](#api_types) |  ``` Optional ```  | Human-readable text providing additional information on error.<br>Used to assist the client developer in understanding the error that occurred. | 
| error_uri | [string](#api_types) |  ``` Optional ```  | A URI identifying a human-readable web page with information about the error, used to provide the client developer with additional information about the error | 




### <a name="o_auth_provider_error"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProviderError") OAuthProviderError



> OAuth 2 Authorization error codes




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `invalid_request` | The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed. | 
| `invalid_client` | Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method). | 
| `invalid_grant` | The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client. | 
| `unauthorized_client` | The authenticated client is not authorized to use this authorization grant type. | 
| `unsupported_grant_type` | The authorization grant type is not supported by the authorization server. | 
| `invalid_scope` | The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner. | 




### <a name="o_auth_token"></a>![Model: ](https://apidocs.io/img/method.png "OAuthToken") OAuthToken



> OAuth 2 Authorization endpoint response




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| access_token | [string](#api_types) |  ``` Required ```  | Access token | 
| token_type | [string](#api_types) |  ``` Required ```  | Type of access token | 
| expires_in | [long](#api_types) |  ``` Optional ```  | Time in seconds before the access token expires | 
| scope | [string](#api_types) |  ``` Optional ```  | List of scopes granted<br>This is a space-delimited list of strings. | 
| expiry | [long](#api_types) |  ``` Optional ```  | Time of token expiry as unix timestamp (UTC) | 
| refresh_token | [string](#api_types) |  ``` Optional ```  | Refresh token<br>Used to get a new access token when it expires. | 




### <a name="o_auth_provider"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProvider") OAuthProvider



> OAuth 2 Authorization endpoint exception




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| error | [OAuthProviderError](#o_auth_provider_error) |  ``` Required ```  | Error code | 
| error_description | [string](#api_types) |  ``` Optional ```  | Human-readable text providing additional information on error.<br>Used to assist the client developer in understanding the error that occurred. | 
| error_uri | [string](#api_types) |  ``` Optional ```  | A URI identifying a human-readable web page with information about the error, used to provide the client developer with additional information about the error | 




### <a name="o_auth_provider_error"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProviderError") OAuthProviderError



> OAuth 2 Authorization error codes




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `invalid_request` | The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed. | 
| `invalid_client` | Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method). | 
| `invalid_grant` | The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client. | 
| `unauthorized_client` | The authenticated client is not authorized to use this authorization grant type. | 
| `unsupported_grant_type` | The authorization grant type is not supported by the authorization server. | 
| `invalid_scope` | The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner. | 




### <a name="o_auth_token"></a>![Model: ](https://apidocs.io/img/method.png "OAuthToken") OAuthToken



> OAuth 2 Authorization endpoint response




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| access_token | [string](#api_types) |  ``` Required ```  | Access token | 
| token_type | [string](#api_types) |  ``` Required ```  | Type of access token | 
| expires_in | [long](#api_types) |  ``` Optional ```  | Time in seconds before the access token expires | 
| scope | [string](#api_types) |  ``` Optional ```  | List of scopes granted<br>This is a space-delimited list of strings. | 
| expiry | [long](#api_types) |  ``` Optional ```  | Time of token expiry as unix timestamp (UTC) | 
| refresh_token | [string](#api_types) |  ``` Optional ```  | Refresh token<br>Used to get a new access token when it expires. | 




### <a name="o_auth_provider"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProvider") OAuthProvider



> OAuth 2 Authorization endpoint exception




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| error | [OAuthProviderError](#o_auth_provider_error) |  ``` Required ```  | Error code | 
| error_description | [string](#api_types) |  ``` Optional ```  | Human-readable text providing additional information on error.<br>Used to assist the client developer in understanding the error that occurred. | 
| error_uri | [string](#api_types) |  ``` Optional ```  | A URI identifying a human-readable web page with information about the error, used to provide the client developer with additional information about the error | 




### <a name="o_auth_provider_error"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProviderError") OAuthProviderError



> OAuth 2 Authorization error codes




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `invalid_request` | The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed. | 
| `invalid_client` | Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method). | 
| `invalid_grant` | The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client. | 
| `unauthorized_client` | The authenticated client is not authorized to use this authorization grant type. | 
| `unsupported_grant_type` | The authorization grant type is not supported by the authorization server. | 
| `invalid_scope` | The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner. | 




### <a name="o_auth_token"></a>![Model: ](https://apidocs.io/img/method.png "OAuthToken") OAuthToken



> OAuth 2 Authorization endpoint response




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| access_token | [string](#api_types) |  ``` Required ```  | Access token | 
| token_type | [string](#api_types) |  ``` Required ```  | Type of access token | 
| expires_in | [long](#api_types) |  ``` Optional ```  | Time in seconds before the access token expires | 
| scope | [string](#api_types) |  ``` Optional ```  | List of scopes granted<br>This is a space-delimited list of strings. | 
| expiry | [long](#api_types) |  ``` Optional ```  | Time of token expiry as unix timestamp (UTC) | 
| refresh_token | [string](#api_types) |  ``` Optional ```  | Refresh token<br>Used to get a new access token when it expires. | 




### <a name="o_auth_provider"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProvider") OAuthProvider



> OAuth 2 Authorization endpoint exception




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| error | [OAuthProviderError](#o_auth_provider_error) |  ``` Required ```  | Error code | 
| error_description | [string](#api_types) |  ``` Optional ```  | Human-readable text providing additional information on error.<br>Used to assist the client developer in understanding the error that occurred. | 
| error_uri | [string](#api_types) |  ``` Optional ```  | A URI identifying a human-readable web page with information about the error, used to provide the client developer with additional information about the error | 




### <a name="o_auth_provider_error"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProviderError") OAuthProviderError



> OAuth 2 Authorization error codes




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `invalid_request` | The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed. | 
| `invalid_client` | Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method). | 
| `invalid_grant` | The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client. | 
| `unauthorized_client` | The authenticated client is not authorized to use this authorization grant type. | 
| `unsupported_grant_type` | The authorization grant type is not supported by the authorization server. | 
| `invalid_scope` | The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner. | 




### <a name="o_auth_token"></a>![Model: ](https://apidocs.io/img/method.png "OAuthToken") OAuthToken



> OAuth 2 Authorization endpoint response




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| access_token | [string](#api_types) |  ``` Required ```  | Access token | 
| token_type | [string](#api_types) |  ``` Required ```  | Type of access token | 
| expires_in | [long](#api_types) |  ``` Optional ```  | Time in seconds before the access token expires | 
| scope | [string](#api_types) |  ``` Optional ```  | List of scopes granted<br>This is a space-delimited list of strings. | 
| expiry | [long](#api_types) |  ``` Optional ```  | Time of token expiry as unix timestamp (UTC) | 
| refresh_token | [string](#api_types) |  ``` Optional ```  | Refresh token<br>Used to get a new access token when it expires. | 




### <a name="o_auth_provider"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProvider") OAuthProvider



> OAuth 2 Authorization endpoint exception




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| error | [OAuthProviderError](#o_auth_provider_error) |  ``` Required ```  | Error code | 
| error_description | [string](#api_types) |  ``` Optional ```  | Human-readable text providing additional information on error.<br>Used to assist the client developer in understanding the error that occurred. | 
| error_uri | [string](#api_types) |  ``` Optional ```  | A URI identifying a human-readable web page with information about the error, used to provide the client developer with additional information about the error | 




### <a name="o_auth_provider_error"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProviderError") OAuthProviderError



> OAuth 2 Authorization error codes




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `invalid_request` | The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed. | 
| `invalid_client` | Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method). | 
| `invalid_grant` | The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client. | 
| `unauthorized_client` | The authenticated client is not authorized to use this authorization grant type. | 
| `unsupported_grant_type` | The authorization grant type is not supported by the authorization server. | 
| `invalid_scope` | The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner. |

