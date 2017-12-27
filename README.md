# info-cloud-client

## Requirements

Building the API client library requires [Maven](https://maven.apache.org/) to be installed.

## Installation

To install the API client library to your local Maven repository, simply execute:

```shell
mvn install
```

To deploy it to a remote Maven repository instead, configure the settings of the repository and execute:

```shell
mvn deploy
```

Refer to the [official documentation](https://maven.apache.org/plugins/maven-deploy-plugin/usage.html) for more information.

### Maven users

Add this dependency to your project's POM:

```xml
<dependency>
    <groupId>net.liavontsibrechka</groupId>
    <artifactId>info-cloud-client</artifactId>
    <version>1.0.0-SNAPSHOT</version>
    <scope>compile</scope>
</dependency>
```

### Gradle users

Add this dependency to your project's build file:

```groovy
compile "net.liavontsibrechka:info-cloud-client:1.0.0-SNAPSHOT"
```

### Others

At first generate the JAR by executing:

    mvn package

Then manually install the following JARs:

* target/info-cloud-client-1.0.0-SNAPSHOT.jar
* target/lib/*.jar

## Getting Started

Please follow the [installation](#installation) instruction and execute the following Java code:

```java

import net.liavontsibrechka.invoker.*;
import net.liavontsibrechka.invoker.auth.*;
import net.liavontsibrechka.model.*;
import net.liavontsibrechka.api.AuthenticationControllerApi;

import java.io.File;
import java.util.*;

public class AuthenticationControllerApiExample {

    public static void main(String[] args) {
        
        AuthenticationControllerApi apiInstance = new AuthenticationControllerApi();
        Credentials credentials = new Credentials(); // Credentials | credentials
        try {
            apiInstance.loginUsingPOST(credentials);
        } catch (ApiException e) {
            System.err.println("Exception when calling AuthenticationControllerApi#loginUsingPOST");
            e.printStackTrace();
        }
    }
}

```

## Documentation for API Endpoints

All URIs are relative to *https://api-final-project-19022.appspot.com*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AuthenticationControllerApi* | [**loginUsingPOST**](docs/AuthenticationControllerApi.md#loginUsingPOST) | **POST** /api/auth/login | login
*AuthenticationControllerApi* | [**refreshTokenUsingGET**](docs/AuthenticationControllerApi.md#refreshTokenUsingGET) | **GET** /api/auth/token | refreshToken
*AuthenticationControllerApi* | [**registerUserUsingPOST**](docs/AuthenticationControllerApi.md#registerUserUsingPOST) | **POST** /api/auth/register | registerUser
*BasicErrorControllerApi* | [**errorUsingDELETE**](docs/BasicErrorControllerApi.md#errorUsingDELETE) | **DELETE** /error | error
*BasicErrorControllerApi* | [**errorUsingGET**](docs/BasicErrorControllerApi.md#errorUsingGET) | **GET** /error | error
*BasicErrorControllerApi* | [**errorUsingHEAD**](docs/BasicErrorControllerApi.md#errorUsingHEAD) | **HEAD** /error | error
*BasicErrorControllerApi* | [**errorUsingOPTIONS**](docs/BasicErrorControllerApi.md#errorUsingOPTIONS) | **OPTIONS** /error | error
*BasicErrorControllerApi* | [**errorUsingPATCH**](docs/BasicErrorControllerApi.md#errorUsingPATCH) | **PATCH** /error | error
*BasicErrorControllerApi* | [**errorUsingPOST**](docs/BasicErrorControllerApi.md#errorUsingPOST) | **POST** /error | error
*BasicErrorControllerApi* | [**errorUsingPUT**](docs/BasicErrorControllerApi.md#errorUsingPUT) | **PUT** /error | error
*CategoryControllerApi* | [**addCategoryUsingPOST**](docs/CategoryControllerApi.md#addCategoryUsingPOST) | **POST** /api/categories | addCategory
*CategoryControllerApi* | [**removeCategoryUsingDELETE**](docs/CategoryControllerApi.md#removeCategoryUsingDELETE) | **DELETE** /api/categories/{id} | removeCategory
*CategoryControllerApi* | [**saveCategoryUsingPUT**](docs/CategoryControllerApi.md#saveCategoryUsingPUT) | **PUT** /api/categories/{id} | saveCategory
*CategoryControllerApi* | [**showCategoriesUsingGET**](docs/CategoryControllerApi.md#showCategoriesUsingGET) | **GET** /api/categories | showCategories
*DocumentControllerApi* | [**getFileUsingGET**](docs/DocumentControllerApi.md#getFileUsingGET) | **GET** /api/documents/download/{id} | getFile
*DocumentControllerApi* | [**removeDocumentUsingDELETE**](docs/DocumentControllerApi.md#removeDocumentUsingDELETE) | **DELETE** /api/documents/{id} | removeDocument
*DocumentControllerApi* | [**saveNewDocumentUsingPOST**](docs/DocumentControllerApi.md#saveNewDocumentUsingPOST) | **POST** /api/documents | saveNewDocument
*DocumentControllerApi* | [**showDocumentByIdUsingGET**](docs/DocumentControllerApi.md#showDocumentByIdUsingGET) | **GET** /api/documents/{id} | showDocumentById
*DocumentControllerApi* | [**showDocumentListUsingGET**](docs/DocumentControllerApi.md#showDocumentListUsingGET) | **GET** /api/documents | showDocumentList
*DocumentControllerApi* | [**updateDocumentUsingPUT**](docs/DocumentControllerApi.md#updateDocumentUsingPUT) | **PUT** /api/documents | updateDocument
*DocumentTypeControllerApi* | [**addDocumentTypeUsingPOST**](docs/DocumentTypeControllerApi.md#addDocumentTypeUsingPOST) | **POST** /api/documentTypes | addDocumentType
*DocumentTypeControllerApi* | [**removeDocumentTypeUsingDELETE**](docs/DocumentTypeControllerApi.md#removeDocumentTypeUsingDELETE) | **DELETE** /api/documentTypes/{id} | removeDocumentType
*DocumentTypeControllerApi* | [**saveDocumentTypeUsingPUT**](docs/DocumentTypeControllerApi.md#saveDocumentTypeUsingPUT) | **PUT** /api/documentTypes/{id} | saveDocumentType
*DocumentTypeControllerApi* | [**showDocumentTypesUsingGET**](docs/DocumentTypeControllerApi.md#showDocumentTypesUsingGET) | **GET** /api/documentTypes | showDocumentTypes
*TagControllerApi* | [**addTagUsingPOST**](docs/TagControllerApi.md#addTagUsingPOST) | **POST** /api/tags | addTag
*TagControllerApi* | [**removeTagUsingDELETE**](docs/TagControllerApi.md#removeTagUsingDELETE) | **DELETE** /api/tags/{id} | removeTag
*TagControllerApi* | [**saveTagUsingPUT**](docs/TagControllerApi.md#saveTagUsingPUT) | **PUT** /api/tags/{id} | saveTag
*TagControllerApi* | [**saveTagsUsingPUT**](docs/TagControllerApi.md#saveTagsUsingPUT) | **PUT** /api/tags | saveTags
*TagControllerApi* | [**showTagsUsingGET**](docs/TagControllerApi.md#showTagsUsingGET) | **GET** /api/tags | showTags


## Documentation for Models

 - [Category](docs/Category.md)
 - [Credentials](docs/Credentials.md)
 - [Document](docs/Document.md)
 - [DocumentType](docs/DocumentType.md)
 - [JwtToken](docs/JwtToken.md)
 - [ModelAndView](docs/ModelAndView.md)
 - [Tag](docs/Tag.md)
 - [User](docs/User.md)
 - [UserRole](docs/UserRole.md)
 - [View](docs/View.md)


## Documentation for Authorization

All endpoints do not require authorization.
Authentication schemes defined for the API:

## Recommendation

It's recommended to create an instance of `ApiClient` per thread in a multithreaded environment to avoid any potential issues.

## Author



