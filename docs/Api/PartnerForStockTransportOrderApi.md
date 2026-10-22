# BeLenka\SAP\StockTransportOrderODV4\PartnerForStockTransportOrderApi

All URIs are relative to https://:/sap/opu/odata4/sap/api_stocktransportorder/srvd_a2x/sap/stocktransportorder/0001, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**stockTransportOrderPartnerGet()**](PartnerForStockTransportOrderApi.md#stockTransportOrderPartnerGet) | **GET** /StockTransportOrderPartner | Get entities from StockTransportOrderPartner |
| [**stockTransportOrderPartnerStockTransportOrderPartnerFunctionDelete()**](PartnerForStockTransportOrderApi.md#stockTransportOrderPartnerStockTransportOrderPartnerFunctionDelete) | **DELETE** /StockTransportOrderPartner/{StockTransportOrder}/{PartnerFunction} | Delete entity from StockTransportOrderPartner |
| [**stockTransportOrderPartnerStockTransportOrderPartnerFunctionGet()**](PartnerForStockTransportOrderApi.md#stockTransportOrderPartnerStockTransportOrderPartnerFunctionGet) | **GET** /StockTransportOrderPartner/{StockTransportOrder}/{PartnerFunction} | Get entity from StockTransportOrderPartner by key |
| [**stockTransportOrderPartnerStockTransportOrderPartnerFunctionPatch()**](PartnerForStockTransportOrderApi.md#stockTransportOrderPartnerStockTransportOrderPartnerFunctionPatch) | **PATCH** /StockTransportOrderPartner/{StockTransportOrder}/{PartnerFunction} | Update entity in StockTransportOrderPartner |
| [**stockTransportOrderPartnerStockTransportOrderPartnerFunctionStockTransportOrderGet()**](PartnerForStockTransportOrderApi.md#stockTransportOrderPartnerStockTransportOrderPartnerFunctionStockTransportOrderGet) | **GET** /StockTransportOrderPartner/{StockTransportOrder}/{PartnerFunction}/_StockTransportOrder | Get related _StockTransportOrder |
| [**stockTransportOrderStockTransportOrderStockTransportOrderPartnerGet()**](PartnerForStockTransportOrderApi.md#stockTransportOrderStockTransportOrderStockTransportOrderPartnerGet) | **GET** /StockTransportOrder/{StockTransportOrder}/_StockTransportOrderPartner | Get entities from related _StockTransportOrderPartner |
| [**stockTransportOrderStockTransportOrderStockTransportOrderPartnerPost()**](PartnerForStockTransportOrderApi.md#stockTransportOrderStockTransportOrderStockTransportOrderPartnerPost) | **POST** /StockTransportOrder/{StockTransportOrder}/_StockTransportOrderPartner | Add new entity to related _StockTransportOrderPartner |


## `stockTransportOrderPartnerGet()`

```php
stockTransportOrderPartnerGet($top, $skip, $filter, $count, $orderby, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderPartnerType
```

Get entities from StockTransportOrderPartner

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\PartnerForStockTransportOrderApi(
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
    $result = $apiInstance->stockTransportOrderPartnerGet($top, $skip, $filter, $count, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerForStockTransportOrderApi->stockTransportOrderPartnerGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\StockTransportOrderODV4\Model\CollectionOfStockTransportOrderPartnerType**](../Model/CollectionOfStockTransportOrderPartnerType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderPartnerStockTransportOrderPartnerFunctionDelete()`

```php
stockTransportOrderPartnerStockTransportOrderPartnerFunctionDelete($stock_transport_order, $partner_function)
```

Delete entity from StockTransportOrderPartner

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\PartnerForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$partner_function = 'partner_function_example'; // string | Partner Function

try {
    $apiInstance->stockTransportOrderPartnerStockTransportOrderPartnerFunctionDelete($stock_transport_order, $partner_function);
} catch (Exception $e) {
    echo 'Exception when calling PartnerForStockTransportOrderApi->stockTransportOrderPartnerStockTransportOrderPartnerFunctionDelete: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **partner_function** | **string**| Partner Function | |

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

## `stockTransportOrderPartnerStockTransportOrderPartnerFunctionGet()`

```php
stockTransportOrderPartnerStockTransportOrderPartnerFunctionGet($stock_transport_order, $partner_function, $select, $expand): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerType
```

Get entity from StockTransportOrderPartner by key

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\PartnerForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$partner_function = 'partner_function_example'; // string | Partner Function
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->stockTransportOrderPartnerStockTransportOrderPartnerFunctionGet($stock_transport_order, $partner_function, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerForStockTransportOrderApi->stockTransportOrderPartnerStockTransportOrderPartnerFunctionGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `stockTransportOrderPartnerStockTransportOrderPartnerFunctionPatch()`

```php
stockTransportOrderPartnerStockTransportOrderPartnerFunctionPatch($stock_transport_order, $partner_function, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_partner_type_update): \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerType
```

Update entity in StockTransportOrderPartner

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\PartnerForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$partner_function = 'partner_function_example'; // string | Partner Function
$com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_partner_type_update = new \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerTypeUpdate(); // \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerTypeUpdate | New property values

try {
    $result = $apiInstance->stockTransportOrderPartnerStockTransportOrderPartnerFunctionPatch($stock_transport_order, $partner_function, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_partner_type_update);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerForStockTransportOrderApi->stockTransportOrderPartnerStockTransportOrderPartnerFunctionPatch: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stock_transport_order** | **string**| Stock Transport Order | |
| **partner_function** | **string**| Partner Function | |
| **com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_partner_type_update** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerTypeUpdate**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerTypeUpdate.md)| New property values | |

### Return type

[**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerType**](../Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerType.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
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



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\PartnerForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$partner_function = 'partner_function_example'; // string | Partner Function
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionselect)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part1-protocol.html#sec_SystemQueryOptionexpand)

try {
    $result = $apiInstance->stockTransportOrderPartnerStockTransportOrderPartnerFunctionStockTransportOrderGet($stock_transport_order, $partner_function, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerForStockTransportOrderApi->stockTransportOrderPartnerStockTransportOrderPartnerFunctionStockTransportOrderGet: ', $e->getMessage(), PHP_EOL;
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

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
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



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\PartnerForStockTransportOrderApi(
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
    $result = $apiInstance->stockTransportOrderStockTransportOrderStockTransportOrderPartnerGet($stock_transport_order, $top, $skip, $filter, $count, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerForStockTransportOrderApi->stockTransportOrderStockTransportOrderStockTransportOrderPartnerGet: ', $e->getMessage(), PHP_EOL;
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

No authorization required

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



$apiInstance = new BeLenka\SAP\StockTransportOrderODV4\Api\PartnerForStockTransportOrderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$stock_transport_order = 'stock_transport_order_example'; // string | Stock Transport Order
$com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_partner_type_create = new \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerTypeCreate(); // \BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerTypeCreate | New entity

try {
    $result = $apiInstance->stockTransportOrderStockTransportOrderStockTransportOrderPartnerPost($stock_transport_order, $com_sap_gateway_srvd_a2x_api_stocktransportorder_v0001_stock_transport_order_partner_type_create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerForStockTransportOrderApi->stockTransportOrderStockTransportOrderStockTransportOrderPartnerPost: ', $e->getMessage(), PHP_EOL;
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

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
