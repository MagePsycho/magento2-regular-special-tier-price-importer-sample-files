
## Overview
[Magento 2 Regular, Special & Tier Price Importer](https://www.magepsycho.com/extensions/magento-2/magento2-mass-regular-special-tier-group-price-importer.html) is the fastest import tool for bulk updating different prices like regular, cost, MSRP/MAP, special, tier & customer group price.  
  
![Magento 2 Regular, Special & Tier Price Importer Extension Backend Demo](http://g.recordit.co/9t1Dt1srQD.gif)  
  
Magento 2 has built-in data transfer for importing products and advanced pricing. But it lacks the functionality of updating all types of prices whether it's regular or advanced pricing in a single go.  
Also, the native import has very limited options for pricing.  
  
With this extension, store admin can achieve the simplest & fastest way to import all types of pricing with just a single CSV file *(more import sources will be added soon)*.  
And with the export pricing option, store admin can easily prepare the import file.  
  
## Key Features
* Provides bulk update for all types of price with just a single CSV file - *more import sources will be added soon*  
* Option to preview the uploaded file which gives the glance view of the file data  
* The detailed error message provided during import validation helps to fix the price data faster  
* Support for different types of price rounding (whole number to the psychological pricing)  
* Price values can be increased(`+`), decreased(`-`) by a fixed amount value or percentage  
* Price values can also be set as a certain percentage(`%`) of some reference attribute value  
* Option to export the different prices which makes import file preparation much easier  
  
## Sample Files  
These samples files are collected here so as to quickly demonstrate the functionality of [Magento 2 Regular, Special & Tier Price Importer](https://www.magepsycho.com/extensions/magento-2/magento2-mass-regular-special-tier-group-price-importer.html) Extension.  
  
The samples files can be either downloaded from the extension settings(see below screenshots) or from Github repository(files under `/samples` folder).  
![Magento 2 Regular, Special & Tier Price Importer Extension Sample Files](https://raw.githubusercontent.com/MagePsycho/magento2-regular-special-tier-price-importer-sample-files/master/docs/download-sample-file.png)  
  
### Validation  
All pricing data must pass validation before it can be imported into the system, to ensure that the values are consistent with the system database.    
If validation fails, the extension describes each error. This helps the store owner to quickly find and correct the problem in the CSV file.    
  
This sample file demonstrates the possible validation performed by the extension.  
[Download Validation Sample File](https://github.com/MagePsycho/magento2-regular-special-tier-price-importer-sample-files/blob/master/samples/1.validation_sample.csv)  
  
### Import Regular Price & Cost  
This sample file shows how to update `price` & `cost`
 ![Magento 2 Regular, Special & Tier Price Importer Extension Sample Files](http://g.recordit.co/ALTkYjrFQu.gif)
 
 [Download Regular Price Sample File](https://github.com/MagePsycho/magento2-regular-special-tier-price-importer-sample-files/blob/master/samples/3.regular_price_sample.csv)  
  

### Import Special Price with From & To Dates  
This sample file shows how to update `special_price`, `special_from_date` & `special_to_date`

 ![Magento 2 Regular, Special & Tier Price Importer Extension Sample Files](http://g.recordit.co/QeJFtXKMA2.gif)
 
  [Download Special Price Sample File](https://github.com/MagePsycho/magento2-regular-special-tier-price-importer-sample-files/blob/master/samples/4.special_price_sample.csv)   
  
### Import Tier Price/Customer Group Price  
 This sample file shows how to update `tier_price:*`
 
 ![Magento 2 Regular, Special & Tier Price Importer Extension Sample Files](http://g.recordit.co/UvCGAMUson.gif)
 
  [Download Tier Price Sample File](https://github.com/MagePsycho/magento2-regular-special-tier-price-importer-sample-files/blob/master/samples/5.tier_price_sample.csv)   

*'Group Price' in Magento 2 is the special case of Tier Price (with tier qty equals to 1).*

### Import All Prices (Regular, Cost, MSRP/MAP, Tier/Customer Group Price)  at Once
This sample file shows how to update all possible prices in Magento 2 at once with just a single CSV file.
![Magento 2 Regular, Special & Tier Price Importer Extension Sample Files](http://g.recordit.co/biMoNGTqVb.gif)

<p style="text-align: center;">
  <a href="https://github.com/MagePsycho/magento2-regular-special-tier-price-importer-sample-files/blob/master/samples/2.all_prices_sample.csv" title="Download All Prices Sample File">Download All Prices Sample File</a> 
</p>  

  *`sku`, `website_id` are two compulsory field for importing any types of pricing in Magento 2.*
 ## Price Value Format 
This extension supports different formats for pricing.


| Format | Description | Applied To |
| ------- | -------------- | ------------ |
| +10   | Increase the current value by 10  | All Prices |
| -10   | Decrease the current value by 10  | All Prices |
| 10%   | 10% of the reference price value (except `tier_price` where X% represents the discount) | `msrp`, `special_price`, `tier_price` |
| +10%  | Increase the current value by 10%  | All Prices |
| -10%  | Decrease the current value by 10%  | All Prices |
| x | Delete the value from the system  | All Prices (except `price`) |
