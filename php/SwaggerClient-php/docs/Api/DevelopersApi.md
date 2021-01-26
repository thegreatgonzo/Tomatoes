# Swagger\Client\DevelopersApi

All URIs are relative to *https://virtserver.swaggerhub.com/thegreatgonzo/test1/1.0.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**searchInventory**](DevelopersApi.md#searchinventory) | **GET** /inventory | searches inventory

# **searchInventory**
> \Swagger\Client\Model\InventoryItem[] searchInventory($search_string, $skip, $limit)

searches inventory

By passing in the appropriate options, you can search for available inventory in the system

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\DevelopersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$search_string = "search_string_example"; // string | pass an optional search string for looking up inventory
$skip = 56; // int | number of records to skip for pagination
$limit = 56; // int | maximum number of records to return

try {
    $result = $apiInstance->searchInventory($search_string, $skip, $limit);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DevelopersApi->searchInventory: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **search_string** | **string**| pass an optional search string for looking up inventory | [optional]
 **skip** | **int**| number of records to skip for pagination | [optional]
 **limit** | **int**| maximum number of records to return | [optional]

### Return type

[**\Swagger\Client\Model\InventoryItem[]**](../Model/InventoryItem.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

