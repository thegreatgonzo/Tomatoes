# Swagger\Client\AdminsApi

All URIs are relative to *https://virtserver.swaggerhub.com/thegreatgonzo/test1/1.0.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addInventory**](AdminsApi.md#addinventory) | **POST** /inventory | adds an inventory item

# **addInventory**
> addInventory($body)

adds an inventory item

Adds an item to the system

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\AdminsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Swagger\Client\Model\InventoryItem(); // \Swagger\Client\Model\InventoryItem | Inventory item to add

try {
    $apiInstance->addInventory($body);
} catch (Exception $e) {
    echo 'Exception when calling AdminsApi->addInventory: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\InventoryItem**](../Model/InventoryItem.md)| Inventory item to add | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

