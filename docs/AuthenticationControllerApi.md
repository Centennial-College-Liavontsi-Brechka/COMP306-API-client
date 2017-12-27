# AuthenticationControllerApi

All URIs are relative to *https://api-final-project-19022.appspot.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**loginUsingPOST**](AuthenticationControllerApi.md#loginUsingPOST) | **POST** /api/auth/login | login
[**refreshTokenUsingGET**](AuthenticationControllerApi.md#refreshTokenUsingGET) | **GET** /api/auth/token | refreshToken
[**registerUserUsingPOST**](AuthenticationControllerApi.md#registerUserUsingPOST) | **POST** /api/auth/register | registerUser


<a name="loginUsingPOST"></a>
# **loginUsingPOST**
> loginUsingPOST(credentials)

login

### Example
```java
// Import classes:
//import net.liavontsibrechka.invoker.ApiException;
//import net.liavontsibrechka.api.AuthenticationControllerApi;


AuthenticationControllerApi apiInstance = new AuthenticationControllerApi();
Credentials credentials = new Credentials(); // Credentials | credentials
try {
    apiInstance.loginUsingPOST(credentials);
} catch (ApiException e) {
    System.err.println("Exception when calling AuthenticationControllerApi#loginUsingPOST");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **credentials** | [**Credentials**](Credentials.md)| credentials |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

<a name="refreshTokenUsingGET"></a>
# **refreshTokenUsingGET**
> JwtToken refreshTokenUsingGET()

refreshToken

### Example
```java
// Import classes:
//import net.liavontsibrechka.invoker.ApiException;
//import net.liavontsibrechka.api.AuthenticationControllerApi;


AuthenticationControllerApi apiInstance = new AuthenticationControllerApi();
try {
    JwtToken result = apiInstance.refreshTokenUsingGET();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AuthenticationControllerApi#refreshTokenUsingGET");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**JwtToken**](JwtToken.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

<a name="registerUserUsingPOST"></a>
# **registerUserUsingPOST**
> registerUserUsingPOST(user)

registerUser

### Example
```java
// Import classes:
//import net.liavontsibrechka.invoker.ApiException;
//import net.liavontsibrechka.api.AuthenticationControllerApi;


AuthenticationControllerApi apiInstance = new AuthenticationControllerApi();
User user = new User(); // User | user
try {
    apiInstance.registerUserUsingPOST(user);
} catch (ApiException e) {
    System.err.println("Exception when calling AuthenticationControllerApi#registerUserUsingPOST");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user** | [**User**](User.md)| user |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

