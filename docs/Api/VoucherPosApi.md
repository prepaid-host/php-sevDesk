# Swagger\Client\VoucherPosApi

All URIs are relative to *https://my.sevdesk.de/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getVoucherPositions**](VoucherPosApi.md#getvoucherpositions) | **GET** /VoucherPos | Retrieve voucher positions

# **getVoucherPositions**
> \Swagger\Client\Model\InlineResponse20031 getVoucherPositions($voucher_id, $voucher_object_name)

Retrieve voucher positions

Retrieve all voucher positions depending on the filters defined in the query.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\VoucherPosApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$voucher_id = 56; // int | Retrieve all vouchers positions belonging to this voucher. Must be provided with voucher[objectName]
$voucher_object_name = "voucher_object_name_example"; // string | Only required if voucher[id] was provided. 'Voucher' should be used as value.

try {
    $result = $apiInstance->getVoucherPositions($voucher_id, $voucher_object_name);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling VoucherPosApi->getVoucherPositions: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **voucher_id** | **int**| Retrieve all vouchers positions belonging to this voucher. Must be provided with voucher[objectName] | [optional]
 **voucher_object_name** | **string**| Only required if voucher[id] was provided. &#x27;Voucher&#x27; should be used as value. | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse20031**](../Model/InlineResponse20031.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

