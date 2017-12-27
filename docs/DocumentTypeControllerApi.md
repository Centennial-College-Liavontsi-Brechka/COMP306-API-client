# DocumentTypeControllerApi

All URIs are relative to *https://api-final-project-19022.appspot.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addDocumentTypeUsingPOST**](DocumentTypeControllerApi.md#addDocumentTypeUsingPOST) | **POST** /api/documentTypes | addDocumentType
[**removeDocumentTypeUsingDELETE**](DocumentTypeControllerApi.md#removeDocumentTypeUsingDELETE) | **DELETE** /api/documentTypes/{id} | removeDocumentType
[**saveDocumentTypeUsingPUT**](DocumentTypeControllerApi.md#saveDocumentTypeUsingPUT) | **PUT** /api/documentTypes/{id} | saveDocumentType
[**showDocumentTypesUsingGET**](DocumentTypeControllerApi.md#showDocumentTypesUsingGET) | **GET** /api/documentTypes | showDocumentTypes


<a name="addDocumentTypeUsingPOST"></a>
# **addDocumentTypeUsingPOST**
> addDocumentTypeUsingPOST(documentType)

addDocumentType

### Example
```java
// Import classes:
//import net.liavontsibrechka.invoker.ApiException;
//import net.liavontsibrechka.api.DocumentTypeControllerApi;


DocumentTypeControllerApi apiInstance = new DocumentTypeControllerApi();
DocumentType documentType = new DocumentType(); // DocumentType | documentType
try {
    apiInstance.addDocumentTypeUsingPOST(documentType);
} catch (ApiException e) {
    System.err.println("Exception when calling DocumentTypeControllerApi#addDocumentTypeUsingPOST");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **documentType** | [**DocumentType**](DocumentType.md)| documentType |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

<a name="removeDocumentTypeUsingDELETE"></a>
# **removeDocumentTypeUsingDELETE**
> removeDocumentTypeUsingDELETE(id)

removeDocumentType

### Example
```java
// Import classes:
//import net.liavontsibrechka.invoker.ApiException;
//import net.liavontsibrechka.api.DocumentTypeControllerApi;


DocumentTypeControllerApi apiInstance = new DocumentTypeControllerApi();
Long id = 789L; // Long | id
try {
    apiInstance.removeDocumentTypeUsingDELETE(id);
} catch (ApiException e) {
    System.err.println("Exception when calling DocumentTypeControllerApi#removeDocumentTypeUsingDELETE");
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

<a name="saveDocumentTypeUsingPUT"></a>
# **saveDocumentTypeUsingPUT**
> saveDocumentTypeUsingPUT(id, documentType)

saveDocumentType

### Example
```java
// Import classes:
//import net.liavontsibrechka.invoker.ApiException;
//import net.liavontsibrechka.api.DocumentTypeControllerApi;


DocumentTypeControllerApi apiInstance = new DocumentTypeControllerApi();
Long id = 789L; // Long | id
DocumentType documentType = new DocumentType(); // DocumentType | documentType
try {
    apiInstance.saveDocumentTypeUsingPUT(id, documentType);
} catch (ApiException e) {
    System.err.println("Exception when calling DocumentTypeControllerApi#saveDocumentTypeUsingPUT");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Long**| id |
 **documentType** | [**DocumentType**](DocumentType.md)| documentType |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

<a name="showDocumentTypesUsingGET"></a>
# **showDocumentTypesUsingGET**
> List&lt;DocumentType&gt; showDocumentTypesUsingGET()

showDocumentTypes

### Example
```java
// Import classes:
//import net.liavontsibrechka.invoker.ApiException;
//import net.liavontsibrechka.api.DocumentTypeControllerApi;


DocumentTypeControllerApi apiInstance = new DocumentTypeControllerApi();
try {
    List<DocumentType> result = apiInstance.showDocumentTypesUsingGET();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DocumentTypeControllerApi#showDocumentTypesUsingGET");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**List&lt;DocumentType&gt;**](DocumentType.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

