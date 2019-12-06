# Open Data Product Specifications version v3.1.4

## Branch Locator

This specification includes all relevant artefacts for the Open Data Branch API Specification.
This endpoint can contain multiple brands owned by a particular banking group. Each brand can own multiple branches. 
A branch is made up of:-
* Identification - unique identification for the branch
* SequenceNumber - 0 indicates that this is a main branch, 1..n indicates that it's either a sub or mobile branch.
* Name - the branch name
* Type - Physical or Mobile
* CustomerSegment - The segment of customers that the branch serves e.g. Private, Retail, Business
* Photo - you can supply a URL showing an image of the branch e.g. use Google streetview
* Sort-Code(s) associated with branch
* Service/Facility (see subsection below)
* Accessibility (see subsection below)
* Postal Address (see subsection below)


## ATM Locator

This specification includes all relevant artefacts for the Open Data ATM API Specification.

This endpoint can contain multiple brands owned by a particular banking group. Each brand can provide multiple ATMs.

An ATM consists of:-

* A unique Identification
* ATMServices - a pre-defined set of standard code names defining services available from an ATM e.g. PinUnblock.
  
* OtherATMServices - allows a bank to add it's own non-standard/proprietary codes, code names and descriptions.
  
* Accessibility - a pre-defined set of standard code names defining accessibility features that the ATM offers e.g. InductionLoop
  
* OtherAccessibility - allows a bank to add it's own non-standard/proprietary codes, code names and descriptions.
  
* Supported Languages - the 2-digit ISO 639-1 language code.
  
* Location - This is where the ATM is located and is a mix of a postal address and the geographic coordinates (decimal Latitude and Longitude). Postal address information can either be:-
   
   i) Up to 7 lines of unstructured address information (AddressLine ) 
   
   ii) Structured address information e.g. BuildingNumber, StreetName, Town, PostCode etc or a mixture of both. 
   
   Location is very important so the API provider should ensure that either geographical coordinates (preferred) or a combination of building number and postcode are supplied so that the ATM can be accurately located on a map.
  
* Base currency - currently restricted to 'GBP' only, but may be extended in future to cope with other currencies dispensed by ATMs at airports, for example, if the API providers are able to supply this information.
  
* Minimum possible amount - This will inform a consumer as the minimum possible amount that they can withdraw from an ATM. Note: This is not the same as the minimum denomination. For example, an ATM may dispense £5 notes but require the consumer to withdraw a minimum possible amount of £10.


## Business Current Account 

This specification includes all relevant artifacts for the Open Data Business Current Account (BCA) API Specification.
Currently, price comparison websites have to obtain their BCA product data either via bank proprietary APIs, via information collected by dedicated data capture agencies or via "screen scraping" (i.e. capturing product web page information and writing scripts to extract relevant data). This work is complex and prone to error, so having a standard API would make the data capture side much easier and allow more third-party providers to provide applications that could target particular consumer markets.
This endpoint can contain multiple brands owned by a particular banking group. Each brand can own multiple BCA products.

## Personal Current Account

This specification includes all relevant artefacts for the Open Data Personal Current Account (PCA) API Specification.

Currently, price comparison websites have to obtain their PCA product data either via bank proprietary APIs, via information collected by dedicated data capture agencies or via "screen scraping" (i.e. capturing product web page information and writing scripts to extract relevant data). This work is complex and prone to error, so having a standard API would make the data capture side much easier and allow more third party providers to provide applications that could target particular consumer markets.

This endpoint can contain multiple brands owned by a particular banking group. Each brand can own multiple PCA products.


## SME Loan

This specification includes all relevant artefacts for the Open Data Business SME Unsecured Loans (SME) API Specification.

Currently, price comparison websites have to obtain their SME Business Loan product data either via bank proprietary APIs, via information collected by dedicated data capture agencies or via "screen scraping" (i.e. capturing product web page information and writing scripts to extract relevant data). This work is complex and prone to error, so having a standard API would make the data capture side much easier and allow more third party providers to provide applications that could target particular consumer markets.

This endpoint can contain multiple brands owned by a particular banking group. Each brand can own multiple SME Unsecured Loan products.


## SME Commercial Credit Card

This specification includes all relevant artefacts for the Open Data Business SME Commercial Credit Cards (CCC) API Specification.
Currently, price comparison websites have to obtain their CCC product data either via bank proprietary APIs, via information collected by dedicated data capture agencies or via "screen scraping" (i.e. capturing product web page information and writing scripts to extract relevant data). This work is complex and prone to error, so having a standard API would make the data capture side much easier and allow more third party providers to provide applications that could target particular SME markets.
This endpoint can contain multiple brands owned by a particular banking group. Each brand can own multiple SME Commercial Credit Card products.



