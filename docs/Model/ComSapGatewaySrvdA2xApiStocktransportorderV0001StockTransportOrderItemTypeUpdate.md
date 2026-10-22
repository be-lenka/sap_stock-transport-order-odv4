# # ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemTypeUpdate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**stock_transport_order_item_text** | **string** |  | [optional]
**document_currency** | **string** | Currency Key | [optional]
**product_group** | **string** |  | [optional]
**product** | **string** |  | [optional]
**product_type_code** | **string** |  | [optional]
**manufacturer_material** | **string** | Material number | [optional]
**plant** | **string** |  | [optional]
**storage_location** | **string** |  | [optional]
**order_quantity_unit** | **string** | Purchase Order Unit of Measure | [optional]
**is_completely_delivered** | **bool** | \&quot;Delivery Completed\&quot; Indicator | [optional]
**goods_receipt_is_expected** | **bool** | Goods Receipt Indicator | [optional]
**outward_delivery_is_complete** | **bool** | \&quot;Outward Delivery Completed\&quot; Indicator | [optional]
**invoice_is_expected** | **bool** | Invoice Receipt Indicator | [optional]
**unlimited_overdelivery_is_allowed** | **bool** | Unlimited Overdelivery Allowed | [optional]
**overdeliv_tolrtd_lmt_ratio_in_pct** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\OverdelivTolerance**](OverdelivTolerance.md) |  | [optional]
**underdeliv_tolrtd_lmt_ratio_in_pct** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\UnderdelTolerance**](UnderdelTolerance.md) |  | [optional]
**requisitioner_name** | **string** | Name of requisitioner/requester | [optional]
**sto_item_category** | **string** | Item category in purchasing document | [optional]
**delivery_document_type** | **string** | Delivery Type for Returns to Supplier | [optional]
**issuing_storage_location** | **string** | Issuing Storage Location for Stock Transport Order | [optional]
**purchasing_parent_item** | **string** | Higher-Level Item in Purchasing Documents | [optional]
**account_assignment_category** | **string** | Account Assignment Category | [optional]
**order_quantity_unit_iso_code** | **string** | ISO Code for Unit of Measurement | [optional]
**order_quantity** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\OrderQuantity**](OrderQuantity.md) |  | [optional]
**net_price_amount** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\NetOrderPrice**](NetOrderPrice.md) |  | [optional]
**multiple_acct_assgmt_distribution** | **string** | Distribution Indicator for Multiple Account Assignment | [optional]
**partial_invoice_distribution** | **string** | Partial invoice indicator | [optional]
**partial_delivery_is_allowed** | **string** | Partial Delivery at Item Level (Stock Transfer) | [optional]
**goods_receipt_duration_in_days** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\GRProcessingTime**](GRProcessingTime.md) |  | [optional]
**inventory_usability_code** | **string** |  | [optional]
**supplier_confirmation_control_key** | **string** | Confirmation Control Key | [optional]
**subcontractor** | **string** | Supplier to be Supplied/Who is to Receive Delivery | [optional]
**customer** | **string** |  | [optional]
**batch** | **string** | Batch Number | [optional]
**valuation_type** | **string** |  | [optional]
**sap__messages** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001SAPMessageUpdate[]**](ComSapGatewaySrvdA2xApiStocktransportorderV0001SAPMessageUpdate.md) |  | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
