# CategoryControllerApi

All URIs are relative to *https://api-final-project-19022.appspot.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addCategoryUsingPOST**](CategoryControllerApi.md#addCategoryUsingPOST) | **POST** /api/categories | addCategory
[**removeCategoryUsingDELETE**](CategoryControllerApi.md#removeCategoryUsingDELETE) | **DELETE** /api/categories/{id} | removeCategory
[**saveCategoryUsingPUT**](CategoryControllerApi.md#saveCategoryUsingPUT) | **PUT** /api/categories/{id} | saveCategory
[**showCategoriesUsingGET**](CategoryControllerApi.md#showCategoriesUsingGET) | **GET** /api/categories | showCategories


<a name="addCategoryUsingPOST"></a>
# **addCategoryUsingPOST**
> addCategoryUsingPOST(category)

addCategory

### Example
```java
// Import classes:
//import net.liavontsibrechka.invoker.ApiException;
//import net.liavontsibrechka.api.CategoryControllerApi;


CategoryControllerApi apiInstance = new CategoryControllerApi();
Category category = new Category(); // Category | category
try {
    apiInstance.addCategoryUsingPOST(category);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryControllerApi#addCategoryUsingPOST");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **category** | [**Category**](Category.md)| category |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

<a name="removeCategoryUsingDELETE"></a>
# **removeCategoryUsingDELETE**
> removeCategoryUsingDELETE(id)

removeCategory

### Example
```java
// Import classes:
//import net.liavontsibrechka.invoker.ApiException;
//import net.liavontsibrechka.api.CategoryControllerApi;


CategoryControllerApi apiInstance = new CategoryControllerApi();
Long id = 789L; // Long | id
try {
    apiInstance.removeCategoryUsingDELETE(id);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryControllerApi#removeCategoryUsingDELETE");
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

<a name="saveCategoryUsingPUT"></a>
# **saveCategoryUsingPUT**
> saveCategoryUsingPUT(id, category)

saveCategory

### Example
```java
// Import classes:
//import net.liavontsibrechka.invoker.ApiException;
//import net.liavontsibrechka.api.CategoryControllerApi;


CategoryControllerApi apiInstance = new CategoryControllerApi();
Long id = 789L; // Long | id
Category category = new Category(); // Category | category
try {
    apiInstance.saveCategoryUsingPUT(id, category);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryControllerApi#saveCategoryUsingPUT");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Long**| id |
 **category** | [**Category**](Category.md)| category |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

<a name="showCategoriesUsingGET"></a>
# **showCategoriesUsingGET**
> List&lt;Category&gt; showCategoriesUsingGET()

showCategories

### Example
```java
// Import classes:
//import net.liavontsibrechka.invoker.ApiException;
//import net.liavontsibrechka.api.CategoryControllerApi;


CategoryControllerApi apiInstance = new CategoryControllerApi();
try {
    List<Category> result = apiInstance.showCategoriesUsingGET();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryControllerApi#showCategoriesUsingGET");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**List&lt;Category&gt;**](Category.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

