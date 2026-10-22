# # ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderScheduleLineType

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**stock_transport_order** | **string** | Stock Transport Order | [optional]
**stock_transport_order_item** | **string** | Stock Transport Order Item | [optional]
**schedule_line** | **string** | Delivery Schedule Line Counter | [optional]
**deliv_date_category** | **string** | Category of delivery date | [optional]
**schedule_line_delivery_date** | **\DateTime** | Item Delivery Date | [optional]
**schedule_line_delivery_time** | **string** | Delivery Date Time-Spot | [optional]
**order_quantity_unit** | **string** | Purchase Order Unit of Measure | [optional]
**order_quantity_unit_iso_code** | **string** | ISO Code for Unit of Measurement | [optional]
**schedule_line_order_quantity** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ScheduledQuantity**](ScheduledQuantity.md) |  | [optional]
**rough_goods_receipt_qty** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\QuantityDelivered**](QuantityDelivered.md) |  | [optional]
**purchase_requisition** | **string** | Purchase Requisition Number | [optional]
**purchase_requisition_item** | **string** | Item Number of Purchase Requisition | [optional]
**schedule_line_is_fixed** | **bool** | Schedule Line is \&quot;Fixed\&quot; | [optional]
**schedule_line_committed_quantity** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\CommittedQuantity**](CommittedQuantity.md) |  | [optional]
**transportation_planning_date** | **\DateTime** | Transportation Planning Date | [optional]
**transportation_planning_time** | **string** | Transp. Planning Time (Local, Relating to a Shipping Point) | [optional]
**loading_date** | **\DateTime** |  | [optional]
**loading_time** | **string** | Loading Time (Local Time Relating to a Shipping Point) | [optional]
**goods_issue_date** | **\DateTime** |  | [optional]
**goods_issue_time** | **string** | Time of Goods Issue (Local, Relating to a Plant) | [optional]
**sto_latest_possible_gr_date** | **\DateTime** | Goods Receipt End Date | [optional]
**sto_latest_possible_gr_time** | **string** | Goods Receipt End Time (Local, Relating to a Plant) | [optional]
**stock_transfer_delivered_quantity** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\QtyDelivered**](QtyDelivered.md) |  | [optional]
**stock_transport_order_type** | **string** | Purchasing Document Type | [optional]
**purchasing_organization** | **string** | Purchasing Organization | [optional]
**purchasing_group** | **string** |  | [optional]
**plant** | **string** |  | [optional]
**sap__messages** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001SAPMessage[]**](ComSapGatewaySrvdA2xApiStocktransportorderV0001SAPMessage.md) |  | [optional]
**_stock_transport_order** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType**](ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderType.md) |  | [optional]
**_stock_transport_order_item** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemType**](ComSapGatewaySrvdA2xApiStocktransportorderV0001StockTransportOrderItemType.md) |  | [optional]
**_sto_subcontracting_component** | [**\BeLenka\SAP\StockTransportOrderODV4\Model\ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentType[]**](ComSapGatewaySrvdA2xApiStocktransportorderV0001STOSubcontractingComponentType.md) |  | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
