# BeLenka\SAP\StockTransportOrderODV4\ItemNoteForStockTransportOrderApi

All URIs are relative to https://:/sap/opu/odata4/sap/api_stocktransportorder/srvd_a2x/sap/stocktransportorder/0001, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**stockTransportOrderItemNoteGet()**](ItemNoteForStockTransportOrderApi.md#stockTransportOrderItemNoteGet) | **GET** /StockTransportOrderItemNote | Get entities from StockTransportOrderItemNote |
| [**stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageDelete()**](ItemNoteForStockTransportOrderApi.md#stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageDelete) | **DELETE** /StockTransportOrderItemNote/{StockTransportOrder}/{StockTransportOrderItem}/{TextObjectType}/{Language} | Delete entity from StockTransportOrderItemNote |
| [**stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageGet()**](ItemNoteForStockTransportOrderApi.md#stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageGet) | **GET** /StockTransportOrderItemNote/{StockTransportOrder}/{StockTransportOrderItem}/{TextObjectType}/{Language} | Get entity from StockTransportOrderItemNote by key |
| [**stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguagePatch()**](ItemNoteForStockTransportOrderApi.md#stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguagePatch) | **PATCH** /StockTransportOrderItemNote/{StockTransportOrder}/{StockTransportOrderItem}/{TextObjectType}/{Language} | Update entity in StockTransportOrderItemNote |
| [**stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageStockTransportOrderGet()**](ItemNoteForStockTransportOrderApi.md#stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageStockTransportOrderGet) | **GET** /StockTransportOrderItemNote/{StockTransportOrder}/{StockTransportOrderItem}/{TextObjectType}/{Language}/_StockTransportOrder | Get related _StockTransportOrder |
| [**stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageStockTransportOrderItemGet()**](ItemNoteForStockTransportOrderApi.md#stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageStockTransportOrderItemGet) | **GET** /StockTransportOrderItemNote/{StockTransportOrder}/{StockTransportOrderItem}/{TextObjectType}/{Language}/_StockTransportOrderItem | Get related _StockTransportOrderItem |
| [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemNoteGet()**](ItemNoteForStockTransportOrderApi.md#stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemNoteGet) | **GET** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOItemNote | Get entities from related _STOItemNote |
| [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemNotePost()**](ItemNoteForStockTransportOrderApi.md#stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemNotePost) | **POST** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOItemNote | Add new entity to related _STOItemNote |


## `stockTransportOrderItemNoteGet()`

```php
stockTransportOrderItemNoteGet($top, $skip, $filter, $count, $orderby, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderItemNoteType
```

Get entities from StockTransportOrderItemNote

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\ItemNoteForStockTransportOrderApi(
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
    $result = $apiInstance->stockTransportOrderItemNoteGet($top, $skip, $filter, $count, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ItemNoteForStockTransportOrderApi->stockTransportOrderItemNoteGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderItemNoteType**](../Model/CollectionOfStockTransportOrderItemNoteType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageDelete()`

```php
stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageDelete($stock_transport_order, $stock_transport_order_item, $text_object_type, $language)
```

Delete entity from StockTransportOrderItemNote

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\ItemNoteForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$text_object_type = 'text_object_type_example'; // string | Text ID
$language = 'language_example'; // string | Language Key

try {
    $apiInstance->stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageDelete($stock_transport_order, $stock_transport_order_item, $text_object_type, $language);
} catch (Exception $e) {
    echo 'Exception when calling ItemNoteForStockTransportOrderApi->stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageDelete: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **stock_transport_order_item** | **string**| Stock Transport Order Item | |
| **text_object_type** | **string**| Text ID | |
| **language** | **string**| Language Key | |

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

## `stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageGet()`

```php
stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageGet($stock_transport_order, $stock_transport_order_item, $text_object_type, $language, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteType
```

Get entity from StockTransportOrderItemNote by key

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\ItemNoteForStockTransportOrderApi(
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
    $result = $apiInstance->stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageGet($stock_transport_order, $stock_transport_order_item, $text_object_type, $language, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ItemNoteForStockTransportOrderApi->stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguagePatch()`

```php
stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguagePatch($stock_transport_order, $stock_transport_order_item, $text_object_type, $language, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_item_note_type_update): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteType
```

Update entity in StockTransportOrderItemNote

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\ItemNoteForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$text_object_type = 'text_object_type_example'; // string | Text ID
$language = 'language_example'; // string | Language Key
$com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_item_note_type_update = new \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteTypeUpdate(); // \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteTypeUpdate | New property values

try {
    $result = $apiInstance->stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguagePatch($stock_transport_order, $stock_transport_order_item, $text_object_type, $language, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_item_note_type_update);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ItemNoteForStockTransportOrderApi->stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguagePatch: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **stock_transport_order_item** | **string**| Stock Transport Order Item | |
| **text_object_type** | **string**| Text ID | |
| **language** | **string**| Language Key | |
| **com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_item_note_type_update** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteTypeUpdate**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteTypeUpdate.md)| New property values | |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: `application/json`
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


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\ItemNoteForStockTransportOrderApi(
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
    echo 'Exception when calling ItemNoteForStockTransportOrderApi->stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageStockTransportOrderGet: ', $e->getMessage(), PHP_EOL;
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

## `stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageStockTransportOrderItemGet()`

```php
stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageStockTransportOrderItemGet($stock_transport_order, $stock_transport_order_item, $text_object_type, $language, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemType
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


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\ItemNoteForStockTransportOrderApi(
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
    $result = $apiInstance->stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageStockTransportOrderItemGet($stock_transport_order, $stock_transport_order_item, $text_object_type, $language, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ItemNoteForStockTransportOrderApi->stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageStockTransportOrderItemGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemNoteGet()`

```php
stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemNoteGet($stock_transport_order, $stock_transport_order_item, $top, $skip, $filter, $count, $orderby, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderItemNoteType
```

Get entities from related _STOItemNote

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\ItemNoteForStockTransportOrderApi(
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
    $result = $apiInstance->stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemNoteGet($stock_transport_order, $stock_transport_order_item, $top, $skip, $filter, $count, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ItemNoteForStockTransportOrderApi->stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemNoteGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderItemNoteType**](../Model/CollectionOfStockTransportOrderItemNoteType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemNotePost()`

```php
stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemNotePost($stock_transport_order, $stock_transport_order_item, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_item_note_type_create): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteType
```

Add new entity to related _STOItemNote

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuthentication
$config = BeLenka\SAP\StockTransportOrderODV4\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\ItemNoteForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$stock_transport_order_item = 'stock_transport_order_item_example'; // string | Stock Transport Order Item
$com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_item_note_type_create = new \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteTypeCreate(); // \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteTypeCreate | New entity

try {
    $result = $apiInstance->stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemNotePost($stock_transport_order, $stock_transport_order_item, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_item_note_type_create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ItemNoteForStockTransportOrderApi->stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemNotePost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **stock_transport_order_item** | **string**| Stock Transport Order Item | |
| **com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_item_note_type_create** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteTypeCreate**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteTypeCreate.md)| New entity | |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteType.md)

### Authorization

[basicAuthentication](../../README.md#basicAuthentication)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
