# OpenAPI\Client\SirenApi

All URIs are relative to http://localhost:8080/api.

Method | HTTP request | Description
------------- | ------------- | -------------
[**getMode()**](SirenApi.md#getMode) | **GET** /siren/mode | get the mode of the siren (noisy, quiet)
[**playSiren()**](SirenApi.md#playSiren) | **HEAD** /siren | Play the siren sound
[**toggleMode()**](SirenApi.md#toggleMode) | **HEAD** /siren/mode | set the mode of the siren (noisy, quiet)


## `getMode()`

```php
getMode(): bool
```

get the mode of the siren (noisy, quiet)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new OpenAPI\Client\Api\SirenApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->getMode();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SirenApi->getMode: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

**bool**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `playSiren()`

```php
playSiren($siren_type)
```

Play the siren sound

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new OpenAPI\Client\Api\SirenApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$siren_type = 'siren_type_example'; // string | The type of siren

try {
    $apiInstance->playSiren($siren_type);
} catch (Exception $e) {
    echo 'Exception when calling SirenApi->playSiren: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **siren_type** | **string**| The type of siren |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `toggleMode()`

```php
toggleMode()
```

set the mode of the siren (noisy, quiet)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new OpenAPI\Client\Api\SirenApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->toggleMode();
} catch (Exception $e) {
    echo 'Exception when calling SirenApi->toggleMode: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
