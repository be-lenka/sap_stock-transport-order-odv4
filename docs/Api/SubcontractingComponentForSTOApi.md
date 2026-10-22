# BeLenka\SAP\StockTransportOrderODV4\SubcontractingComponentForSTOApi

All URIs are relative to https://:/sap/opu/odata4/sap/api_stocktransportorder/srvd_a2x/sap/stocktransportorder/0001, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentGet()**](SubcontractingComponentForSTOApi.md#sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentGet) | **GET** /STOScheduleLine/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/_STOSubcontractingComponent | Get entities from related _STOSubcontractingComponent |
| [**sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentPost()**](SubcontractingComponentForSTOApi.md#sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentPost) | **POST** /STOScheduleLine/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/_STOSubcontractingComponent | Add new entity to related _STOSubcontractingComponent |
| [**sTOSubcontractingComponentGet()**](SubcontractingComponentForSTOApi.md#sTOSubcontractingComponentGet) | **GET** /STOSubcontractingComponent | Get entities from STOSubcontractingComponent |
| [**sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeDelete()**](SubcontractingComponentForSTOApi.md#sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeDelete) | **DELETE** /STOSubcontractingComponent/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/{ReservationItem}/{RecordType} | Delete entity from STOSubcontractingComponent |
| [**sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeGet()**](SubcontractingComponentForSTOApi.md#sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeGet) | **GET** /STOSubcontractingComponent/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/{ReservationItem}/{RecordType} | Get entity from STOSubcontractingComponent by key |
| [**sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypePatch()**](SubcontractingComponentForSTOApi.md#sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypePatch) | **PATCH** /STOSubcontractingComponent/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/{ReservationItem}/{RecordType} | Update entity in STOSubcontractingComponent |
| [**sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeScheduleLineGet()**](SubcontractingComponentForSTOApi.md#sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeScheduleLineGet) | **GET** /STOSubcontractingComponent/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/{ReservationItem}/{RecordType}/_ScheduleLine | Get related _ScheduleLine |
| [**sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeStockTransportOrderGet()**](SubcontractingComponentForSTOApi.md#sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeStockTransportOrderGet) | **GET** /STOSubcontractingComponent/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/{ReservationItem}/{RecordType}/_StockTransportOrder | Get related _StockTransportOrder |
| [**sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeStockTransportOrderItemGet()**](SubcontractingComponentForSTOApi.md#sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeStockTransportOrderItemGet) | **GET** /STOSubcontractingComponent/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/{ReservationItem}/{RecordType}/_StockTransportOrderItem | Get related _StockTransportOrderItem |


## `sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentGet()`

```php
sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentGet($stock_transport_order, $stock_transport_order_item, $schedule_line, $top, $skip, $filter, $count, $orderby, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfSTOSubcontractingComponentType
```

Get entities from related _STOSubcontractingComponent

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\SubcontractingComponentForSTOApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
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
    echo 'Exception when calling SubcontractingComponentForSTOApi->sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentGet: ', $e->getMessage(), PHP_EOL;
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

No authorization required

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



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\SubcontractingComponentForSTOApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$schedule_line = 'schedule_line_example'; // string | Delivery Schedule Line Counter
$com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_sto_subcontracting_component_type_create = new \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentTypeCreate(); // \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentTypeCreate | New entity

try {
    $result = $apiInstance->sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentPost($stock_transport_order, $stock_transport_order_item, $schedule_line, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_sto_subcontracting_component_type_create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubcontractingComponentForSTOApi->sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentPost: ', $e->getMessage(), PHP_EOL;
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

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sTOSubcontractingComponentGet()`

```php
sTOSubcontractingComponentGet($top, $skip, $filter, $count, $orderby, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfSTOSubcontractingComponentType
```

Get entities from STOSubcontractingComponent

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\SubcontractingComponentForSTOApi(
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
    $result = $apiInstance->sTOSubcontractingComponentGet($top, $skip, $filter, $count, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubcontractingComponentForSTOApi->sTOSubcontractingComponentGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfSTOSubcontractingComponentType**](../Model/CollectionOfSTOSubcontractingComponentType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeDelete()`

```php
sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeDelete($stock_transport_order, $stock_transport_order_item, $schedule_line, $reservation_item, $record_type)
```

Delete entity from STOSubcontractingComponent

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\SubcontractingComponentForSTOApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$schedule_line = 'schedule_line_example'; // string | Delivery Schedule Line Counter
$reservation_item = 'reservation_item_example'; // string | Reservation Item
$record_type = 'record_type_example'; // string | Reservation Record Type

try {
    $apiInstance->sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeDelete($stock_transport_order, $stock_transport_order_item, $schedule_line, $reservation_item, $record_type);
} catch (Exception $e) {
    echo 'Exception when calling SubcontractingComponentForSTOApi->sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeDelete: ', $e->getMessage(), PHP_EOL;
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

## `sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeGet()`

```php
sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeGet($stock_transport_order, $stock_transport_order_item, $schedule_line, $reservation_item, $record_type, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentType
```

Get entity from STOSubcontractingComponent by key

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\SubcontractingComponentForSTOApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$schedule_line = 'schedule_line_example'; // string | Delivery Schedule Line Counter
$reservation_item = 'reservation_item_example'; // string | Reservation Item
$record_type = 'record_type_example'; // string | Reservation Record Type
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeGet($stock_transport_order, $stock_transport_order_item, $schedule_line, $reservation_item, $record_type, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubcontractingComponentForSTOApi->sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypePatch()`

```php
sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypePatch($stock_transport_order, $stock_transport_order_item, $schedule_line, $reservation_item, $record_type, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_sto_subcontracting_component_type_update): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentType
```

Update entity in STOSubcontractingComponent

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\SubcontractingComponentForSTOApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$schedule_line = 'schedule_line_example'; // string | Delivery Schedule Line Counter
$reservation_item = 'reservation_item_example'; // string | Reservation Item
$record_type = 'record_type_example'; // string | Reservation Record Type
$com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_sto_subcontracting_component_type_update = new \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentTypeUpdate(); // \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentTypeUpdate | New property values

try {
    $result = $apiInstance->sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypePatch($stock_transport_order, $stock_transport_order_item, $schedule_line, $reservation_item, $record_type, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_sto_subcontracting_component_type_update);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubcontractingComponentForSTOApi->sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypePatch: ', $e->getMessage(), PHP_EOL;
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
| **com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_sto_subcontracting_component_type_update** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentTypeUpdate**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentTypeUpdate.md)| New property values | |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
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



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\SubcontractingComponentForSTOApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
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
    echo 'Exception when calling SubcontractingComponentForSTOApi->sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeScheduleLineGet: ', $e->getMessage(), PHP_EOL;
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

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeStockTransportOrderGet()`

```php
sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeStockTransportOrderGet($stock_transport_order, $stock_transport_order_item, $schedule_line, $reservation_item, $record_type, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType
```

Get related _StockTransportOrder

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\SubcontractingComponentForSTOApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$schedule_line = 'schedule_line_example'; // string | Delivery Schedule Line Counter
$reservation_item = 'reservation_item_example'; // string | Reservation Item
$record_type = 'record_type_example'; // string | Reservation Record Type
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeStockTransportOrderGet($stock_transport_order, $stock_transport_order_item, $schedule_line, $reservation_item, $record_type, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubcontractingComponentForSTOApi->sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeStockTransportOrderGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeStockTransportOrderItemGet()`

```php
sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeStockTransportOrderItemGet($stock_transport_order, $stock_transport_order_item, $schedule_line, $reservation_item, $record_type, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemType
```

Get related _StockTransportOrderItem

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\SubcontractingComponentForSTOApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$schedule_line = 'schedule_line_example'; // string | Delivery Schedule Line Counter
$reservation_item = 'reservation_item_example'; // string | Reservation Item
$record_type = 'record_type_example'; // string | Reservation Record Type
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeStockTransportOrderItemGet($stock_transport_order, $stock_transport_order_item, $schedule_line, $reservation_item, $record_type, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubcontractingComponentForSTOApi->sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeStockTransportOrderItemGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
