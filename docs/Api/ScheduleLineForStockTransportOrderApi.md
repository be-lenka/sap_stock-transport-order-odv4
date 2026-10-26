# BeLenka\SAP\StockTransportOrderODV4\ScheduleLineForStockTransportOrderApi

All URIs are relative to https://:/sap/opu/odata4/sap/api_stocktransportorder/srvd_a2x/sap/stocktransportorder/0001, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**sTOScheduleLineGet()**](ScheduleLineForStockTransportOrderApi.md#sTOScheduleLineGet) | **GET** /STOScheduleLine | Get entities from STOScheduleLine |
| [**sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineDelete()**](ScheduleLineForStockTransportOrderApi.md#sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineDelete) | **DELETE** /STOScheduleLine/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine} | Delete entity from STOScheduleLine |
| [**sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineGet()**](ScheduleLineForStockTransportOrderApi.md#sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineGet) | **GET** /STOScheduleLine/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine} | Get entity from STOScheduleLine by key |
| [**sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLinePatch()**](ScheduleLineForStockTransportOrderApi.md#sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLinePatch) | **PATCH** /STOScheduleLine/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine} | Update entity in STOScheduleLine |
| [**sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentGet()**](ScheduleLineForStockTransportOrderApi.md#sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentGet) | **GET** /STOScheduleLine/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/_STOSubcontractingComponent | Get entities from related _STOSubcontractingComponent |
| [**sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentPost()**](ScheduleLineForStockTransportOrderApi.md#sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentPost) | **POST** /STOScheduleLine/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/_STOSubcontractingComponent | Add new entity to related _STOSubcontractingComponent |
| [**sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineStockTransportOrderGet()**](ScheduleLineForStockTransportOrderApi.md#sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineStockTransportOrderGet) | **GET** /STOScheduleLine/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/_StockTransportOrder | Get related _StockTransportOrder |
| [**sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineStockTransportOrderItemGet()**](ScheduleLineForStockTransportOrderApi.md#sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineStockTransportOrderItemGet) | **GET** /STOScheduleLine/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/_StockTransportOrderItem | Get related _StockTransportOrderItem |
| [**sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeScheduleLineGet()**](ScheduleLineForStockTransportOrderApi.md#sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeScheduleLineGet) | **GET** /STOSubcontractingComponent/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/{ReservationItem}/{RecordType}/_ScheduleLine | Get related _ScheduleLine |
| [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOScheduleLineGet()**](ScheduleLineForStockTransportOrderApi.md#stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOScheduleLineGet) | **GET** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOScheduleLine | Get entities from related _STOScheduleLine |
| [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOScheduleLinePost()**](ScheduleLineForStockTransportOrderApi.md#stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOScheduleLinePost) | **POST** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOScheduleLine | Add new entity to related _STOScheduleLine |


## `sTOScheduleLineGet()`

```php
sTOScheduleLineGet($top, $skip, $filter, $count, $orderby, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderScheduleLineType
```

Get entities from STOScheduleLine

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\ScheduleLineForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$top = 50; // int | Show only the first n items, see [Paging - Top](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptiontop)
$skip = 56; // int | Skip the first n items, see [Paging - Skip](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionskip)
$filter = 'filter_example'; // string | Filter items by property values, see [Filtering](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionfilter)
$count = True; // bool | Include count of items, see [Count](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptioncount)
$orderby = array('orderby_example'); // string[] | Order items by property values, see [Sorting](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionorderby)
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->sTOScheduleLineGet($top, $skip, $filter, $count, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ScheduleLineForStockTransportOrderApi->sTOScheduleLineGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderScheduleLineType**](../Model/CollectionOfStockTransportOrderScheduleLineType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineDelete()`

```php
sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineDelete($stock_transport_order, $stock_transport_order_item, $schedule_line)
```

Delete entity from STOScheduleLine

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\ScheduleLineForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$schedule_line = 'schedule_line_example'; // string | Delivery Schedule Line Counter

try {
    $apiInstance->sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineDelete($stock_transport_order, $stock_transport_order_item, $schedule_line);
} catch (Exception $e) {
    echo 'Exception when calling ScheduleLineForStockTransportOrderApi->sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineDelete: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **stock_transport_order_item** | **string**| Stock Transport Order Item | |
| **schedule_line** | **string**| Delivery Schedule Line Counter | |

### Return type

void (empty response body)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineGet()`

```php
sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineGet($stock_transport_order, $stock_transport_order_item, $schedule_line, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineType
```

Get entity from STOScheduleLine by key

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\ScheduleLineForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$schedule_line = 'schedule_line_example'; // string | Delivery Schedule Line Counter
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineGet($stock_transport_order, $stock_transport_order_item, $schedule_line, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ScheduleLineForStockTransportOrderApi->sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **stock_transport_order_item** | **string**| Stock Transport Order Item | |
| **schedule_line** | **string**| Delivery Schedule Line Counter | |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand) | [optional] |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLinePatch()`

```php
sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLinePatch($stock_transport_order, $stock_transport_order_item, $schedule_line, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_schedule_line_type_update): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineType
```

Update entity in STOScheduleLine

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\ScheduleLineForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$schedule_line = 'schedule_line_example'; // string | Delivery Schedule Line Counter
$com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_schedule_line_type_update = new \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineTypeUpdate(); // \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineTypeUpdate | New property values

try {
    $result = $apiInstance->sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLinePatch($stock_transport_order, $stock_transport_order_item, $schedule_line, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_schedule_line_type_update);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ScheduleLineForStockTransportOrderApi->sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLinePatch: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **stock_transport_order_item** | **string**| Stock Transport Order Item | |
| **schedule_line** | **string**| Delivery Schedule Line Counter | |
| **com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_schedule_line_type_update** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineTypeUpdate**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineTypeUpdate.md)| New property values | |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentGet()`

```php
sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentGet($stock_transport_order, $stock_transport_order_item, $schedule_line, $top, $skip, $filter, $count, $orderby, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfSTOSubcontractingComponentType
```

Get entities from related _STOSubcontractingComponent

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\ScheduleLineForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$schedule_line = 'schedule_line_example'; // string | Delivery Schedule Line Counter
$top = 50; // int | Show only the first n items, see [Paging - Top](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptiontop)
$skip = 56; // int | Skip the first n items, see [Paging - Skip](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionskip)
$filter = 'filter_example'; // string | Filter items by property values, see [Filtering](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionfilter)
$count = True; // bool | Include count of items, see [Count](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptioncount)
$orderby = array('orderby_example'); // string[] | Order items by property values, see [Sorting](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionorderby)
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentGet($stock_transport_order, $stock_transport_order_item, $schedule_line, $top, $skip, $filter, $count, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ScheduleLineForStockTransportOrderApi->sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **stock_transport_order_item** | **string**| Stock Transport Order Item | |
| **schedule_line** | **string**| Delivery Schedule Line Counter | |
| **top** | **int**| Show only the first n items, see [Paging - Top](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptiontop) | [optional] |
| **skip** | **int**| Skip the first n items, see [Paging - Skip](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionskip) | [optional] |
| **filter** | **string**| Filter items by property values, see [Filtering](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionfilter) | [optional] |
| **count** | **bool**| Include count of items, see [Count](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptioncount) | [optional] |
| **orderby** | [**string[]**](../Model/string.md)| Order items by property values, see [Sorting](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionorderby) | [optional] |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand) | [optional] |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfSTOSubcontractingComponentType**](../Model/CollectionOfSTOSubcontractingComponentType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentPost()`

```php
sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentPost($stock_transport_order, $stock_transport_order_item, $schedule_line, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_sto_subcontracting_component_type_create): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentType
```

Add new entity to related _STOSubcontractingComponent

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\ScheduleLineForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$schedule_line = 'schedule_line_example'; // string | Delivery Schedule Line Counter
$com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_sto_subcontracting_component_type_create = new \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentTypeCreate(); // \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentTypeCreate | New entity

try {
    $result = $apiInstance->sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentPost($stock_transport_order, $stock_transport_order_item, $schedule_line, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_sto_subcontracting_component_type_create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ScheduleLineForStockTransportOrderApi->sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **stock_transport_order_item** | **string**| Stock Transport Order Item | |
| **schedule_line** | **string**| Delivery Schedule Line Counter | |
| **com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_sto_subcontracting_component_type_create** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentTypeCreate**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentTypeCreate.md)| New entity | |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineStockTransportOrderGet()`

```php
sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineStockTransportOrderGet($stock_transport_order, $stock_transport_order_item, $schedule_line, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType
```

Get related _StockTransportOrder

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\ScheduleLineForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$schedule_line = 'schedule_line_example'; // string | Delivery Schedule Line Counter
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineStockTransportOrderGet($stock_transport_order, $stock_transport_order_item, $schedule_line, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ScheduleLineForStockTransportOrderApi->sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineStockTransportOrderGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **stock_transport_order_item** | **string**| Stock Transport Order Item | |
| **schedule_line** | **string**| Delivery Schedule Line Counter | |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand) | [optional] |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineStockTransportOrderItemGet()`

```php
sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineStockTransportOrderItemGet($stock_transport_order, $stock_transport_order_item, $schedule_line, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemType
```

Get related _StockTransportOrderItem

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\ScheduleLineForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$schedule_line = 'schedule_line_example'; // string | Delivery Schedule Line Counter
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineStockTransportOrderItemGet($stock_transport_order, $stock_transport_order_item, $schedule_line, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ScheduleLineForStockTransportOrderApi->sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineStockTransportOrderItemGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **stock_transport_order_item** | **string**| Stock Transport Order Item | |
| **schedule_line** | **string**| Delivery Schedule Line Counter | |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand) | [optional] |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeScheduleLineGet()`

```php
sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeScheduleLineGet($stock_transport_order, $stock_transport_order_item, $schedule_line, $reservation_item, $record_type, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineType
```

Get related _ScheduleLine

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\ScheduleLineForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$schedule_line = 'schedule_line_example'; // string | Delivery Schedule Line Counter
$reservation_item = 'reservation_item_example'; // string | Reservation Item
$record_type = 'record_type_example'; // string | Reservation Record Type
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeScheduleLineGet($stock_transport_order, $stock_transport_order_item, $schedule_line, $reservation_item, $record_type, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ScheduleLineForStockTransportOrderApi->sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeScheduleLineGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **stock_transport_order_item** | **string**| Stock Transport Order Item | |
| **schedule_line** | **string**| Delivery Schedule Line Counter | |
| **reservation_item** | **string**| Reservation Item | |
| **record_type** | **string**| Reservation Record Type | |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand) | [optional] |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOScheduleLineGet()`

```php
stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOScheduleLineGet($stock_transport_order, $stock_transport_order_item, $top, $skip, $filter, $count, $orderby, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderScheduleLineType
```

Get entities from related _STOScheduleLine

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\ScheduleLineForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
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
    $result = $apiInstance->stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOScheduleLineGet($stock_transport_order, $stock_transport_order_item, $top, $skip, $filter, $count, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ScheduleLineForStockTransportOrderApi->stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOScheduleLineGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderScheduleLineType**](../Model/CollectionOfStockTransportOrderScheduleLineType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOScheduleLinePost()`

```php
stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOScheduleLinePost($stock_transport_order, $stock_transport_order_item, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_schedule_line_type_create): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineType
```

Add new entity to related _STOScheduleLine

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\ScheduleLineForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_schedule_line_type_create = new \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineTypeCreate(); // \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineTypeCreate | New entity

try {
    $result = $apiInstance->stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOScheduleLinePost($stock_transport_order, $stock_transport_order_item, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_schedule_line_type_create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ScheduleLineForStockTransportOrderApi->stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOScheduleLinePost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **stock_transport_order_item** | **string**| Stock Transport Order Item | |
| **com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_schedule_line_type_create** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineTypeCreate**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineTypeCreate.md)| New entity | |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
