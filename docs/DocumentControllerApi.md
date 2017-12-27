# DocumentControllerApi

All URIs are relative to *https://api-final-project-19022.appspot.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getFileUsingGET**](DocumentControllerApi.md#getFileUsingGET) | **GET** /api/documents/download/{id} | getFile
[**removeDocumentUsingDELETE**](DocumentControllerApi.md#removeDocumentUsingDELETE) | **DELETE** /api/documents/{id} | removeDocument
[**saveNewDocumentUsingPOST**](DocumentControllerApi.md#saveNewDocumentUsingPOST) | **POST** /api/documents | saveNewDocument
[**showDocumentByIdUsingGET**](DocumentControllerApi.md#showDocumentByIdUsingGET) | **GET** /api/documents/{id} | showDocumentById
[**showDocumentListUsingGET**](DocumentControllerApi.md#showDocumentListUsingGET) | **GET** /api/documents | showDocumentList
[**updateDocumentUsingPUT**](DocumentControllerApi.md#updateDocumentUsingPUT) | **PUT** /api/documents | updateDocument


<a name="getFileUsingGET"></a>
# **getFileUsingGET**
> getFileUsingGET(id)

getFile

### Example
```java
// Import classes:
//import net.liavontsibrechka.invoker.ApiException;
//import net.liavontsibrechka.api.DocumentControllerApi;


DocumentControllerApi apiInstance = new DocumentControllerApi();
Long id = 789L; // Long | id
try {
    apiInstance.getFileUsingGET(id);
} catch (ApiException e) {
    System.err.println("Exception when calling DocumentControllerApi#getFileUsingGET");
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

<a name="removeDocumentUsingDELETE"></a>
# **removeDocumentUsingDELETE**
> removeDocumentUsingDELETE(id)

removeDocument

### Example
```java
// Import classes:
//import net.liavontsibrechka.invoker.ApiException;
//import net.liavontsibrechka.api.DocumentControllerApi;


DocumentControllerApi apiInstance = new DocumentControllerApi();
Long id = 789L; // Long | id
try {
    apiInstance.removeDocumentUsingDELETE(id);
} catch (ApiException e) {
    System.err.println("Exception when calling DocumentControllerApi#removeDocumentUsingDELETE");
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

<a name="saveNewDocumentUsingPOST"></a>
# **saveNewDocumentUsingPOST**
> saveNewDocumentUsingPOST(properties, file)

saveNewDocument

### Example
```java
// Import classes:
//import net.liavontsibrechka.invoker.ApiException;
//import net.liavontsibrechka.api.DocumentControllerApi;


DocumentControllerApi apiInstance = new DocumentControllerApi();
String properties = "properties_example"; // String | properties
File file = new File("/path/to/file.txt"); // File | file
try {
    apiInstance.saveNewDocumentUsingPOST(properties, file);
} catch (ApiException e) {
    System.err.println("Exception when calling DocumentControllerApi#saveNewDocumentUsingPOST");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **properties** | **String**| properties |
 **file** | **File**| file |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: */*

<a name="showDocumentByIdUsingGET"></a>
# **showDocumentByIdUsingGET**
> Document showDocumentByIdUsingGET(id)

showDocumentById

### Example
```java
// Import classes:
//import net.liavontsibrechka.invoker.ApiException;
//import net.liavontsibrechka.api.DocumentControllerApi;


DocumentControllerApi apiInstance = new DocumentControllerApi();
Long id = 789L; // Long | id
try {
    Document result = apiInstance.showDocumentByIdUsingGET(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DocumentControllerApi#showDocumentByIdUsingGET");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Long**| id |

### Return type

[**Document**](Document.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

<a name="showDocumentListUsingGET"></a>
# **showDocumentListUsingGET**
> List&lt;Document&gt; showDocumentListUsingGET(postedBy, category, documentType, sortBy, sortAsc, skip, limit)

showDocumentList

### Example
```java
// Import classes:
//import net.liavontsibrechka.invoker.ApiException;
//import net.liavontsibrechka.api.DocumentControllerApi;


DocumentControllerApi apiInstance = new DocumentControllerApi();
String postedBy = "postedBy_example"; // String | postedBy
String category = "category_example"; // String | category
String documentType = "documentType_example"; // String | documentType
String sortBy = "sortBy_example"; // String | sortBy
Boolean sortAsc = true; // Boolean | sortAsc
Integer skip = 56; // Integer | skip
Integer limit = 56; // Integer | limit
try {
    List<Document> result = apiInstance.showDocumentListUsingGET(postedBy, category, documentType, sortBy, sortAsc, skip, limit);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DocumentControllerApi#showDocumentListUsingGET");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **postedBy** | **String**| postedBy | [optional]
 **category** | **String**| category | [optional]
 **documentType** | **String**| documentType | [optional]
 **sortBy** | **String**| sortBy | [optional]
 **sortAsc** | **Boolean**| sortAsc | [optional]
 **skip** | **Integer**| skip | [optional]
 **limit** | **Integer**| limit | [optional]

### Return type

[**List&lt;Document&gt;**](Document.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

<a name="updateDocumentUsingPUT"></a>
# **updateDocumentUsingPUT**
> updateDocumentUsingPUT(properties, id, file)

updateDocument

### Example
```java
// Import classes:
//import net.liavontsibrechka.invoker.ApiException;
//import net.liavontsibrechka.api.DocumentControllerApi;


DocumentControllerApi apiInstance = new DocumentControllerApi();
String properties = "properties_example"; // String | properties
String id = "id_example"; // String | id
File file = new File("/path/to/file.txt"); // File | file
try {
    apiInstance.updateDocumentUsingPUT(properties, id, file);
} catch (ApiException e) {
    System.err.println("Exception when calling DocumentControllerApi#updateDocumentUsingPUT");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **properties** | **String**| properties |
 **id** | **String**| id |
 **file** | **File**| file |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: */*

