# Swagger\Client\OrderPosApi

All URIs are relative to *https://my.sevdesk.de/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**deleteOrderPos**](OrderPosApi.md#deleteorderpos) | **DELETE** /OrderPos/{orderPosId} | Deletes an order Position
[**getOrderPositionById**](OrderPosApi.md#getorderpositionbyid) | **GET** /OrderPos/{orderPosId} | Find order position by ID
[**getOrderPositions**](OrderPosApi.md#getorderpositions) | **GET** /OrderPos | Retrieve order positions
[**updateOrderPosition**](OrderPosApi.md#updateorderposition) | **PUT** /OrderPos/{orderPosId} | Update an existing order position

# **deleteOrderPos**
> \Swagger\Client\Model\InlineResponse2003 deleteOrderPos($order_pos_id)

Deletes an order Position

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\OrderPosApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$order_pos_id = 56; // int | Id of order position resource to delete

try {
    $result = $apiInstance->deleteOrderPos($order_pos_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrderPosApi->deleteOrderPos: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order_pos_id** | **int**| Id of order position resource to delete |

### Return type

[**\Swagger\Client\Model\InlineResponse2003**](../Model/InlineResponse2003.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getOrderPositionById**
> \Swagger\Client\Model\InlineResponse2007 getOrderPositionById($order_pos_id)

Find order position by ID

Returns a single order position

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\OrderPosApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$order_pos_id = 56; // int | ID of order position to return

try {
    $result = $apiInstance->getOrderPositionById($order_pos_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrderPosApi->getOrderPositionById: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order_pos_id** | **int**| ID of order position to return |

### Return type

[**\Swagger\Client\Model\InlineResponse2007**](../Model/InlineResponse2007.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getOrderPositions**
> \Swagger\Client\Model\InlineResponse2007 getOrderPositions($order_id, $order_object_name)

Retrieve order positions

Retrieve all order positions depending on the filters defined in the query.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\OrderPosApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$order_id = 56; // int | Retrieve all order positions belonging to this order. Must be provided with voucher[objectName]
$order_object_name = "order_object_name_example"; // string | Only required if order[id] was provided. 'Order' should be used as value.

try {
    $result = $apiInstance->getOrderPositions($order_id, $order_object_name);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrderPosApi->getOrderPositions: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order_id** | **int**| Retrieve all order positions belonging to this order. Must be provided with voucher[objectName] | [optional]
 **order_object_name** | **string**| Only required if order[id] was provided. &#x27;Order&#x27; should be used as value. | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse2007**](../Model/InlineResponse2007.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateOrderPosition**
> \Swagger\Client\Model\InlineResponse2007 updateOrderPosition($order_pos_id, $body)

Update an existing order position

Update an order position

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\OrderPosApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$order_pos_id = 56; // int | ID of order position to update
$body = new \Swagger\Client\Model\ModelOrderPosUpdate(); // \Swagger\Client\Model\ModelOrderPosUpdate | Update data

try {
    $result = $apiInstance->updateOrderPosition($order_pos_id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OrderPosApi->updateOrderPosition: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order_pos_id** | **int**| ID of order position to update |
 **body** | [**\Swagger\Client\Model\ModelOrderPosUpdate**](../Model/ModelOrderPosUpdate.md)| Update data | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse2007**](../Model/InlineResponse2007.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

