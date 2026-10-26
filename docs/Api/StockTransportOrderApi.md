# BeLenka\SAP\StockTransportOrderODV4\StockTransportOrderApi

All URIs are relative to https://:/sap/opu/odata4/sap/api_stocktransportorder/srvd_a2x/sap/stocktransportorder/0001, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberStockTransportOrderGet()**](StockTransportOrderApi.md#sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberStockTransportOrderGet) | **GET** /STOAccountAssignment/{StockTransportOrder}/{StockTransportOrderItem}/{AccountAssignmentNumber}/_StockTransportOrder | Get related _StockTransportOrder |
| [**sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterStockTransportOrderGet()**](StockTransportOrderApi.md#sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterStockTransportOrderGet) | **GET** /STOItemPricingElement/{StockTransportOrder}/{StockTransportOrderItem}/{PricingDocument}/{PricingDocumentItem}/{PricingProcedureStep}/{PricingProcedureCounter}/_StockTransportOrder | Get related _StockTransportOrder |
| [**sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineStockTransportOrderGet()**](StockTransportOrderApi.md#sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineStockTransportOrderGet) | **GET** /STOScheduleLine/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/_StockTransportOrder | Get related _StockTransportOrder |
| [**sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeStockTransportOrderGet()**](StockTransportOrderApi.md#sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeStockTransportOrderGet) | **GET** /STOSubcontractingComponent/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/{ReservationItem}/{RecordType}/_StockTransportOrder | Get related _StockTransportOrder |
| [**stockTransportOrderGet()**](StockTransportOrderApi.md#stockTransportOrderGet) | **GET** /StockTransportOrder | Get entities from StockTransportOrder |
| [**stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageStockTransportOrderGet()**](StockTransportOrderApi.md#stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageStockTransportOrderGet) | **GET** /StockTransportOrderItemNote/{StockTransportOrder}/{StockTransportOrderItem}/{TextObjectType}/{Language}/_StockTransportOrder | Get related _StockTransportOrder |
| [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemStockTransportOrderGet()**](StockTransportOrderApi.md#stockTransportOrderItemStockTransportOrderStockTransportOrderItemStockTransportOrderGet) | **GET** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_StockTransportOrder | Get related _StockTransportOrder |
| [**stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageStockTransportOrderGet()**](StockTransportOrderApi.md#stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageStockTransportOrderGet) | **GET** /StockTransportOrderNote/{StockTransportOrder}/{TextObjectType}/{Language}/_StockTransportOrder | Get related _StockTransportOrder |
| [**stockTransportOrderPartnerStockTransportOrderPartnerFunctionStockTransportOrderGet()**](StockTransportOrderApi.md#stockTransportOrderPartnerStockTransportOrderPartnerFunctionStockTransportOrderGet) | **GET** /StockTransportOrderPartner/{StockTransportOrder}/{PartnerFunction}/_StockTransportOrder | Get related _StockTransportOrder |
| [**stockTransportOrderPost()**](StockTransportOrderApi.md#stockTransportOrderPost) | **POST** /StockTransportOrder | Add new entity to StockTransportOrder |
| [**stockTransportOrderShippingStockTransportOrderStockTransportOrderItemStockTransportOrderGet()**](StockTransportOrderApi.md#stockTransportOrderShippingStockTransportOrderStockTransportOrderItemStockTransportOrderGet) | **GET** /StockTransportOrderShipping/{StockTransportOrder}/{StockTransportOrderItem}/_StockTransportOrder | Get related _StockTransportOrder |
| [**stockTransportOrderStockTransportOrderGet()**](StockTransportOrderApi.md#stockTransportOrderStockTransportOrderGet) | **GET** /StockTransportOrder/{StockTransportOrder} | Get entity from StockTransportOrder by key |
| [**stockTransportOrderStockTransportOrderPatch()**](StockTransportOrderApi.md#stockTransportOrderStockTransportOrderPatch) | **PATCH** /StockTransportOrder/{StockTransportOrder} | Update entity in StockTransportOrder |
| [**stockTransportOrderStockTransportOrderSAPSelfBlockAllItemsPost()**](StockTransportOrderApi.md#stockTransportOrderStockTransportOrderSAPSelfBlockAllItemsPost) | **POST** /StockTransportOrder/{StockTransportOrder}/SAP__self.BlockAllItems | Invoke action BlockAllItems |
| [**stockTransportOrderStockTransportOrderSAPSelfReadOrderingAddressGet()**](StockTransportOrderApi.md#stockTransportOrderStockTransportOrderSAPSelfReadOrderingAddressGet) | **GET** /StockTransportOrder/{StockTransportOrder}/SAP__self.ReadOrderingAddress() | Invoke function ReadOrderingAddress |
| [**stockTransportOrderStockTransportOrderSAPSelfSetAllItemsToDeletedPost()**](StockTransportOrderApi.md#stockTransportOrderStockTransportOrderSAPSelfSetAllItemsToDeletedPost) | **POST** /StockTransportOrder/{StockTransportOrder}/SAP__self.SetAllItemsToDeleted | Invoke action SetAllItemsToDeleted |
| [**stockTransportOrderStockTransportOrderStockTransportOrderItemGet()**](StockTransportOrderApi.md#stockTransportOrderStockTransportOrderStockTransportOrderItemGet) | **GET** /StockTransportOrder/{StockTransportOrder}/_StockTransportOrderItem | Get entities from related _StockTransportOrderItem |
| [**stockTransportOrderStockTransportOrderStockTransportOrderItemPost()**](StockTransportOrderApi.md#stockTransportOrderStockTransportOrderStockTransportOrderItemPost) | **POST** /StockTransportOrder/{StockTransportOrder}/_StockTransportOrderItem | Add new entity to related _StockTransportOrderItem |
| [**stockTransportOrderStockTransportOrderStockTransportOrderNoteGet()**](StockTransportOrderApi.md#stockTransportOrderStockTransportOrderStockTransportOrderNoteGet) | **GET** /StockTransportOrder/{StockTransportOrder}/_StockTransportOrderNote | Get entities from related _StockTransportOrderNote |
| [**stockTransportOrderStockTransportOrderStockTransportOrderNotePost()**](StockTransportOrderApi.md#stockTransportOrderStockTransportOrderStockTransportOrderNotePost) | **POST** /StockTransportOrder/{StockTransportOrder}/_StockTransportOrderNote | Add new entity to related _StockTransportOrderNote |
| [**stockTransportOrderStockTransportOrderStockTransportOrderPartnerGet()**](StockTransportOrderApi.md#stockTransportOrderStockTransportOrderStockTransportOrderPartnerGet) | **GET** /StockTransportOrder/{StockTransportOrder}/_StockTransportOrderPartner | Get entities from related _StockTransportOrderPartner |
| [**stockTransportOrderStockTransportOrderStockTransportOrderPartnerPost()**](StockTransportOrderApi.md#stockTransportOrderStockTransportOrderStockTransportOrderPartnerPost) | **POST** /StockTransportOrder/{StockTransportOrder}/_StockTransportOrderPartner | Add new entity to related _StockTransportOrderPartner |


## `sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberStockTransportOrderGet()`

```php
sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberStockTransportOrderGet($stock_transport_order, $stock_transport_order_item, $account_assignment_number, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType
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


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\StockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
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
    echo 'Exception when calling StockTransportOrderApi->sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberStockTransportOrderGet: ', $e->getMessage(), PHP_EOL;
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

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterStockTransportOrderGet()`

```php
sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterStockTransportOrderGet($stock_transport_order, $stock_transport_order_item, $pricing_document, $pricing_document_item, $pricing_procedure_step, $pricing_procedure_counter, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType
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


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\StockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$pricing_document = 'pricing_document_example'; // string | Number of the Document Condition
$pricing_document_item = 'pricing_document_item_example'; // string | Condition item number
$pricing_procedure_step = 'pricing_procedure_step_example'; // string | Step Number
$pricing_procedure_counter = 'pricing_procedure_counter_example'; // string | Condition Counter
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterStockTransportOrderGet($stock_transport_order, $stock_transport_order_item, $pricing_document, $pricing_document_item, $pricing_procedure_step, $pricing_procedure_counter, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StockTransportOrderApi->sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterStockTransportOrderGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **stock_transport_order_item** | **string**| Stock Transport Order Item | |
| **pricing_document** | **string**| Number of the Document Condition | |
| **pricing_document_item** | **string**| Condition item number | |
| **pricing_procedure_step** | **string**| Step Number | |
| **pricing_procedure_counter** | **string**| Condition Counter | |
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


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\StockTransportOrderApi(
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
    echo 'Exception when calling StockTransportOrderApi->sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineStockTransportOrderGet: ', $e->getMessage(), PHP_EOL;
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

## `sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeStockTransportOrderGet()`

```php
sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeStockTransportOrderGet($stock_transport_order, $stock_transport_order_item, $schedule_line, $reservation_item, $record_type, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType
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


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\StockTransportOrderApi(
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
    $result = $apiInstance->sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeStockTransportOrderGet($stock_transport_order, $stock_transport_order_item, $schedule_line, $reservation_item, $record_type, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StockTransportOrderApi->sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeStockTransportOrderGet: ', $e->getMessage(), PHP_EOL;
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

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderGet()`

```php
stockTransportOrderGet($top, $skip, $filter, $count, $orderby, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderType
```

Get entities from StockTransportOrder

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\StockTransportOrderApi(
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
    $result = $apiInstance->stockTransportOrderGet($top, $skip, $filter, $count, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StockTransportOrderApi->stockTransportOrderGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderType**](../Model/CollectionOfStockTransportOrderType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageStockTransportOrderGet()`

```php
stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageStockTransportOrderGet($stock_transport_order, $stock_transport_order_item, $text_object_type, $language, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType
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


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\StockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$text_object_type = 'text_object_type_example'; // string | Text ID
$language = 'language_example'; // string | Language Key
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageStockTransportOrderGet($stock_transport_order, $stock_transport_order_item, $text_object_type, $language, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StockTransportOrderApi->stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageStockTransportOrderGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **stock_transport_order_item** | **string**| Stock Transport Order Item | |
| **text_object_type** | **string**| Text ID | |
| **language** | **string**| Language Key | |
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

## `stockTransportOrderItemStockTransportOrderStockTransportOrderItemStockTransportOrderGet()`

```php
stockTransportOrderItemStockTransportOrderStockTransportOrderItemStockTransportOrderGet($stock_transport_order, $stock_transport_order_item, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType
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


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\StockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->stockTransportOrderItemStockTransportOrderStockTransportOrderItemStockTransportOrderGet($stock_transport_order, $stock_transport_order_item, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StockTransportOrderApi->stockTransportOrderItemStockTransportOrderStockTransportOrderItemStockTransportOrderGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **stock_transport_order_item** | **string**| Stock Transport Order Item | |
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

## `stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageStockTransportOrderGet()`

```php
stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageStockTransportOrderGet($stock_transport_order, $text_object_type, $language, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType
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


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\StockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$text_object_type = 'text_object_type_example'; // string | Text ID
$language = 'language_example'; // string | Language Key
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageStockTransportOrderGet($stock_transport_order, $text_object_type, $language, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StockTransportOrderApi->stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageStockTransportOrderGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **text_object_type** | **string**| Text ID | |
| **language** | **string**| Language Key | |
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

## `stockTransportOrderPartnerStockTransportOrderPartnerFunctionStockTransportOrderGet()`

```php
stockTransportOrderPartnerStockTransportOrderPartnerFunctionStockTransportOrderGet($stock_transport_order, $partner_function, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType
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


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\StockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$partner_function = 'partner_function_example'; // string | Partner Function
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->stockTransportOrderPartnerStockTransportOrderPartnerFunctionStockTransportOrderGet($stock_transport_order, $partner_function, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StockTransportOrderApi->stockTransportOrderPartnerStockTransportOrderPartnerFunctionStockTransportOrderGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **partner_function** | **string**| Partner Function | |
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

## `stockTransportOrderPost()`

```php
stockTransportOrderPost($com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_type_create): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType
```

Add new entity to StockTransportOrder

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\StockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_type_create = new \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderTypeCreate(); // \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderTypeCreate | New entity

try {
    $result = $apiInstance->stockTransportOrderPost($com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_type_create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StockTransportOrderApi->stockTransportOrderPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_type_create** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderTypeCreate**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderTypeCreate.md)| New entity | |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderShippingStockTransportOrderStockTransportOrderItemStockTransportOrderGet()`

```php
stockTransportOrderShippingStockTransportOrderStockTransportOrderItemStockTransportOrderGet($stock_transport_order, $stock_transport_order_item, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType
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


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\StockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->stockTransportOrderShippingStockTransportOrderStockTransportOrderItemStockTransportOrderGet($stock_transport_order, $stock_transport_order_item, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StockTransportOrderApi->stockTransportOrderShippingStockTransportOrderStockTransportOrderItemStockTransportOrderGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **stock_transport_order_item** | **string**| Stock Transport Order Item | |
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

## `stockTransportOrderStockTransportOrderGet()`

```php
stockTransportOrderStockTransportOrderGet($stock_transport_order, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType
```

Get entity from StockTransportOrder by key

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\StockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->stockTransportOrderStockTransportOrderGet($stock_transport_order, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StockTransportOrderApi->stockTransportOrderStockTransportOrderGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
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

## `stockTransportOrderStockTransportOrderPatch()`

```php
stockTransportOrderStockTransportOrderPatch($stock_transport_order, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_type_update): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType
```

Update entity in StockTransportOrder

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\StockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_type_update = new \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderTypeUpdate(); // \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderTypeUpdate | New property values

try {
    $result = $apiInstance->stockTransportOrderStockTransportOrderPatch($stock_transport_order, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_type_update);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StockTransportOrderApi->stockTransportOrderStockTransportOrderPatch: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_type_update** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderTypeUpdate**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderTypeUpdate.md)| New property values | |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderStockTransportOrderSAPSelfBlockAllItemsPost()`

```php
stockTransportOrderStockTransportOrderSAPSelfBlockAllItemsPost($stock_transport_order)
```

Invoke action BlockAllItems

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\StockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order

try {
    $apiInstance->stockTransportOrderStockTransportOrderSAPSelfBlockAllItemsPost($stock_transport_order);
} catch (Exception $e) {
    echo 'Exception when calling StockTransportOrderApi->stockTransportOrderStockTransportOrderSAPSelfBlockAllItemsPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |

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

## `stockTransportOrderStockTransportOrderSAPSelfReadOrderingAddressGet()`

```php
stockTransportOrderStockTransportOrderSAPSelfReadOrderingAddressGet($stock_transport_order): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderReadOrderingAddressResultType
```

Invoke function ReadOrderingAddress

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\StockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order

try {
    $result = $apiInstance->stockTransportOrderStockTransportOrderSAPSelfReadOrderingAddressGet($stock_transport_order);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StockTransportOrderApi->stockTransportOrderStockTransportOrderSAPSelfReadOrderingAddressGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderReadOrderingAddressResultType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderReadOrderingAddressResultType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderStockTransportOrderSAPSelfSetAllItemsToDeletedPost()`

```php
stockTransportOrderStockTransportOrderSAPSelfSetAllItemsToDeletedPost($stock_transport_order)
```

Invoke action SetAllItemsToDeleted

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\StockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order

try {
    $apiInstance->stockTransportOrderStockTransportOrderSAPSelfSetAllItemsToDeletedPost($stock_transport_order);
} catch (Exception $e) {
    echo 'Exception when calling StockTransportOrderApi->stockTransportOrderStockTransportOrderSAPSelfSetAllItemsToDeletedPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |

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

## `stockTransportOrderStockTransportOrderStockTransportOrderItemGet()`

```php
stockTransportOrderStockTransportOrderStockTransportOrderItemGet($stock_transport_order, $top, $skip, $filter, $count, $orderby, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderItemType
```

Get entities from related _StockTransportOrderItem

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\StockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$top = 50; // int | Show only the first n items, see [Paging - Top](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptiontop)
$skip = 56; // int | Skip the first n items, see [Paging - Skip](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionskip)
$filter = 'filter_example'; // string | Filter items by property values, see [Filtering](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionfilter)
$count = True; // bool | Include count of items, see [Count](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptioncount)
$orderby = array('orderby_example'); // string[] | Order items by property values, see [Sorting](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionorderby)
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->stockTransportOrderStockTransportOrderStockTransportOrderItemGet($stock_transport_order, $top, $skip, $filter, $count, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StockTransportOrderApi->stockTransportOrderStockTransportOrderStockTransportOrderItemGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **top** | **int**| Show only the first n items, see [Paging - Top](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptiontop) | [optional] |
| **skip** | **int**| Skip the first n items, see [Paging - Skip](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionskip) | [optional] |
| **filter** | **string**| Filter items by property values, see [Filtering](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionfilter) | [optional] |
| **count** | **bool**| Include count of items, see [Count](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptioncount) | [optional] |
| **orderby** | [**string[]**](../Model/string.md)| Order items by property values, see [Sorting](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionorderby) | [optional] |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand) | [optional] |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderItemType**](../Model/CollectionOfStockTransportOrderItemType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderStockTransportOrderStockTransportOrderItemPost()`

```php
stockTransportOrderStockTransportOrderStockTransportOrderItemPost($stock_transport_order, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_item_type_create): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemType
```

Add new entity to related _StockTransportOrderItem

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\StockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_item_type_create = new \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemTypeCreate(); // \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemTypeCreate | New entity

try {
    $result = $apiInstance->stockTransportOrderStockTransportOrderStockTransportOrderItemPost($stock_transport_order, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_item_type_create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StockTransportOrderApi->stockTransportOrderStockTransportOrderStockTransportOrderItemPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_item_type_create** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemTypeCreate**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemTypeCreate.md)| New entity | |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderStockTransportOrderStockTransportOrderNoteGet()`

```php
stockTransportOrderStockTransportOrderStockTransportOrderNoteGet($stock_transport_order, $top, $skip, $filter, $count, $orderby, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderNoteType
```

Get entities from related _StockTransportOrderNote

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\StockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$top = 50; // int | Show only the first n items, see [Paging - Top](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptiontop)
$skip = 56; // int | Skip the first n items, see [Paging - Skip](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionskip)
$filter = 'filter_example'; // string | Filter items by property values, see [Filtering](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionfilter)
$count = True; // bool | Include count of items, see [Count](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptioncount)
$orderby = array('orderby_example'); // string[] | Order items by property values, see [Sorting](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionorderby)
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->stockTransportOrderStockTransportOrderStockTransportOrderNoteGet($stock_transport_order, $top, $skip, $filter, $count, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StockTransportOrderApi->stockTransportOrderStockTransportOrderStockTransportOrderNoteGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **top** | **int**| Show only the first n items, see [Paging - Top](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptiontop) | [optional] |
| **skip** | **int**| Skip the first n items, see [Paging - Skip](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionskip) | [optional] |
| **filter** | **string**| Filter items by property values, see [Filtering](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionfilter) | [optional] |
| **count** | **bool**| Include count of items, see [Count](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptioncount) | [optional] |
| **orderby** | [**string[]**](../Model/string.md)| Order items by property values, see [Sorting](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionorderby) | [optional] |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand) | [optional] |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderNoteType**](../Model/CollectionOfStockTransportOrderNoteType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderStockTransportOrderStockTransportOrderNotePost()`

```php
stockTransportOrderStockTransportOrderStockTransportOrderNotePost($stock_transport_order, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_note_type_create): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteType
```

Add new entity to related _StockTransportOrderNote

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\StockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_note_type_create = new \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteTypeCreate(); // \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteTypeCreate | New entity

try {
    $result = $apiInstance->stockTransportOrderStockTransportOrderStockTransportOrderNotePost($stock_transport_order, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_note_type_create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StockTransportOrderApi->stockTransportOrderStockTransportOrderStockTransportOrderNotePost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_note_type_create** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteTypeCreate**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteTypeCreate.md)| New entity | |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderStockTransportOrderStockTransportOrderPartnerGet()`

```php
stockTransportOrderStockTransportOrderStockTransportOrderPartnerGet($stock_transport_order, $top, $skip, $filter, $count, $orderby, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderPartnerType
```

Get entities from related _StockTransportOrderPartner

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\StockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$top = 50; // int | Show only the first n items, see [Paging - Top](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptiontop)
$skip = 56; // int | Skip the first n items, see [Paging - Skip](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionskip)
$filter = 'filter_example'; // string | Filter items by property values, see [Filtering](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionfilter)
$count = True; // bool | Include count of items, see [Count](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptioncount)
$orderby = array('orderby_example'); // string[] | Order items by property values, see [Sorting](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionorderby)
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->stockTransportOrderStockTransportOrderStockTransportOrderPartnerGet($stock_transport_order, $top, $skip, $filter, $count, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StockTransportOrderApi->stockTransportOrderStockTransportOrderStockTransportOrderPartnerGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **top** | **int**| Show only the first n items, see [Paging - Top](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptiontop) | [optional] |
| **skip** | **int**| Skip the first n items, see [Paging - Skip](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionskip) | [optional] |
| **filter** | **string**| Filter items by property values, see [Filtering](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionfilter) | [optional] |
| **count** | **bool**| Include count of items, see [Count](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptioncount) | [optional] |
| **orderby** | [**string[]**](../Model/string.md)| Order items by property values, see [Sorting](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionorderby) | [optional] |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand) | [optional] |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderPartnerType**](../Model/CollectionOfStockTransportOrderPartnerType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderStockTransportOrderStockTransportOrderPartnerPost()`

```php
stockTransportOrderStockTransportOrderStockTransportOrderPartnerPost($stock_transport_order, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_partner_type_create): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerType
```

Add new entity to related _StockTransportOrderPartner

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\StockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_partner_type_create = new \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerTypeCreate(); // \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerTypeCreate | New entity

try {
    $result = $apiInstance->stockTransportOrderStockTransportOrderStockTransportOrderPartnerPost($stock_transport_order, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_partner_type_create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StockTransportOrderApi->stockTransportOrderStockTransportOrderStockTransportOrderPartnerPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_partner_type_create** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerTypeCreate**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerTypeCreate.md)| New entity | |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
