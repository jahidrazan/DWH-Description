# Schema Description


### 1.suppliers

This table lists down all the suppliers and their code name as tag

+ **supplier_id**: id of the suppliers

+ **tag**: nshort version of the name

+ **name**: name of the supplier

![suppliers](https://github.com/jahidrazan/DWH_pictures/blob/main/suppliers.PNG "VIEW of the suppliers table")


### 2.supplier_product_wish
 
This table contains the lead time quantities, safety stock and reorder_point for a product_id supplied by a supplier

+ **product_id**: id of product

+ **supplier_id**: id of a supplier

+ **lead_time_mean**: mean lead time of a supplier for delivering a specific product 

+ **lead_time_deviation**:  deviation of lead time for this product calculated by taking into account the lead time by all suppliers for this product

+ **lead_time_demand**: demand of a product during the lead time

+ **safety_stock**: calculated using following the formula:  Service factor * Standard deviaton * (Sq root) Lead time

+ **reorder_point**: This is the minimum amount of quantity we want to have for a specific product.
                     Reorder Point = Lead Time Demand + Safety Stock.
                     
 ![supplier_product_wish]https://github.com/jahidrazan/DWH_pictures/blob/main/supplier_product_wish.PNG "VIEW of the supplier_product_wish table")
