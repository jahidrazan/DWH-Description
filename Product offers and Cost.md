# Schema Description



### 1.api.product_offers

This table lists the product_id and the price information at which the product is sold at diffrent countries


+ **product_id**: distinct product_id for all the products

+ **country**: country where the product is sold

+ **price_excl**: price excluding VAT for the product in a specific country

+ **tax**: tax paid by fixami for selling a specific proudct in a country

+ **currency**: currency of transaction 

![product_offers](https://github.com/jahidrazan/DWH_pictures/blob/main/api.product_offers.PNG "VIEW of the product_offers table")

### 2.api.product_offer_logs

This table lists the price update of a product in a specific country 


+ **product_id**: distinct product_id for all the products

+ **country**: country where the product is sold

+ **updated_at**: the price update information 

+ **price_excl**: updated price excluding VAT for the product in a specific country

+ **tax**: tax paid by fixami for selling a specific proudct in a country

+ **currency**: currency of transaction 
        

![product_offer_logs](https://github.com/jahidrazan/DWH_pictures/blob/main/api.product_offer_logs.PNG "VIEW of the product_offer_logs table")

### 3.api.product_cost_logs

This table lists the cost update of a product that was paid by fiaxmi to buy it


+ **product_id**: distinct product_id for all the products

+ **updated_at**: the price paid by  update information 

+ **price**: price paid by fixami for the product

+ **currency**: currency of transaction 

![product_cost_logs](https://github.com/jahidrazan/DWH_pictures/blob/main/api.product_cost_logs.PNG "VIEW of the product_cost_logs table")

### 4.api.product_set_items

This table lists all the items sold as part of bundle


+ **parent_product_id**: parent id of a product bundle 

+ **child_product_id**: child id of a product

+ **quantity**: describes the composition of the bundle, how many child products are present within the bundle

![product_set_items](https://github.com/jahidrazan/DWH_pictures/blob/main/api.product_set_items.PNG "VIEW of the product_set_items table")       

### 5.api_history.product_offers

This table lists the history of the product pricing records at diffrent countries


+ **date**: day when the product is offered at a specific coutnry at a specific price

+ **product_id**: distinct product_id for all the products

+ **country**: country where the product is sold

+ **price_excl**: price excluding VAT for the product in a specific country

+ **tax**: tax paid by fixami for selling a specific proudct in a country

+ **currency**: currency of transaction 

![api_history.product_offers](https://github.com/jahidrazan/DWH_pictures/blob/main/api_history.product_offers.PNG "VIEW of the api_history.product_offers table")
