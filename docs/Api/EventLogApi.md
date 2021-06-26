# OpenAPI\Client\EventLogApi

All URIs are relative to http://localhost:8080/api.

Method | HTTP request | Description
------------- | ------------- | -------------
[**deleteEvents()**](EventLogApi.md#deleteEvents) | **DELETE** /eventLog | Delete list of events
[**getEvents()**](EventLogApi.md#getEvents) | **GET** /eventLog/events | Get list of events


## `deleteEvents()`

```php
deleteEvents()
```

Delete list of events

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new OpenAPI\Client\Api\EventLogApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->deleteEvents();
} catch (Exception $e) {
    echo 'Exception when calling EventLogApi->deleteEvents: ', $e->getMessage(), PHP_EOL;
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

## `getEvents()`

```php
getEvents(): \OpenAPI\Client\Model\Event[]
```

Get list of events

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new OpenAPI\Client\Api\EventLogApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->getEvents();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EventLogApi->getEvents: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\OpenAPI\Client\Model\Event[]**](../Model/Event.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
