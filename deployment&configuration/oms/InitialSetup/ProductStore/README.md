# Configure Product Store

A Product Store in HotWax Commerce is like the a company, or a brand if a retailer has multipe brands.

Here are the settings that can be configured in a Product Store:

**Product Store Name** This is the name of the company. If the company has multiple brands this shoudl be the name of one brand.

**Currency:** Fetch it from the organization’s google form. Generally, it is USD.

**Weight:** Its value can be fetched from Shopify. Usually, it is WT_lb in USA else in other countries it is WT_Kg.

**Auto Approve Order:** By default, its value is N. Based on the business rules whether auto-approval of orders needs to be enabled or disabled its value can be set from the dropdown as Y or N.

**Auto Cancel Days:** The default value is 0. That indicates no auto cancel days should be applied. If needed, enter the the total number of days after which an order should be auto-canceled if it remains un-allocated.

**Sales Order and Purchase Order ID Prefix:** This should be checked with the retailer if they have a preference. Adding a prefix to the internal ID helps visually seperate purchase orders and sales orders. 

**Allow Split:** By default allow split is set to Y. If we need not allow the order split its value can be set from the dropdown as Y or N. Based on this the orders will be split and multiple shipments will be created.

**Product Identifier Enum ID:** This setting changes which Identification of a product to use as its primary internalName.

### Do not edit these fields

**Explode Order Items** This setting changes if multi-quantity order items are exploded into single quantity items. The default value for this setting is "Y" indicating that it is enabled, it should not be changed to "N", may flows of the OMS are not tested for this setting.

**External ID** Most retailers will never need this. Adding it will not break any flows but since it is not part of required data setup, it's recommended to leave it blank.


## Add a Company Name
This is the organization at the top of the retailers heirarchy. If a retailer has multiple brands, this would be the name of the organization that owns all of them.

To configure the company name, you'll have to navigate to Webtools.

```
{hostname}.hotwax.io/webtools
```

Under "Framework Web Tools", click "Entity Engine". Search for the "WebSite" entity.
```
WebSite
```

Open the website entity and click search to see a result of the all the companies configured in the system. By default there should only be one company which is part of the default setup.

Continue to the detail page of the defualt company by clicking 'View'.

In the Company Detail page, click "Edit" and change the name of the company in the field "siteName".


{% hint style="info" %}
    If a brand only has one Product Store, its a good idea to reuse its name here.
{% endhint %}