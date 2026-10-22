# BeLenka\SAP\StockTransportOrderODV4\AccountAssignmentForSTOApi

All URIs are relative to https://:/sap/opu/odata4/sap/api_stocktransportorder/srvd_a2x/sap/stocktransportorder/0001, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**sTOAccountAssignmentGet()**](AccountAssignmentForSTOApi.md#sTOAccountAssignmentGet) | **GET** /STOAccountAssignment | Get entities from STOAccountAssignment |
| [**sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberDelete()**](AccountAssignmentForSTOApi.md#sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberDelete) | **DELETE** /STOAccountAssignment/{StockTransportOrder}/{StockTransportOrderItem}/{AccountAssignmentNumber} | Delete entity from STOAccountAssignment |
| [**sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberGet()**](AccountAssignmentForSTOApi.md#sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberGet) | **GET** /STOAccountAssignment/{StockTransportOrder}/{StockTransportOrderItem}/{AccountAssignmentNumber} | Get entity from STOAccountAssignment by key |
| [**sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberPatch()**](AccountAssignmentForSTOApi.md#sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberPatch) | **PATCH** /STOAccountAssignment/{StockTransportOrder}/{StockTransportOrderItem}/{AccountAssignmentNumber} | Update entity in STOAccountAssignment |
| [**sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberStockTransportOrderGet()**](AccountAssignmentForSTOApi.md#sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberStockTransportOrderGet) | **GET** /STOAccountAssignment/{StockTransportOrder}/{StockTransportOrderItem}/{AccountAssignmentNumber}/_StockTransportOrder | Get related _StockTransportOrder |
| [**sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberStockTransportOrderItemGet()**](AccountAssignmentForSTOApi.md#sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberStockTransportOrderItemGet) | **GET** /STOAccountAssignment/{StockTransportOrder}/{StockTransportOrderItem}/{AccountAssignmentNumber}/_StockTransportOrderItem | Get related _StockTransportOrderItem |
| [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOAccountAssignmentGet()**](AccountAssignmentForSTOApi.md#stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOAccountAssignmentGet) | **GET** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOAccountAssignment | Get entities from related _STOAccountAssignment |
| [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOAccountAssignmentPost()**](AccountAssignmentForSTOApi.md#stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOAccountAssignmentPost) | **POST** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOAccountAssignment | Add new entity to related _STOAccountAssignment |


## `sTOAccountAssignmentGet()`

```php
sTOAccountAssignmentGet($top, $skip, $filter, $count, $orderby, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderAccountAssignmentType
```

Get entities from STOAccountAssignment

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\AccountAssignmentForSTOApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$top = 50; // int | Show only the first n items, see [Paging - Top](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptiontop)
$skip = 56; // int | Skip the first n items, see [Paging - Skip](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionskip)
$filter = 'filter_example'; // string | Filter items by property values, see [Filtering](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionfilter)
$count = True; // bool | Include count of items, see [Count](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptioncount)
$orderby = array('orderby_example'); // string[] | Order items by property values, see [Sorting](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionorderby)
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->sTOAccountAssignmentGet($top, $skip, $filter, $count, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AccountAssignmentForSTOApi->sTOAccountAssignmentGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **top** | **int**| Show only the first n items, see [Paging - Top](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptiontop) | [optional] |
| **skip** | **int**| Skip the first n items, see [Paging - Skip](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionskip) | [optional] |
| **filter** | **string**| Filter items by property values, see [Filtering](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionfilter) | [optional] |
| **count** | **bool**| Include count of items, see [Count](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptioncount) | [optional] |
| **orderby** | [**string[]**](../Model/string.md)| Order items by property values, see [Sorting](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionorderby) | [optional] |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand) | [optional] |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderAccountAssignmentType**](../Model/CollectionOfStockTransportOrderAccountAssignmentType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberDelete()`

```php
sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberDelete($stock_transport_order, $stock_transport_order_item, $account_assignment_number)
```

Delete entity from STOAccountAssignment

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\AccountAssignmentForSTOApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Purchasing Document Number
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Item Number of Purchasing Document
$account_assignment_number = 'account_assignment_number_example'; // string | Sequential Number of Account Assignment

try {
    $apiInstance->sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberDelete($stock_transport_order, $stock_transport_order_item, $account_assignment_number);
} catch (Exception $e) {
    echo 'Exception when calling AccountAssignmentForSTOApi->sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberDelete: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Purchasing Document Number | |
| **stock_transport_order_item** | **string**| Item Number of Purchasing Document | |
| **account_assignment_number** | **string**| Sequential Number of Account Assignment | |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberGet()`

```php
sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberGet($stock_transport_order, $stock_transport_order_item, $account_assignment_number, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentType
```

Get entity from STOAccountAssignment by key

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\AccountAssignmentForSTOApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Purchasing Document Number
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Item Number of Purchasing Document
$account_assignment_number = 'account_assignment_number_example'; // string | Sequential Number of Account Assignment
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberGet($stock_transport_order, $stock_transport_order_item, $account_assignment_number, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AccountAssignmentForSTOApi->sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Purchasing Document Number | |
| **stock_transport_order_item** | **string**| Item Number of Purchasing Document | |
| **account_assignment_number** | **string**| Sequential Number of Account Assignment | |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand) | [optional] |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberPatch()`

```php
sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberPatch($stock_transport_order, $stock_transport_order_item, $account_assignment_number, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_account_assignment_type_update): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentType
```

Update entity in STOAccountAssignment

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\AccountAssignmentForSTOApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Purchasing Document Number
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Item Number of Purchasing Document
$account_assignment_number = 'account_assignment_number_example'; // string | Sequential Number of Account Assignment
$com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_account_assignment_type_update = new \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentTypeUpdate(); // \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentTypeUpdate | New property values

try {
    $result = $apiInstance->sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberPatch($stock_transport_order, $stock_transport_order_item, $account_assignment_number, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_account_assignment_type_update);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AccountAssignmentForSTOApi->sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberPatch: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Purchasing Document Number | |
| **stock_transport_order_item** | **string**| Item Number of Purchasing Document | |
| **account_assignment_number** | **string**| Sequential Number of Account Assignment | |
| **com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_account_assignment_type_update** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentTypeUpdate**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentTypeUpdate.md)| New property values | |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberStockTransportOrderGet()`

```php
sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberStockTransportOrderGet($stock_transport_order, $stock_transport_order_item, $account_assignment_number, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType
```

Get related _StockTransportOrder

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\AccountAssignmentForSTOApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Purchasing Document Number
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Item Number of Purchasing Document
$account_assignment_number = 'account_assignment_number_example'; // string | Sequential Number of Account Assignment
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberStockTransportOrderGet($stock_transport_order, $stock_transport_order_item, $account_assignment_number, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AccountAssignmentForSTOApi->sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberStockTransportOrderGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Purchasing Document Number | |
| **stock_transport_order_item** | **string**| Item Number of Purchasing Document | |
| **account_assignment_number** | **string**| Sequential Number of Account Assignment | |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand) | [optional] |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberStockTransportOrderItemGet()`

```php
sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberStockTransportOrderItemGet($stock_transport_order, $stock_transport_order_item, $account_assignment_number, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemType
```

Get related _StockTransportOrderItem

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\AccountAssignmentForSTOApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Purchasing Document Number
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Item Number of Purchasing Document
$account_assignment_number = 'account_assignment_number_example'; // string | Sequential Number of Account Assignment
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberStockTransportOrderItemGet($stock_transport_order, $stock_transport_order_item, $account_assignment_number, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AccountAssignmentForSTOApi->sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberStockTransportOrderItemGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Purchasing Document Number | |
| **stock_transport_order_item** | **string**| Item Number of Purchasing Document | |
| **account_assignment_number** | **string**| Sequential Number of Account Assignment | |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand) | [optional] |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOAccountAssignmentGet()`

```php
stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOAccountAssignmentGet($stock_transport_order, $stock_transport_order_item, $top, $skip, $filter, $count, $orderby, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderAccountAssignmentType
```

Get entities from related _STOAccountAssignment

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\AccountAssignmentForSTOApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$top = 50; // int | Show only the first n items, see [Paging - Top](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptiontop)
$skip = 56; // int | Skip the first n items, see [Paging - Skip](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionskip)
$filter = 'filter_example'; // string | Filter items by property values, see [Filtering](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionfilter)
$count = True; // bool | Include count of items, see [Count](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptioncount)
$orderby = array('orderby_example'); // string[] | Order items by property values, see [Sorting](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionorderby)
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOAccountAssignmentGet($stock_transport_order, $stock_transport_order_item, $top, $skip, $filter, $count, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AccountAssignmentForSTOApi->stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOAccountAssignmentGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **stock_transport_order_item** | **string**| Stock Transport Order Item | |
| **top** | **int**| Show only the first n items, see [Paging - Top](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptiontop) | [optional] |
| **skip** | **int**| Skip the first n items, see [Paging - Skip](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionskip) | [optional] |
| **filter** | **string**| Filter items by property values, see [Filtering](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionfilter) | [optional] |
| **count** | **bool**| Include count of items, see [Count](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptioncount) | [optional] |
| **orderby** | [**string[]**](../Model/string.md)| Order items by property values, see [Sorting](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionorderby) | [optional] |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand) | [optional] |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderAccountAssignmentType**](../Model/CollectionOfStockTransportOrderAccountAssignmentType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOAccountAssignmentPost()`

```php
stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOAccountAssignmentPost($stock_transport_order, $stock_transport_order_item, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_account_assignment_type_create): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentType
```

Add new entity to related _STOAccountAssignment

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\AccountAssignmentForSTOApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_account_assignment_type_create = new \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentTypeCreate(); // \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentTypeCreate | New entity

try {
    $result = $apiInstance->stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOAccountAssignmentPost($stock_transport_order, $stock_transport_order_item, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_account_assignment_type_create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AccountAssignmentForSTOApi->stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOAccountAssignmentPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **stock_transport_order_item** | **string**| Stock Transport Order Item | |
| **com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_account_assignment_type_create** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentTypeCreate**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentTypeCreate.md)| New entity | |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
