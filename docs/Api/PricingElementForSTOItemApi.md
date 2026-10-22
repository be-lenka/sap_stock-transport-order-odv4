# BeLenka\SAP\StockTransportOrderODV4\PricingElementForSTOItemApi

All URIs are relative to https://:/sap/opu/odata4/sap/api_stocktransportorder/srvd_a2x/sap/stocktransportorder/0001, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**sTOItemPricingElementGet()**](PricingElementForSTOItemApi.md#sTOItemPricingElementGet) | **GET** /STOItemPricingElement | Get entities from STOItemPricingElement |
| [**sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterDelete()**](PricingElementForSTOItemApi.md#sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterDelete) | **DELETE** /STOItemPricingElement/{StockTransportOrder}/{StockTransportOrderItem}/{PricingDocument}/{PricingDocumentItem}/{PricingProcedureStep}/{PricingProcedureCounter} | Delete entity from STOItemPricingElement |
| [**sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterGet()**](PricingElementForSTOItemApi.md#sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterGet) | **GET** /STOItemPricingElement/{StockTransportOrder}/{StockTransportOrderItem}/{PricingDocument}/{PricingDocumentItem}/{PricingProcedureStep}/{PricingProcedureCounter} | Get entity from STOItemPricingElement by key |
| [**sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterPatch()**](PricingElementForSTOItemApi.md#sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterPatch) | **PATCH** /STOItemPricingElement/{StockTransportOrder}/{StockTransportOrderItem}/{PricingDocument}/{PricingDocumentItem}/{PricingProcedureStep}/{PricingProcedureCounter} | Update entity in STOItemPricingElement |
| [**sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterStockTransportOrderGet()**](PricingElementForSTOItemApi.md#sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterStockTransportOrderGet) | **GET** /STOItemPricingElement/{StockTransportOrder}/{StockTransportOrderItem}/{PricingDocument}/{PricingDocumentItem}/{PricingProcedureStep}/{PricingProcedureCounter}/_StockTransportOrder | Get related _StockTransportOrder |
| [**sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterStockTransportOrderItemGet()**](PricingElementForSTOItemApi.md#sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterStockTransportOrderItemGet) | **GET** /STOItemPricingElement/{StockTransportOrder}/{StockTransportOrderItem}/{PricingDocument}/{PricingDocumentItem}/{PricingProcedureStep}/{PricingProcedureCounter}/_StockTransportOrderItem | Get related _StockTransportOrderItem |
| [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemPricingElementGet()**](PricingElementForSTOItemApi.md#stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemPricingElementGet) | **GET** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOItemPricingElement | Get entities from related _STOItemPricingElement |
| [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemPricingElementPost()**](PricingElementForSTOItemApi.md#stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemPricingElementPost) | **POST** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOItemPricingElement | Add new entity to related _STOItemPricingElement |


## `sTOItemPricingElementGet()`

```php
sTOItemPricingElementGet($top, $skip, $filter, $count, $orderby, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfSTOPricingElementType
```

Get entities from STOItemPricingElement

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\PricingElementForSTOItemApi(
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
    $result = $apiInstance->sTOItemPricingElementGet($top, $skip, $filter, $count, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PricingElementForSTOItemApi->sTOItemPricingElementGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfSTOPricingElementType**](../Model/CollectionOfSTOPricingElementType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterDelete()`

```php
sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterDelete($stock_transport_order, $stock_transport_order_item, $pricing_document, $pricing_document_item, $pricing_procedure_step, $pricing_procedure_counter)
```

Delete entity from STOItemPricingElement

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\PricingElementForSTOItemApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$pricing_document = 'pricing_document_example'; // string | Number of the Document Condition
$pricing_document_item = 'pricing_document_item_example'; // string | Condition item number
$pricing_procedure_step = 'pricing_procedure_step_example'; // string | Step Number
$pricing_procedure_counter = 'pricing_procedure_counter_example'; // string | Condition Counter

try {
    $apiInstance->sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterDelete($stock_transport_order, $stock_transport_order_item, $pricing_document, $pricing_document_item, $pricing_procedure_step, $pricing_procedure_counter);
} catch (Exception $e) {
    echo 'Exception when calling PricingElementForSTOItemApi->sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterDelete: ', $e->getMessage(), PHP_EOL;
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

## `sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterGet()`

```php
sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterGet($stock_transport_order, $stock_transport_order_item, $pricing_document, $pricing_document_item, $pricing_procedure_step, $pricing_procedure_counter, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementType
```

Get entity from STOItemPricingElement by key

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\PricingElementForSTOItemApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
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
    $result = $apiInstance->sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterGet($stock_transport_order, $stock_transport_order_item, $pricing_document, $pricing_document_item, $pricing_procedure_step, $pricing_procedure_counter, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PricingElementForSTOItemApi->sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterPatch()`

```php
sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterPatch($stock_transport_order, $stock_transport_order_item, $pricing_document, $pricing_document_item, $pricing_procedure_step, $pricing_procedure_counter, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_sto_pricing_element_type_update): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementType
```

Update entity in STOItemPricingElement

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\PricingElementForSTOItemApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$pricing_document = 'pricing_document_example'; // string | Number of the Document Condition
$pricing_document_item = 'pricing_document_item_example'; // string | Condition item number
$pricing_procedure_step = 'pricing_procedure_step_example'; // string | Step Number
$pricing_procedure_counter = 'pricing_procedure_counter_example'; // string | Condition Counter
$com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_sto_pricing_element_type_update = new \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementTypeUpdate(); // \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementTypeUpdate | New property values

try {
    $result = $apiInstance->sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterPatch($stock_transport_order, $stock_transport_order_item, $pricing_document, $pricing_document_item, $pricing_procedure_step, $pricing_procedure_counter, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_sto_pricing_element_type_update);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PricingElementForSTOItemApi->sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterPatch: ', $e->getMessage(), PHP_EOL;
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
| **com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_sto_pricing_element_type_update** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementTypeUpdate**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementTypeUpdate.md)| New property values | |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
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



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\PricingElementForSTOItemApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
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
    echo 'Exception when calling PricingElementForSTOItemApi->sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterStockTransportOrderGet: ', $e->getMessage(), PHP_EOL;
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

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterStockTransportOrderItemGet()`

```php
sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterStockTransportOrderItemGet($stock_transport_order, $stock_transport_order_item, $pricing_document, $pricing_document_item, $pricing_procedure_step, $pricing_procedure_counter, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemType
```

Get related _StockTransportOrderItem

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\PricingElementForSTOItemApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
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
    $result = $apiInstance->sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterStockTransportOrderItemGet($stock_transport_order, $stock_transport_order_item, $pricing_document, $pricing_document_item, $pricing_procedure_step, $pricing_procedure_counter, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PricingElementForSTOItemApi->sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterStockTransportOrderItemGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemPricingElementGet()`

```php
stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemPricingElementGet($stock_transport_order, $stock_transport_order_item, $top, $skip, $filter, $count, $orderby, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfSTOPricingElementType
```

Get entities from related _STOItemPricingElement

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\PricingElementForSTOItemApi(
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
    $result = $apiInstance->stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemPricingElementGet($stock_transport_order, $stock_transport_order_item, $top, $skip, $filter, $count, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PricingElementForSTOItemApi->stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemPricingElementGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfSTOPricingElementType**](../Model/CollectionOfSTOPricingElementType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemPricingElementPost()`

```php
stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemPricingElementPost($stock_transport_order, $stock_transport_order_item, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_sto_pricing_element_type_create): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementType
```

Add new entity to related _STOItemPricingElement

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\PricingElementForSTOItemApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_sto_pricing_element_type_create = new \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementTypeCreate(); // \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementTypeCreate | New entity

try {
    $result = $apiInstance->stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemPricingElementPost($stock_transport_order, $stock_transport_order_item, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_sto_pricing_element_type_create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PricingElementForSTOItemApi->stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemPricingElementPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **stock_transport_order_item** | **string**| Stock Transport Order Item | |
| **com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_sto_pricing_element_type_create** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementTypeCreate**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementTypeCreate.md)| New entity | |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
