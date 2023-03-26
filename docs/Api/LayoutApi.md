# Swagger\Client\LayoutApi

All URIs are relative to *https://my.sevdesk.de/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getLetterpapersWithThumb**](LayoutApi.md#getletterpaperswiththumb) | **GET** /DocServer/getLetterpapersWithThumb | Retrieve letterpapers
[**getTemplates**](LayoutApi.md#gettemplates) | **GET** /DocServer/getTemplatesWithThumb | Retrieve templates
[**updateCreditNoteTemplate**](LayoutApi.md#updatecreditnotetemplate) | **PUT** /CreditNote/{creditNoteId}/changeParameter | Update an of credit note template
[**updateInvoiceTemplate**](LayoutApi.md#updateinvoicetemplate) | **PUT** /Invoice/{invoiceId}/changeParameter | Update an invoice template
[**updateOrderTemplate**](LayoutApi.md#updateordertemplate) | **PUT** /Order/{orderId}/changeParameter | Update an order template

# **getLetterpapersWithThumb**
> \Swagger\Client\Model\InlineResponse20015 getLetterpapersWithThumb()

Retrieve letterpapers

Retrieve all letterpapers with Thumb

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\LayoutApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->getLetterpapersWithThumb();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling LayoutApi->getLetterpapersWithThumb: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\InlineResponse20015**](../Model/InlineResponse20015.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getTemplates**
> \Swagger\Client\Model\InlineResponse20037 getTemplates($type)

Retrieve templates

Retrieve all templates

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\LayoutApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$type = "type_example"; // string | Type of the templates you want to get.

try {
    $result = $apiInstance->getTemplates($type);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling LayoutApi->getTemplates: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **type** | **string**| Type of the templates you want to get. | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse20037**](../Model/InlineResponse20037.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateCreditNoteTemplate**
> \Swagger\Client\Model\InlineResponse20017 updateCreditNoteTemplate($credit_note_id, $body)

Update an of credit note template

Update an existing of credit note template

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\LayoutApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$credit_note_id = 56; // int | ID of credit note to update
$body = new \Swagger\Client\Model\ModelChangeLayout(); // \Swagger\Client\Model\ModelChangeLayout | Change Layout

try {
    $result = $apiInstance->updateCreditNoteTemplate($credit_note_id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling LayoutApi->updateCreditNoteTemplate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **credit_note_id** | **int**| ID of credit note to update |
 **body** | [**\Swagger\Client\Model\ModelChangeLayout**](../Model/ModelChangeLayout.md)| Change Layout | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse20017**](../Model/InlineResponse20017.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateInvoiceTemplate**
> \Swagger\Client\Model\InlineResponse20017 updateInvoiceTemplate($invoice_id, $body)

Update an invoice template

Update an existing invoice template

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\LayoutApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$invoice_id = 56; // int | ID of invoice to update
$body = new \Swagger\Client\Model\ModelChangeLayout(); // \Swagger\Client\Model\ModelChangeLayout | Change Layout

try {
    $result = $apiInstance->updateInvoiceTemplate($invoice_id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling LayoutApi->updateInvoiceTemplate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **int**| ID of invoice to update |
 **body** | [**\Swagger\Client\Model\ModelChangeLayout**](../Model/ModelChangeLayout.md)| Change Layout | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse20017**](../Model/InlineResponse20017.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateOrderTemplate**
> \Swagger\Client\Model\InlineResponse20017 updateOrderTemplate($order_id, $body)

Update an order template

Update an existing order template

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\LayoutApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$order_id = 56; // int | ID of order to update
$body = new \Swagger\Client\Model\ModelChangeLayout(); // \Swagger\Client\Model\ModelChangeLayout | Change Layout

try {
    $result = $apiInstance->updateOrderTemplate($order_id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling LayoutApi->updateOrderTemplate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order_id** | **int**| ID of order to update |
 **body** | [**\Swagger\Client\Model\ModelChangeLayout**](../Model/ModelChangeLayout.md)| Change Layout | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse20017**](../Model/InlineResponse20017.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

