# Schema Description



### 1.marketplaces

This table lists down all the marketpetplaces for the Fixami products

+ **marketplace_id**: id of marketplace

+ **name**: name of the marketplace


### 2.marketplace_feeds
 
This table contains details of a marketplace (i.e- country, name, language)

+ **marketplace_feed_id**: id of marketplace feed

+ **marketplace_id**: id of the marketplace

+ **locale**: combination of language and country 

+ **language**: lnaguage of the marketplace

+ **country**: country of the marketplace

+ **name**: name of the marketplace




### 3.marketplace_offers 

This table contains information regarding what products the customers can buy in a marketplace: lists the product id, price, tax and currency in the marketplace. 


+ **marketplace_feed_id**: id of manufacturer

+ **product_id**: id of a product

+ **offer_status**: Indicates whether a product is active or inactive in a marketplace for the customers to buy. 

+ **price_excl**: price of a product in a marketplace excluding VAT

+ **tax**: tax amount of a product in a marketplace

+ **currency**: currency of the marketplace




### 4.warehouses

This table contains the names of the warehouses 


+ **warehouse_id**: id of warehouse

+ **slug**: shortform/code of a warehouse name

+ **name**: Full Name of a warehouse
