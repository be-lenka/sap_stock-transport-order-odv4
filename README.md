# OpenAPIClient-php

This service enables you to create stock transport orders through an API call from a source service outside the SAP S/4HANA Cloud Public Edition system. Furthermore, the service enables you to read, update or delete stock transport orders. This service is based on the OData V4 protocol.


## Installation & Usage

### Requirements

PHP 7.4 and later.
Should also work with PHP 8.0.

### Composer

To install the bindings via [Composer](https://getcomposer.org/), add the following to `composer.json`:

```json
{
  "repositories": [
    {
      "type": "vcs",
      "url": "https://github.com/GIT_USER_ID/GIT_REPO_ID.git"
    }
  ],
  "require": {
    "GIT_USER_ID/GIT_REPO_ID": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
<?php
require_once('/path/to/OpenAPIClient-php/vendor/autoload.php');
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

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

## API Endpoints

All URIs are relative to *https://:/sap/opu/odata4/sap/api_stocktransportorder/srvd_a2x/sap/stocktransportorder/0001*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AccountAssignmentForSTOApi* | [**sTOAccountAssignmentGet**](docs/Api/AccountAssignmentForSTOApi.md#stoaccountassignmentget) | **GET** /STOAccountAssignment | Get entities from STOAccountAssignment
*AccountAssignmentForSTOApi* | [**sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberDelete**](docs/Api/AccountAssignmentForSTOApi.md#stoaccountassignmentstocktransportorderstocktransportorderitemaccountassignmentnumberdelete) | **DELETE** /STOAccountAssignment/{StockTransportOrder}/{StockTransportOrderItem}/{AccountAssignmentNumber} | Delete entity from STOAccountAssignment
*AccountAssignmentForSTOApi* | [**sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberGet**](docs/Api/AccountAssignmentForSTOApi.md#stoaccountassignmentstocktransportorderstocktransportorderitemaccountassignmentnumberget) | **GET** /STOAccountAssignment/{StockTransportOrder}/{StockTransportOrderItem}/{AccountAssignmentNumber} | Get entity from STOAccountAssignment by key
*AccountAssignmentForSTOApi* | [**sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberPatch**](docs/Api/AccountAssignmentForSTOApi.md#stoaccountassignmentstocktransportorderstocktransportorderitemaccountassignmentnumberpatch) | **PATCH** /STOAccountAssignment/{StockTransportOrder}/{StockTransportOrderItem}/{AccountAssignmentNumber} | Update entity in STOAccountAssignment
*AccountAssignmentForSTOApi* | [**sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberStockTransportOrderGet**](docs/Api/AccountAssignmentForSTOApi.md#stoaccountassignmentstocktransportorderstocktransportorderitemaccountassignmentnumberstocktransportorderget) | **GET** /STOAccountAssignment/{StockTransportOrder}/{StockTransportOrderItem}/{AccountAssignmentNumber}/_StockTransportOrder | Get related _StockTransportOrder
*AccountAssignmentForSTOApi* | [**sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberStockTransportOrderItemGet**](docs/Api/AccountAssignmentForSTOApi.md#stoaccountassignmentstocktransportorderstocktransportorderitemaccountassignmentnumberstocktransportorderitemget) | **GET** /STOAccountAssignment/{StockTransportOrder}/{StockTransportOrderItem}/{AccountAssignmentNumber}/_StockTransportOrderItem | Get related _StockTransportOrderItem
*AccountAssignmentForSTOApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOAccountAssignmentGet**](docs/Api/AccountAssignmentForSTOApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemstoaccountassignmentget) | **GET** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOAccountAssignment | Get entities from related _STOAccountAssignment
*AccountAssignmentForSTOApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOAccountAssignmentPost**](docs/Api/AccountAssignmentForSTOApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemstoaccountassignmentpost) | **POST** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOAccountAssignment | Add new entity to related _STOAccountAssignment
*BatchRequestsApi* | [**batchPost**](docs/Api/BatchRequestsApi.md#batchpost) | **POST** /$batch | Send a group of requests
*ItemInStockTransportOrderApi* | [**sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberStockTransportOrderItemGet**](docs/Api/ItemInStockTransportOrderApi.md#stoaccountassignmentstocktransportorderstocktransportorderitemaccountassignmentnumberstocktransportorderitemget) | **GET** /STOAccountAssignment/{StockTransportOrder}/{StockTransportOrderItem}/{AccountAssignmentNumber}/_StockTransportOrderItem | Get related _StockTransportOrderItem
*ItemInStockTransportOrderApi* | [**sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterStockTransportOrderItemGet**](docs/Api/ItemInStockTransportOrderApi.md#stoitempricingelementstocktransportorderstocktransportorderitempricingdocumentpricingdocumentitempricingproceduresteppricingprocedurecounterstocktransportorderitemget) | **GET** /STOItemPricingElement/{StockTransportOrder}/{StockTransportOrderItem}/{PricingDocument}/{PricingDocumentItem}/{PricingProcedureStep}/{PricingProcedureCounter}/_StockTransportOrderItem | Get related _StockTransportOrderItem
*ItemInStockTransportOrderApi* | [**sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineStockTransportOrderItemGet**](docs/Api/ItemInStockTransportOrderApi.md#stoschedulelinestocktransportorderstocktransportorderitemschedulelinestocktransportorderitemget) | **GET** /STOScheduleLine/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/_StockTransportOrderItem | Get related _StockTransportOrderItem
*ItemInStockTransportOrderApi* | [**sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeStockTransportOrderItemGet**](docs/Api/ItemInStockTransportOrderApi.md#stosubcontractingcomponentstocktransportorderstocktransportorderitemschedulelinereservationitemrecordtypestocktransportorderitemget) | **GET** /STOSubcontractingComponent/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/{ReservationItem}/{RecordType}/_StockTransportOrderItem | Get related _StockTransportOrderItem
*ItemInStockTransportOrderApi* | [**stockTransportOrderItemGet**](docs/Api/ItemInStockTransportOrderApi.md#stocktransportorderitemget) | **GET** /StockTransportOrderItem | Get entities from StockTransportOrderItem
*ItemInStockTransportOrderApi* | [**stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageStockTransportOrderItemGet**](docs/Api/ItemInStockTransportOrderApi.md#stocktransportorderitemnotestocktransportorderstocktransportorderitemtextobjecttypelanguagestocktransportorderitemget) | **GET** /StockTransportOrderItemNote/{StockTransportOrder}/{StockTransportOrderItem}/{TextObjectType}/{Language}/_StockTransportOrderItem | Get related _StockTransportOrderItem
*ItemInStockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemGet**](docs/Api/ItemInStockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemget) | **GET** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem} | Get entity from StockTransportOrderItem by key
*ItemInStockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemPatch**](docs/Api/ItemInStockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitempatch) | **PATCH** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem} | Update entity in StockTransportOrderItem
*ItemInStockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSAPSelfBlockItemPost**](docs/Api/ItemInStockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemsapselfblockitempost) | **POST** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/SAP__self.BlockItem | Invoke action BlockItem
*ItemInStockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSAPSelfReadDeliveryAddressGet**](docs/Api/ItemInStockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemsapselfreaddeliveryaddressget) | **GET** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/SAP__self.ReadDeliveryAddress() | Invoke function ReadDeliveryAddress
*ItemInStockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSAPSelfSetItemToDeletedPost**](docs/Api/ItemInStockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemsapselfsetitemtodeletedpost) | **POST** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/SAP__self.SetItemToDeleted | Invoke action SetItemToDeleted
*ItemInStockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSAPSelfSetItemToNotDeletedPost**](docs/Api/ItemInStockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemsapselfsetitemtonotdeletedpost) | **POST** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/SAP__self.SetItemToNotDeleted | Invoke action SetItemToNotDeleted
*ItemInStockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSAPSelfUnblockItemPost**](docs/Api/ItemInStockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemsapselfunblockitempost) | **POST** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/SAP__self.UnblockItem | Invoke action UnblockItem
*ItemInStockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOAccountAssignmentGet**](docs/Api/ItemInStockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemstoaccountassignmentget) | **GET** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOAccountAssignment | Get entities from related _STOAccountAssignment
*ItemInStockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOAccountAssignmentPost**](docs/Api/ItemInStockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemstoaccountassignmentpost) | **POST** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOAccountAssignment | Add new entity to related _STOAccountAssignment
*ItemInStockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemNoteGet**](docs/Api/ItemInStockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemstoitemnoteget) | **GET** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOItemNote | Get entities from related _STOItemNote
*ItemInStockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemNotePost**](docs/Api/ItemInStockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemstoitemnotepost) | **POST** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOItemNote | Add new entity to related _STOItemNote
*ItemInStockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemPricingElementGet**](docs/Api/ItemInStockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemstoitempricingelementget) | **GET** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOItemPricingElement | Get entities from related _STOItemPricingElement
*ItemInStockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemPricingElementPost**](docs/Api/ItemInStockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemstoitempricingelementpost) | **POST** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOItemPricingElement | Add new entity to related _STOItemPricingElement
*ItemInStockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOScheduleLineGet**](docs/Api/ItemInStockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemstoschedulelineget) | **GET** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOScheduleLine | Get entities from related _STOScheduleLine
*ItemInStockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOScheduleLinePost**](docs/Api/ItemInStockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemstoschedulelinepost) | **POST** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOScheduleLine | Add new entity to related _STOScheduleLine
*ItemInStockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOShippingGet**](docs/Api/ItemInStockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemstoshippingget) | **GET** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOShipping | Get related _STOShipping
*ItemInStockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemStockTransportOrderGet**](docs/Api/ItemInStockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemstocktransportorderget) | **GET** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_StockTransportOrder | Get related _StockTransportOrder
*ItemInStockTransportOrderApi* | [**stockTransportOrderShippingStockTransportOrderStockTransportOrderItemStockTransportOrderItemGet**](docs/Api/ItemInStockTransportOrderApi.md#stocktransportordershippingstocktransportorderstocktransportorderitemstocktransportorderitemget) | **GET** /StockTransportOrderShipping/{StockTransportOrder}/{StockTransportOrderItem}/_StockTransportOrderItem | Get related _StockTransportOrderItem
*ItemInStockTransportOrderApi* | [**stockTransportOrderStockTransportOrderStockTransportOrderItemGet**](docs/Api/ItemInStockTransportOrderApi.md#stocktransportorderstocktransportorderstocktransportorderitemget) | **GET** /StockTransportOrder/{StockTransportOrder}/_StockTransportOrderItem | Get entities from related _StockTransportOrderItem
*ItemInStockTransportOrderApi* | [**stockTransportOrderStockTransportOrderStockTransportOrderItemPost**](docs/Api/ItemInStockTransportOrderApi.md#stocktransportorderstocktransportorderstocktransportorderitempost) | **POST** /StockTransportOrder/{StockTransportOrder}/_StockTransportOrderItem | Add new entity to related _StockTransportOrderItem
*ItemNoteForStockTransportOrderApi* | [**stockTransportOrderItemNoteGet**](docs/Api/ItemNoteForStockTransportOrderApi.md#stocktransportorderitemnoteget) | **GET** /StockTransportOrderItemNote | Get entities from StockTransportOrderItemNote
*ItemNoteForStockTransportOrderApi* | [**stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageDelete**](docs/Api/ItemNoteForStockTransportOrderApi.md#stocktransportorderitemnotestocktransportorderstocktransportorderitemtextobjecttypelanguagedelete) | **DELETE** /StockTransportOrderItemNote/{StockTransportOrder}/{StockTransportOrderItem}/{TextObjectType}/{Language} | Delete entity from StockTransportOrderItemNote
*ItemNoteForStockTransportOrderApi* | [**stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageGet**](docs/Api/ItemNoteForStockTransportOrderApi.md#stocktransportorderitemnotestocktransportorderstocktransportorderitemtextobjecttypelanguageget) | **GET** /StockTransportOrderItemNote/{StockTransportOrder}/{StockTransportOrderItem}/{TextObjectType}/{Language} | Get entity from StockTransportOrderItemNote by key
*ItemNoteForStockTransportOrderApi* | [**stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguagePatch**](docs/Api/ItemNoteForStockTransportOrderApi.md#stocktransportorderitemnotestocktransportorderstocktransportorderitemtextobjecttypelanguagepatch) | **PATCH** /StockTransportOrderItemNote/{StockTransportOrder}/{StockTransportOrderItem}/{TextObjectType}/{Language} | Update entity in StockTransportOrderItemNote
*ItemNoteForStockTransportOrderApi* | [**stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageStockTransportOrderGet**](docs/Api/ItemNoteForStockTransportOrderApi.md#stocktransportorderitemnotestocktransportorderstocktransportorderitemtextobjecttypelanguagestocktransportorderget) | **GET** /StockTransportOrderItemNote/{StockTransportOrder}/{StockTransportOrderItem}/{TextObjectType}/{Language}/_StockTransportOrder | Get related _StockTransportOrder
*ItemNoteForStockTransportOrderApi* | [**stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageStockTransportOrderItemGet**](docs/Api/ItemNoteForStockTransportOrderApi.md#stocktransportorderitemnotestocktransportorderstocktransportorderitemtextobjecttypelanguagestocktransportorderitemget) | **GET** /StockTransportOrderItemNote/{StockTransportOrder}/{StockTransportOrderItem}/{TextObjectType}/{Language}/_StockTransportOrderItem | Get related _StockTransportOrderItem
*ItemNoteForStockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemNoteGet**](docs/Api/ItemNoteForStockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemstoitemnoteget) | **GET** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOItemNote | Get entities from related _STOItemNote
*ItemNoteForStockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemNotePost**](docs/Api/ItemNoteForStockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemstoitemnotepost) | **POST** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOItemNote | Add new entity to related _STOItemNote
*NoteForStockTransportOrderApi* | [**stockTransportOrderNoteGet**](docs/Api/NoteForStockTransportOrderApi.md#stocktransportordernoteget) | **GET** /StockTransportOrderNote | Get entities from StockTransportOrderNote
*NoteForStockTransportOrderApi* | [**stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageDelete**](docs/Api/NoteForStockTransportOrderApi.md#stocktransportordernotestocktransportordertextobjecttypelanguagedelete) | **DELETE** /StockTransportOrderNote/{StockTransportOrder}/{TextObjectType}/{Language} | Delete entity from StockTransportOrderNote
*NoteForStockTransportOrderApi* | [**stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageGet**](docs/Api/NoteForStockTransportOrderApi.md#stocktransportordernotestocktransportordertextobjecttypelanguageget) | **GET** /StockTransportOrderNote/{StockTransportOrder}/{TextObjectType}/{Language} | Get entity from StockTransportOrderNote by key
*NoteForStockTransportOrderApi* | [**stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguagePatch**](docs/Api/NoteForStockTransportOrderApi.md#stocktransportordernotestocktransportordertextobjecttypelanguagepatch) | **PATCH** /StockTransportOrderNote/{StockTransportOrder}/{TextObjectType}/{Language} | Update entity in StockTransportOrderNote
*NoteForStockTransportOrderApi* | [**stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageStockTransportOrderGet**](docs/Api/NoteForStockTransportOrderApi.md#stocktransportordernotestocktransportordertextobjecttypelanguagestocktransportorderget) | **GET** /StockTransportOrderNote/{StockTransportOrder}/{TextObjectType}/{Language}/_StockTransportOrder | Get related _StockTransportOrder
*NoteForStockTransportOrderApi* | [**stockTransportOrderStockTransportOrderStockTransportOrderNoteGet**](docs/Api/NoteForStockTransportOrderApi.md#stocktransportorderstocktransportorderstocktransportordernoteget) | **GET** /StockTransportOrder/{StockTransportOrder}/_StockTransportOrderNote | Get entities from related _StockTransportOrderNote
*NoteForStockTransportOrderApi* | [**stockTransportOrderStockTransportOrderStockTransportOrderNotePost**](docs/Api/NoteForStockTransportOrderApi.md#stocktransportorderstocktransportorderstocktransportordernotepost) | **POST** /StockTransportOrder/{StockTransportOrder}/_StockTransportOrderNote | Add new entity to related _StockTransportOrderNote
*PartnerForStockTransportOrderApi* | [**stockTransportOrderPartnerGet**](docs/Api/PartnerForStockTransportOrderApi.md#stocktransportorderpartnerget) | **GET** /StockTransportOrderPartner | Get entities from StockTransportOrderPartner
*PartnerForStockTransportOrderApi* | [**stockTransportOrderPartnerStockTransportOrderPartnerFunctionDelete**](docs/Api/PartnerForStockTransportOrderApi.md#stocktransportorderpartnerstocktransportorderpartnerfunctiondelete) | **DELETE** /StockTransportOrderPartner/{StockTransportOrder}/{PartnerFunction} | Delete entity from StockTransportOrderPartner
*PartnerForStockTransportOrderApi* | [**stockTransportOrderPartnerStockTransportOrderPartnerFunctionGet**](docs/Api/PartnerForStockTransportOrderApi.md#stocktransportorderpartnerstocktransportorderpartnerfunctionget) | **GET** /StockTransportOrderPartner/{StockTransportOrder}/{PartnerFunction} | Get entity from StockTransportOrderPartner by key
*PartnerForStockTransportOrderApi* | [**stockTransportOrderPartnerStockTransportOrderPartnerFunctionPatch**](docs/Api/PartnerForStockTransportOrderApi.md#stocktransportorderpartnerstocktransportorderpartnerfunctionpatch) | **PATCH** /StockTransportOrderPartner/{StockTransportOrder}/{PartnerFunction} | Update entity in StockTransportOrderPartner
*PartnerForStockTransportOrderApi* | [**stockTransportOrderPartnerStockTransportOrderPartnerFunctionStockTransportOrderGet**](docs/Api/PartnerForStockTransportOrderApi.md#stocktransportorderpartnerstocktransportorderpartnerfunctionstocktransportorderget) | **GET** /StockTransportOrderPartner/{StockTransportOrder}/{PartnerFunction}/_StockTransportOrder | Get related _StockTransportOrder
*PartnerForStockTransportOrderApi* | [**stockTransportOrderStockTransportOrderStockTransportOrderPartnerGet**](docs/Api/PartnerForStockTransportOrderApi.md#stocktransportorderstocktransportorderstocktransportorderpartnerget) | **GET** /StockTransportOrder/{StockTransportOrder}/_StockTransportOrderPartner | Get entities from related _StockTransportOrderPartner
*PartnerForStockTransportOrderApi* | [**stockTransportOrderStockTransportOrderStockTransportOrderPartnerPost**](docs/Api/PartnerForStockTransportOrderApi.md#stocktransportorderstocktransportorderstocktransportorderpartnerpost) | **POST** /StockTransportOrder/{StockTransportOrder}/_StockTransportOrderPartner | Add new entity to related _StockTransportOrderPartner
*PricingElementForSTOItemApi* | [**sTOItemPricingElementGet**](docs/Api/PricingElementForSTOItemApi.md#stoitempricingelementget) | **GET** /STOItemPricingElement | Get entities from STOItemPricingElement
*PricingElementForSTOItemApi* | [**sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterDelete**](docs/Api/PricingElementForSTOItemApi.md#stoitempricingelementstocktransportorderstocktransportorderitempricingdocumentpricingdocumentitempricingproceduresteppricingprocedurecounterdelete) | **DELETE** /STOItemPricingElement/{StockTransportOrder}/{StockTransportOrderItem}/{PricingDocument}/{PricingDocumentItem}/{PricingProcedureStep}/{PricingProcedureCounter} | Delete entity from STOItemPricingElement
*PricingElementForSTOItemApi* | [**sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterGet**](docs/Api/PricingElementForSTOItemApi.md#stoitempricingelementstocktransportorderstocktransportorderitempricingdocumentpricingdocumentitempricingproceduresteppricingprocedurecounterget) | **GET** /STOItemPricingElement/{StockTransportOrder}/{StockTransportOrderItem}/{PricingDocument}/{PricingDocumentItem}/{PricingProcedureStep}/{PricingProcedureCounter} | Get entity from STOItemPricingElement by key
*PricingElementForSTOItemApi* | [**sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterPatch**](docs/Api/PricingElementForSTOItemApi.md#stoitempricingelementstocktransportorderstocktransportorderitempricingdocumentpricingdocumentitempricingproceduresteppricingprocedurecounterpatch) | **PATCH** /STOItemPricingElement/{StockTransportOrder}/{StockTransportOrderItem}/{PricingDocument}/{PricingDocumentItem}/{PricingProcedureStep}/{PricingProcedureCounter} | Update entity in STOItemPricingElement
*PricingElementForSTOItemApi* | [**sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterStockTransportOrderGet**](docs/Api/PricingElementForSTOItemApi.md#stoitempricingelementstocktransportorderstocktransportorderitempricingdocumentpricingdocumentitempricingproceduresteppricingprocedurecounterstocktransportorderget) | **GET** /STOItemPricingElement/{StockTransportOrder}/{StockTransportOrderItem}/{PricingDocument}/{PricingDocumentItem}/{PricingProcedureStep}/{PricingProcedureCounter}/_StockTransportOrder | Get related _StockTransportOrder
*PricingElementForSTOItemApi* | [**sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterStockTransportOrderItemGet**](docs/Api/PricingElementForSTOItemApi.md#stoitempricingelementstocktransportorderstocktransportorderitempricingdocumentpricingdocumentitempricingproceduresteppricingprocedurecounterstocktransportorderitemget) | **GET** /STOItemPricingElement/{StockTransportOrder}/{StockTransportOrderItem}/{PricingDocument}/{PricingDocumentItem}/{PricingProcedureStep}/{PricingProcedureCounter}/_StockTransportOrderItem | Get related _StockTransportOrderItem
*PricingElementForSTOItemApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemPricingElementGet**](docs/Api/PricingElementForSTOItemApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemstoitempricingelementget) | **GET** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOItemPricingElement | Get entities from related _STOItemPricingElement
*PricingElementForSTOItemApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOItemPricingElementPost**](docs/Api/PricingElementForSTOItemApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemstoitempricingelementpost) | **POST** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOItemPricingElement | Add new entity to related _STOItemPricingElement
*ScheduleLineForStockTransportOrderApi* | [**sTOScheduleLineGet**](docs/Api/ScheduleLineForStockTransportOrderApi.md#stoschedulelineget) | **GET** /STOScheduleLine | Get entities from STOScheduleLine
*ScheduleLineForStockTransportOrderApi* | [**sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineDelete**](docs/Api/ScheduleLineForStockTransportOrderApi.md#stoschedulelinestocktransportorderstocktransportorderitemschedulelinedelete) | **DELETE** /STOScheduleLine/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine} | Delete entity from STOScheduleLine
*ScheduleLineForStockTransportOrderApi* | [**sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineGet**](docs/Api/ScheduleLineForStockTransportOrderApi.md#stoschedulelinestocktransportorderstocktransportorderitemschedulelineget) | **GET** /STOScheduleLine/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine} | Get entity from STOScheduleLine by key
*ScheduleLineForStockTransportOrderApi* | [**sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLinePatch**](docs/Api/ScheduleLineForStockTransportOrderApi.md#stoschedulelinestocktransportorderstocktransportorderitemschedulelinepatch) | **PATCH** /STOScheduleLine/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine} | Update entity in STOScheduleLine
*ScheduleLineForStockTransportOrderApi* | [**sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentGet**](docs/Api/ScheduleLineForStockTransportOrderApi.md#stoschedulelinestocktransportorderstocktransportorderitemschedulelinestosubcontractingcomponentget) | **GET** /STOScheduleLine/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/_STOSubcontractingComponent | Get entities from related _STOSubcontractingComponent
*ScheduleLineForStockTransportOrderApi* | [**sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentPost**](docs/Api/ScheduleLineForStockTransportOrderApi.md#stoschedulelinestocktransportorderstocktransportorderitemschedulelinestosubcontractingcomponentpost) | **POST** /STOScheduleLine/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/_STOSubcontractingComponent | Add new entity to related _STOSubcontractingComponent
*ScheduleLineForStockTransportOrderApi* | [**sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineStockTransportOrderGet**](docs/Api/ScheduleLineForStockTransportOrderApi.md#stoschedulelinestocktransportorderstocktransportorderitemschedulelinestocktransportorderget) | **GET** /STOScheduleLine/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/_StockTransportOrder | Get related _StockTransportOrder
*ScheduleLineForStockTransportOrderApi* | [**sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineStockTransportOrderItemGet**](docs/Api/ScheduleLineForStockTransportOrderApi.md#stoschedulelinestocktransportorderstocktransportorderitemschedulelinestocktransportorderitemget) | **GET** /STOScheduleLine/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/_StockTransportOrderItem | Get related _StockTransportOrderItem
*ScheduleLineForStockTransportOrderApi* | [**sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeScheduleLineGet**](docs/Api/ScheduleLineForStockTransportOrderApi.md#stosubcontractingcomponentstocktransportorderstocktransportorderitemschedulelinereservationitemrecordtypeschedulelineget) | **GET** /STOSubcontractingComponent/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/{ReservationItem}/{RecordType}/_ScheduleLine | Get related _ScheduleLine
*ScheduleLineForStockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOScheduleLineGet**](docs/Api/ScheduleLineForStockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemstoschedulelineget) | **GET** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOScheduleLine | Get entities from related _STOScheduleLine
*ScheduleLineForStockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOScheduleLinePost**](docs/Api/ScheduleLineForStockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemstoschedulelinepost) | **POST** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOScheduleLine | Add new entity to related _STOScheduleLine
*ShippingDataForStockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemSTOShippingGet**](docs/Api/ShippingDataForStockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemstoshippingget) | **GET** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_STOShipping | Get related _STOShipping
*ShippingDataForStockTransportOrderApi* | [**stockTransportOrderShippingGet**](docs/Api/ShippingDataForStockTransportOrderApi.md#stocktransportordershippingget) | **GET** /StockTransportOrderShipping | Get entities from StockTransportOrderShipping
*ShippingDataForStockTransportOrderApi* | [**stockTransportOrderShippingStockTransportOrderStockTransportOrderItemGet**](docs/Api/ShippingDataForStockTransportOrderApi.md#stocktransportordershippingstocktransportorderstocktransportorderitemget) | **GET** /StockTransportOrderShipping/{StockTransportOrder}/{StockTransportOrderItem} | Get entity from StockTransportOrderShipping by key
*ShippingDataForStockTransportOrderApi* | [**stockTransportOrderShippingStockTransportOrderStockTransportOrderItemPatch**](docs/Api/ShippingDataForStockTransportOrderApi.md#stocktransportordershippingstocktransportorderstocktransportorderitempatch) | **PATCH** /StockTransportOrderShipping/{StockTransportOrder}/{StockTransportOrderItem} | Update entity in StockTransportOrderShipping
*ShippingDataForStockTransportOrderApi* | [**stockTransportOrderShippingStockTransportOrderStockTransportOrderItemStockTransportOrderGet**](docs/Api/ShippingDataForStockTransportOrderApi.md#stocktransportordershippingstocktransportorderstocktransportorderitemstocktransportorderget) | **GET** /StockTransportOrderShipping/{StockTransportOrder}/{StockTransportOrderItem}/_StockTransportOrder | Get related _StockTransportOrder
*ShippingDataForStockTransportOrderApi* | [**stockTransportOrderShippingStockTransportOrderStockTransportOrderItemStockTransportOrderItemGet**](docs/Api/ShippingDataForStockTransportOrderApi.md#stocktransportordershippingstocktransportorderstocktransportorderitemstocktransportorderitemget) | **GET** /StockTransportOrderShipping/{StockTransportOrder}/{StockTransportOrderItem}/_StockTransportOrderItem | Get related _StockTransportOrderItem
*StockTransportOrderApi* | [**sTOAccountAssignmentStockTransportOrderStockTransportOrderItemAccountAssignmentNumberStockTransportOrderGet**](docs/Api/StockTransportOrderApi.md#stoaccountassignmentstocktransportorderstocktransportorderitemaccountassignmentnumberstocktransportorderget) | **GET** /STOAccountAssignment/{StockTransportOrder}/{StockTransportOrderItem}/{AccountAssignmentNumber}/_StockTransportOrder | Get related _StockTransportOrder
*StockTransportOrderApi* | [**sTOItemPricingElementStockTransportOrderStockTransportOrderItemPricingDocumentPricingDocumentItemPricingProcedureStepPricingProcedureCounterStockTransportOrderGet**](docs/Api/StockTransportOrderApi.md#stoitempricingelementstocktransportorderstocktransportorderitempricingdocumentpricingdocumentitempricingproceduresteppricingprocedurecounterstocktransportorderget) | **GET** /STOItemPricingElement/{StockTransportOrder}/{StockTransportOrderItem}/{PricingDocument}/{PricingDocumentItem}/{PricingProcedureStep}/{PricingProcedureCounter}/_StockTransportOrder | Get related _StockTransportOrder
*StockTransportOrderApi* | [**sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineStockTransportOrderGet**](docs/Api/StockTransportOrderApi.md#stoschedulelinestocktransportorderstocktransportorderitemschedulelinestocktransportorderget) | **GET** /STOScheduleLine/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/_StockTransportOrder | Get related _StockTransportOrder
*StockTransportOrderApi* | [**sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeStockTransportOrderGet**](docs/Api/StockTransportOrderApi.md#stosubcontractingcomponentstocktransportorderstocktransportorderitemschedulelinereservationitemrecordtypestocktransportorderget) | **GET** /STOSubcontractingComponent/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/{ReservationItem}/{RecordType}/_StockTransportOrder | Get related _StockTransportOrder
*StockTransportOrderApi* | [**stockTransportOrderGet**](docs/Api/StockTransportOrderApi.md#stocktransportorderget) | **GET** /StockTransportOrder | Get entities from StockTransportOrder
*StockTransportOrderApi* | [**stockTransportOrderItemNoteStockTransportOrderStockTransportOrderItemTextObjectTypeLanguageStockTransportOrderGet**](docs/Api/StockTransportOrderApi.md#stocktransportorderitemnotestocktransportorderstocktransportorderitemtextobjecttypelanguagestocktransportorderget) | **GET** /StockTransportOrderItemNote/{StockTransportOrder}/{StockTransportOrderItem}/{TextObjectType}/{Language}/_StockTransportOrder | Get related _StockTransportOrder
*StockTransportOrderApi* | [**stockTransportOrderItemStockTransportOrderStockTransportOrderItemStockTransportOrderGet**](docs/Api/StockTransportOrderApi.md#stocktransportorderitemstocktransportorderstocktransportorderitemstocktransportorderget) | **GET** /StockTransportOrderItem/{StockTransportOrder}/{StockTransportOrderItem}/_StockTransportOrder | Get related _StockTransportOrder
*StockTransportOrderApi* | [**stockTransportOrderNoteStockTransportOrderTextObjectTypeLanguageStockTransportOrderGet**](docs/Api/StockTransportOrderApi.md#stocktransportordernotestocktransportordertextobjecttypelanguagestocktransportorderget) | **GET** /StockTransportOrderNote/{StockTransportOrder}/{TextObjectType}/{Language}/_StockTransportOrder | Get related _StockTransportOrder
*StockTransportOrderApi* | [**stockTransportOrderPartnerStockTransportOrderPartnerFunctionStockTransportOrderGet**](docs/Api/StockTransportOrderApi.md#stocktransportorderpartnerstocktransportorderpartnerfunctionstocktransportorderget) | **GET** /StockTransportOrderPartner/{StockTransportOrder}/{PartnerFunction}/_StockTransportOrder | Get related _StockTransportOrder
*StockTransportOrderApi* | [**stockTransportOrderPost**](docs/Api/StockTransportOrderApi.md#stocktransportorderpost) | **POST** /StockTransportOrder | Add new entity to StockTransportOrder
*StockTransportOrderApi* | [**stockTransportOrderShippingStockTransportOrderStockTransportOrderItemStockTransportOrderGet**](docs/Api/StockTransportOrderApi.md#stocktransportordershippingstocktransportorderstocktransportorderitemstocktransportorderget) | **GET** /StockTransportOrderShipping/{StockTransportOrder}/{StockTransportOrderItem}/_StockTransportOrder | Get related _StockTransportOrder
*StockTransportOrderApi* | [**stockTransportOrderStockTransportOrderGet**](docs/Api/StockTransportOrderApi.md#stocktransportorderstocktransportorderget) | **GET** /StockTransportOrder/{StockTransportOrder} | Get entity from StockTransportOrder by key
*StockTransportOrderApi* | [**stockTransportOrderStockTransportOrderPatch**](docs/Api/StockTransportOrderApi.md#stocktransportorderstocktransportorderpatch) | **PATCH** /StockTransportOrder/{StockTransportOrder} | Update entity in StockTransportOrder
*StockTransportOrderApi* | [**stockTransportOrderStockTransportOrderSAPSelfBlockAllItemsPost**](docs/Api/StockTransportOrderApi.md#stocktransportorderstocktransportordersapselfblockallitemspost) | **POST** /StockTransportOrder/{StockTransportOrder}/SAP__self.BlockAllItems | Invoke action BlockAllItems
*StockTransportOrderApi* | [**stockTransportOrderStockTransportOrderSAPSelfReadOrderingAddressGet**](docs/Api/StockTransportOrderApi.md#stocktransportorderstocktransportordersapselfreadorderingaddressget) | **GET** /StockTransportOrder/{StockTransportOrder}/SAP__self.ReadOrderingAddress() | Invoke function ReadOrderingAddress
*StockTransportOrderApi* | [**stockTransportOrderStockTransportOrderSAPSelfSetAllItemsToDeletedPost**](docs/Api/StockTransportOrderApi.md#stocktransportorderstocktransportordersapselfsetallitemstodeletedpost) | **POST** /StockTransportOrder/{StockTransportOrder}/SAP__self.SetAllItemsToDeleted | Invoke action SetAllItemsToDeleted
*StockTransportOrderApi* | [**stockTransportOrderStockTransportOrderStockTransportOrderItemGet**](docs/Api/StockTransportOrderApi.md#stocktransportorderstocktransportorderstocktransportorderitemget) | **GET** /StockTransportOrder/{StockTransportOrder}/_StockTransportOrderItem | Get entities from related _StockTransportOrderItem
*StockTransportOrderApi* | [**stockTransportOrderStockTransportOrderStockTransportOrderItemPost**](docs/Api/StockTransportOrderApi.md#stocktransportorderstocktransportorderstocktransportorderitempost) | **POST** /StockTransportOrder/{StockTransportOrder}/_StockTransportOrderItem | Add new entity to related _StockTransportOrderItem
*StockTransportOrderApi* | [**stockTransportOrderStockTransportOrderStockTransportOrderNoteGet**](docs/Api/StockTransportOrderApi.md#stocktransportorderstocktransportorderstocktransportordernoteget) | **GET** /StockTransportOrder/{StockTransportOrder}/_StockTransportOrderNote | Get entities from related _StockTransportOrderNote
*StockTransportOrderApi* | [**stockTransportOrderStockTransportOrderStockTransportOrderNotePost**](docs/Api/StockTransportOrderApi.md#stocktransportorderstocktransportorderstocktransportordernotepost) | **POST** /StockTransportOrder/{StockTransportOrder}/_StockTransportOrderNote | Add new entity to related _StockTransportOrderNote
*StockTransportOrderApi* | [**stockTransportOrderStockTransportOrderStockTransportOrderPartnerGet**](docs/Api/StockTransportOrderApi.md#stocktransportorderstocktransportorderstocktransportorderpartnerget) | **GET** /StockTransportOrder/{StockTransportOrder}/_StockTransportOrderPartner | Get entities from related _StockTransportOrderPartner
*StockTransportOrderApi* | [**stockTransportOrderStockTransportOrderStockTransportOrderPartnerPost**](docs/Api/StockTransportOrderApi.md#stocktransportorderstocktransportorderstocktransportorderpartnerpost) | **POST** /StockTransportOrder/{StockTransportOrder}/_StockTransportOrderPartner | Add new entity to related _StockTransportOrderPartner
*SubcontractingComponentForSTOApi* | [**sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentGet**](docs/Api/SubcontractingComponentForSTOApi.md#stoschedulelinestocktransportorderstocktransportorderitemschedulelinestosubcontractingcomponentget) | **GET** /STOScheduleLine/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/_STOSubcontractingComponent | Get entities from related _STOSubcontractingComponent
*SubcontractingComponentForSTOApi* | [**sTOScheduleLineStockTransportOrderStockTransportOrderItemScheduleLineSTOSubcontractingComponentPost**](docs/Api/SubcontractingComponentForSTOApi.md#stoschedulelinestocktransportorderstocktransportorderitemschedulelinestosubcontractingcomponentpost) | **POST** /STOScheduleLine/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/_STOSubcontractingComponent | Add new entity to related _STOSubcontractingComponent
*SubcontractingComponentForSTOApi* | [**sTOSubcontractingComponentGet**](docs/Api/SubcontractingComponentForSTOApi.md#stosubcontractingcomponentget) | **GET** /STOSubcontractingComponent | Get entities from STOSubcontractingComponent
*SubcontractingComponentForSTOApi* | [**sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeDelete**](docs/Api/SubcontractingComponentForSTOApi.md#stosubcontractingcomponentstocktransportorderstocktransportorderitemschedulelinereservationitemrecordtypedelete) | **DELETE** /STOSubcontractingComponent/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/{ReservationItem}/{RecordType} | Delete entity from STOSubcontractingComponent
*SubcontractingComponentForSTOApi* | [**sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeGet**](docs/Api/SubcontractingComponentForSTOApi.md#stosubcontractingcomponentstocktransportorderstocktransportorderitemschedulelinereservationitemrecordtypeget) | **GET** /STOSubcontractingComponent/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/{ReservationItem}/{RecordType} | Get entity from STOSubcontractingComponent by key
*SubcontractingComponentForSTOApi* | [**sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypePatch**](docs/Api/SubcontractingComponentForSTOApi.md#stosubcontractingcomponentstocktransportorderstocktransportorderitemschedulelinereservationitemrecordtypepatch) | **PATCH** /STOSubcontractingComponent/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/{ReservationItem}/{RecordType} | Update entity in STOSubcontractingComponent
*SubcontractingComponentForSTOApi* | [**sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeScheduleLineGet**](docs/Api/SubcontractingComponentForSTOApi.md#stosubcontractingcomponentstocktransportorderstocktransportorderitemschedulelinereservationitemrecordtypeschedulelineget) | **GET** /STOSubcontractingComponent/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/{ReservationItem}/{RecordType}/_ScheduleLine | Get related _ScheduleLine
*SubcontractingComponentForSTOApi* | [**sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeStockTransportOrderGet**](docs/Api/SubcontractingComponentForSTOApi.md#stosubcontractingcomponentstocktransportorderstocktransportorderitemschedulelinereservationitemrecordtypestocktransportorderget) | **GET** /STOSubcontractingComponent/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/{ReservationItem}/{RecordType}/_StockTransportOrder | Get related _StockTransportOrder
*SubcontractingComponentForSTOApi* | [**sTOSubcontractingComponentStockTransportOrderStockTransportOrderItemScheduleLineReservationItemRecordTypeStockTransportOrderItemGet**](docs/Api/SubcontractingComponentForSTOApi.md#stosubcontractingcomponentstocktransportorderstocktransportorderitemschedulelinereservationitemrecordtypestocktransportorderitemget) | **GET** /STOSubcontractingComponent/{StockTransportOrder}/{StockTransportOrderItem}/{ScheduleLine}/{ReservationItem}/{RecordType}/_StockTransportOrderItem | Get related _StockTransportOrderItem

## Models

- [AdjustedQty](docs/Model/AdjustedQty.md)
- [CndnBsAmt](docs/Model/CndnBsAmt.md)
- [CollectionOfSTOPricingElementType](docs/Model/CollectionOfSTOPricingElementType.md)
- [CollectionOfSTOSubcontractingComponentType](docs/Model/CollectionOfSTOSubcontractingComponentType.md)
- [CollectionOfStockTransportOrderAccountAssignmentType](docs/Model/CollectionOfStockTransportOrderAccountAssignmentType.md)
- [CollectionOfStockTransportOrderItemNoteType](docs/Model/CollectionOfStockTransportOrderItemNoteType.md)
- [CollectionOfStockTransportOrderItemType](docs/Model/CollectionOfStockTransportOrderItemType.md)
- [CollectionOfStockTransportOrderNoteType](docs/Model/CollectionOfStockTransportOrderNoteType.md)
- [CollectionOfStockTransportOrderPartnerType](docs/Model/CollectionOfStockTransportOrderPartnerType.md)
- [CollectionOfStockTransportOrderScheduleLineType](docs/Model/CollectionOfStockTransportOrderScheduleLineType.md)
- [CollectionOfStockTransportOrderShippingType](docs/Model/CollectionOfStockTransportOrderShippingType.md)
- [CollectionOfStockTransportOrderType](docs/Model/CollectionOfStockTransportOrderType.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001SAPMessage](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001SAPMessage.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001SAPMessageCreate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001SAPMessageCreate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001SAPMessageUpdate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001SAPMessageUpdate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementType](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementType.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementTypeCreate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementTypeCreate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementTypeUpdate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001STOPricingElementTypeUpdate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentType](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentType.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentTypeCreate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentTypeCreate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentTypeUpdate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentTypeUpdate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentType](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentType.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentTypeCreate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentTypeCreate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentTypeUpdate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderAccountAssignmentTypeUpdate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteType](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteType.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteTypeCreate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteTypeCreate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteTypeUpdate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemNoteTypeUpdate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemType](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemType.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemTypeCreate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemTypeCreate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemTypeUpdate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemTypeUpdate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteType](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteType.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteTypeCreate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteTypeCreate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteTypeUpdate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderNoteTypeUpdate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerType](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerType.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerTypeCreate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerTypeCreate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerTypeUpdate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderPartnerTypeUpdate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderReadDeliveryAddressResultType](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderReadDeliveryAddressResultType.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderReadDeliveryAddressResultTypeCreate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderReadDeliveryAddressResultTypeCreate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderReadDeliveryAddressResultTypeUpdate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderReadDeliveryAddressResultTypeUpdate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderReadOrderingAddressResultType](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderReadOrderingAddressResultType.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderReadOrderingAddressResultTypeCreate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderReadOrderingAddressResultTypeCreate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderReadOrderingAddressResultTypeUpdate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderReadOrderingAddressResultTypeUpdate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineType](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineType.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineTypeCreate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineTypeCreate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineTypeUpdate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineTypeUpdate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderShippingType](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderShippingType.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderShippingTypeCreate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderShippingTypeCreate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderShippingTypeUpdate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderShippingTypeUpdate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderTypeCreate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderTypeCreate.md)
- [ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderTypeUpdate](docs/Model/ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderTypeUpdate.md)
- [CommittedQuantity](docs/Model/CommittedQuantity.md)
- [ComponentScrap](docs/Model/ComponentScrap.md)
- [ConditionAmount](docs/Model/ConditionAmount.md)
- [ConditionFactor](docs/Model/ConditionFactor.md)
- [ConditionFactor1](docs/Model/ConditionFactor1.md)
- [ConditionRoundingDifference](docs/Model/ConditionRoundingDifference.md)
- [ConditionValue](docs/Model/ConditionValue.md)
- [Count](docs/Model/Count.md)
- [Denominator](docs/Model/Denominator.md)
- [Denominator1](docs/Model/Denominator1.md)
- [Distribution](docs/Model/Distribution.md)
- [EffectiveValue](docs/Model/EffectiveValue.md)
- [Error](docs/Model/Error.md)
- [ErrorError](docs/Model/ErrorError.md)
- [ErrorErrorDetailsInner](docs/Model/ErrorErrorDetailsInner.md)
- [ExchangeRate](docs/Model/ExchangeRate.md)
- [GRProcessingTime](docs/Model/GRProcessingTime.md)
- [GrossWeight](docs/Model/GrossWeight.md)
- [LeadTimeOffset](docs/Model/LeadTimeOffset.md)
- [NetOrderPrice](docs/Model/NetOrderPrice.md)
- [NetOrderValue](docs/Model/NetOrderValue.md)
- [NetWeight](docs/Model/NetWeight.md)
- [Numerator](docs/Model/Numerator.md)
- [Numerator1](docs/Model/Numerator1.md)
- [OperationScrapIn](docs/Model/OperationScrapIn.md)
- [OrderQuantity](docs/Model/OrderQuantity.md)
- [OverdelivTolerance](docs/Model/OverdelivTolerance.md)
- [PricingUnit](docs/Model/PricingUnit.md)
- [QtyDelivered](docs/Model/QtyDelivered.md)
- [Quantity](docs/Model/Quantity.md)
- [QuantityDelivered](docs/Model/QuantityDelivered.md)
- [QuantityInUnitOfEntry](docs/Model/QuantityInUnitOfEntry.md)
- [Ratio](docs/Model/Ratio.md)
- [RequirementQuantity](docs/Model/RequirementQuantity.md)
- [ScheduledQuantity](docs/Model/ScheduledQuantity.md)
- [Size1](docs/Model/Size1.md)
- [Size2](docs/Model/Size2.md)
- [Size3](docs/Model/Size3.md)
- [UnderdelTolerance](docs/Model/UnderdelTolerance.md)
- [VSIQuantity](docs/Model/VSIQuantity.md)
- [Volume](docs/Model/Volume.md)
- [WithdrawnQuantity](docs/Model/WithdrawnQuantity.md)

## Authorization

Authentication schemes defined for the API:
### basicAuthentication

- **Type**: HTTP basic authentication

## Tests

To run the tests, use:

```bash
composer install
vendor/bin/phpunit
```

## Author



## About this package

This PHP package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

- API version: `1.1.0`
- Build package: `org.openapitools.codegen.languages.PhpClientCodegen`
