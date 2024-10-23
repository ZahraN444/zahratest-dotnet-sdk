
# Getting Started with Cypress Test API

## Introduction

This is a sample API to demonstrate an OpenAPI spec with multiple endpoints and a custom model.

## Install the Package

If you are building with .NET CLI tools then you can also use the following command:

```bash
dotnet add package ZahratestSDK --version 2.3.4
```

You can also view the package at:
https://www.nuget.org/packages/ZahratestSDK/2.3.4

## Test the SDK

The generated SDK also contain one or more Tests, which are contained in the Tests project. In order to invoke these test cases, you will need `NUnit 3.0 Test Adapter Extension` for Visual Studio. Once the SDK is complied, the test cases should appear in the Test Explorer window. Here, you can click `Run All` to execute these test cases.

## Initialize the API Client

**_Note:_** Documentation for the client can be found [here.](https://www.github.com/ZahraN444/zahratest-dotnet-sdk/tree/2.3.4/doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| `DefaultHost` | `string` | *Default*: `"www.example.com"` |
| `Environment` | `Environment` | The API environment. <br> **Default: `Environment.Production`** |
| `Timeout` | `TimeSpan` | Http client timeout.<br>*Default*: `TimeSpan.FromSeconds(100)` |

The API client can be initialized as follows:

```csharp
CypressTestAPIClient client = new CypressTestAPIClient.Builder()
    .Environment(CypressTestAPI.Standard.Environment.Production)
    .DefaultHost("www.example.com")
    .Build();
```

## List of APIs

* [API](https://www.github.com/ZahraN444/zahratest-dotnet-sdk/tree/2.3.4/doc/controllers/api.md)

## Classes Documentation

* [Utility Classes](https://www.github.com/ZahraN444/zahratest-dotnet-sdk/tree/2.3.4/doc/utility-classes.md)
* [HttpRequest](https://www.github.com/ZahraN444/zahratest-dotnet-sdk/tree/2.3.4/doc/http-request.md)
* [HttpResponse](https://www.github.com/ZahraN444/zahratest-dotnet-sdk/tree/2.3.4/doc/http-response.md)
* [HttpStringResponse](https://www.github.com/ZahraN444/zahratest-dotnet-sdk/tree/2.3.4/doc/http-string-response.md)
* [HttpContext](https://www.github.com/ZahraN444/zahratest-dotnet-sdk/tree/2.3.4/doc/http-context.md)
* [HttpClientConfiguration](https://www.github.com/ZahraN444/zahratest-dotnet-sdk/tree/2.3.4/doc/http-client-configuration.md)
* [HttpClientConfiguration Builder](https://www.github.com/ZahraN444/zahratest-dotnet-sdk/tree/2.3.4/doc/http-client-configuration-builder.md)
* [IAuthManager](https://www.github.com/ZahraN444/zahratest-dotnet-sdk/tree/2.3.4/doc/i-auth-manager.md)
* [ApiException](https://www.github.com/ZahraN444/zahratest-dotnet-sdk/tree/2.3.4/doc/api-exception.md)

