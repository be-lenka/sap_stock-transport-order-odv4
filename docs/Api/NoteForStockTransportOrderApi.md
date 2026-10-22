# BeLenka\SAP\StockTransportOrderODV4\NoteForStockTransportOrderApi

All URIs are relative to https://:/sap/opu/odata4/sap/api_stocktransportorder/srvd_a2x/sap/stocktransportorder/0001, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**stockTransportOrderNoteGet()**](NoteForStockTransportOrderApi.md#stockTransportOrderNoteGet) | **GET** /StockTransportOrderNote | Get entities from StockTransportOrderNote |
| [**stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageDelete()**](NoteForStockTransportOrderApi.md#stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageDelete) | **DELETE** /StockTransportOrderNote/{StockTransportOrder}/{TextObjectType}/{Language} | Delete entity from StockTransportOrderNote |
| [**stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageGet()**](NoteForStockTransportOrderApi.md#stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageGet) | **GET** /StockTransportOrderNote/{StockTransportOrder}/{TextObjectType}/{Language} | Get entity from StockTransportOrderNote by key |
| [**stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguagePatch()**](NoteForStockTransportOrderApi.md#stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguagePatch) | **PATCH** /StockTransportOrderNote/{StockTransportOrder}/{TextObjectType}/{Language} | Update entity in StockTransportOrderNote |
| [**stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageStockTransportOrderGet()**](NoteForStockTransportOrderApi.md#stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageStockTransportOrderGet) | **GET** /StockTransportOrderNote/{StockTransportOrder}/{TextObjectType}/{Language}/_StockTransportOrder | Get related _StockTransportOrder |
| [**stockTransportOrderStockTransportOrderStockTransportOrderNoteGet()**](NoteForStockTransportOrderApi.md#stockTransportOrderStockTransportOrderStockTransportOrderNoteGet) | **GET** /StockTransportOrder/{StockTransportOrder}/_StockTransportOrderNote | Get entities from related _StockTransportOrderNote |
| [**stockTransportOrderStockTransportOrderStockTransportOrderNotePost()**](NoteForStockTransportOrderApi.md#stockTransportOrderStockTransportOrderStockTransportOrderNotePost) | **POST** /StockTransportOrder/{StockTransportOrder}/_StockTransportOrderNote | Add new entity to related _StockTransportOrderNote |


## `stockTransportOrderNoteGet()`

```php
stockTransportOrderNoteGet($top, $skip, $filter, $count, $orderby, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderNoteType
```

Get entities from StockTransportOrderNote

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\NoteForStockTransportOrderApi(
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
    $result = $apiInstance->stockTransportOrderNoteGet($top, $skip, $filter, $count, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling NoteForStockTransportOrderApi->stockTransportOrderNoteGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderNoteType**](../Model/CollectionOfStockTransportOrderNoteType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageDelete()`

```php
stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageDelete($stock_transport_order, $text_object_type, $language)
```

Delete entity from StockTransportOrderNote

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\NoteForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$text_object_type = 'text_object_type_example'; // string | Text ID
$language = 'language_example'; // string | Language Key

try {
    $apiInstance->stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageDelete($stock_transport_order, $text_object_type, $language);
} catch (Exception $e) {
    echo 'Exception when calling NoteForStockTransportOrderApi->stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageDelete: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **text_object_type** | **string**| Text ID | |
| **language** | **string**| Language Key | |

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

## `stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageGet()`

```php
stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageGet($stock_transport_order, $text_object_type, $language, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteType
```

Get entity from StockTransportOrderNote by key

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\NoteForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$text_object_type = 'text_object_type_example'; // string | Text ID
$language = 'language_example'; // string | Language Key
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageGet($stock_transport_order, $text_object_type, $language, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling NoteForStockTransportOrderApi->stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguagePatch()`

```php
stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguagePatch($stock_transport_order, $text_object_type, $language, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_note_type_update): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteType
```

Update entity in StockTransportOrderNote

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\NoteForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$text_object_type = 'text_object_type_example'; // string | Text ID
$language = 'language_example'; // string | Language Key
$com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_note_type_update = new \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteTypeUpdate(); // \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteTypeUpdate | New property values

try {
    $result = $apiInstance->stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguagePatch($stock_transport_order, $text_object_type, $language, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_note_type_update);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling NoteForStockTransportOrderApi->stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguagePatch: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **text_object_type** | **string**| Text ID | |
| **language** | **string**| Language Key | |
| **com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_note_type_update** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteTypeUpdate**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteTypeUpdate.md)| New property values | |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
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



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\NoteForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
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
    echo 'Exception when calling NoteForStockTransportOrderApi->stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageStockTransportOrderGet: ', $e->getMessage(), PHP_EOL;
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

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
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



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\NoteForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
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
    echo 'Exception when calling NoteForStockTransportOrderApi->stockTransportOrderStockTransportOrderStockTransportOrderNoteGet: ', $e->getMessage(), PHP_EOL;
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

No authorization required

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



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\NoteForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_note_type_create = new \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteTypeCreate(); // \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteTypeCreate | New entity

try {
    $result = $apiInstance->stockTransportOrderStockTransportOrderStockTransportOrderNotePost($stock_transport_order, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_note_type_create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling NoteForStockTransportOrderApi->stockTransportOrderStockTransportOrderStockTransportOrderNotePost: ', $e->getMessage(), PHP_EOL;
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

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
