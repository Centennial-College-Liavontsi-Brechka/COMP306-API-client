# TagControllerApi

All URIs are relative to *https://api-final-project-19022.appspot.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addTagUsingPOST**](TagControllerApi.md#addTagUsingPOST) | **POST** /api/tags | addTag
[**removeTagUsingDELETE**](TagControllerApi.md#removeTagUsingDELETE) | **DELETE** /api/tags/{id} | removeTag
[**saveTagUsingPUT**](TagControllerApi.md#saveTagUsingPUT) | **PUT** /api/tags/{id} | saveTag
[**saveTagsUsingPUT**](TagControllerApi.md#saveTagsUsingPUT) | **PUT** /api/tags | saveTags
[**showTagsUsingGET**](TagControllerApi.md#showTagsUsingGET) | **GET** /api/tags | showTags


<a name="addTagUsingPOST"></a>
# **addTagUsingPOST**
> addTagUsingPOST(tag)

addTag

### Example
```java
// Import classes:
//import net.liavontsibrechka.invoker.ApiException;
//import net.liavontsibrechka.api.TagControllerApi;


TagControllerApi apiInstance = new TagControllerApi();
Tag tag = new Tag(); // Tag | tag
try {
    apiInstance.addTagUsingPOST(tag);
} catch (ApiException e) {
    System.err.println("Exception when calling TagControllerApi#addTagUsingPOST");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tag** | [**Tag**](Tag.md)| tag |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

<a name="removeTagUsingDELETE"></a>
# **removeTagUsingDELETE**
> removeTagUsingDELETE(id)

removeTag

### Example
```java
// Import classes:
//import net.liavontsibrechka.invoker.ApiException;
//import net.liavontsibrechka.api.TagControllerApi;


TagControllerApi apiInstance = new TagControllerApi();
Long id = 789L; // Long | id
try {
    apiInstance.removeTagUsingDELETE(id);
} catch (ApiException e) {
    System.err.println("Exception when calling TagControllerApi#removeTagUsingDELETE");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Long**| id |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

<a name="saveTagUsingPUT"></a>
# **saveTagUsingPUT**
> saveTagUsingPUT(id, tag)

saveTag

### Example
```java
// Import classes:
//import net.liavontsibrechka.invoker.ApiException;
//import net.liavontsibrechka.api.TagControllerApi;


TagControllerApi apiInstance = new TagControllerApi();
Long id = 789L; // Long | id
Tag tag = new Tag(); // Tag | tag
try {
    apiInstance.saveTagUsingPUT(id, tag);
} catch (ApiException e) {
    System.err.println("Exception when calling TagControllerApi#saveTagUsingPUT");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Long**| id |
 **tag** | [**Tag**](Tag.md)| tag |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

<a name="saveTagsUsingPUT"></a>
# **saveTagsUsingPUT**
> saveTagsUsingPUT(tags)

saveTags

### Example
```java
// Import classes:
//import net.liavontsibrechka.invoker.ApiException;
//import net.liavontsibrechka.api.TagControllerApi;


TagControllerApi apiInstance = new TagControllerApi();
List<Tag> tags = Arrays.asList(new Tag()); // List<Tag> | tags
try {
    apiInstance.saveTagsUsingPUT(tags);
} catch (ApiException e) {
    System.err.println("Exception when calling TagControllerApi#saveTagsUsingPUT");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tags** | [**List&lt;Tag&gt;**](Tag.md)| tags |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

<a name="showTagsUsingGET"></a>
# **showTagsUsingGET**
> List&lt;Tag&gt; showTagsUsingGET(search, skip, limit)

showTags

### Example
```java
// Import classes:
//import net.liavontsibrechka.invoker.ApiException;
//import net.liavontsibrechka.api.TagControllerApi;


TagControllerApi apiInstance = new TagControllerApi();
String search = "search_example"; // String | search
Integer skip = 56; // Integer | skip
Integer limit = 56; // Integer | limit
try {
    List<Tag> result = apiInstance.showTagsUsingGET(search, skip, limit);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TagControllerApi#showTagsUsingGET");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **search** | **String**| search | [optional]
 **skip** | **Integer**| skip | [optional]
 **limit** | **Integer**| limit | [optional]

### Return type

[**List&lt;Tag&gt;**](Tag.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

