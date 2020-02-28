---
title: Third Party Listings
redirect_from:
  - /sales-channels/amazon/ob-third-party-listings.html
---

Third Party Listing settings are part of your store's listing settings. Listing settings are accessed from the [store's dashboard]({% link sales-channels/asc/amazon-store-dashboard.md %}).

The Third Party Listings section defines if your Magento catalog will import products from your existing Amazon Seller Central listings. We recommend importing listings from Amazon, to ensure all listings have matching Magento products. By having your listings as part of your Magento catalog, you can manage all of your products from a single catalog and leverage Amazon Sales Channel features including fulfillment and order management with Amazon, intelligent repricing, and quantity management.

When set to `Import listing`, Amazon Sales Channel imports your Amazon listings into your Magento catalog, attempting to match them to existing products. If a match is not automatically found, you can import the Amazon listing as a new Magento product or manually match the listing to a product.

If you choose to import listings, select the Magento attributes with values for Amazon Seller SKU and Amazon ASIN. If you do not have Magento [product attributes]({% link sales-channels/asc/ob-creating-magento-attributes.md %}), consider creating and assigning them. Mapping these attributes helps correctly match imported Amazon listings to your Magento products.

The initial listing import initiates when completing your store's setup during onboarding. After setup is complete and based on your cron settings, Magento continually checks for newly added Amazon listings (not created in Amazon Sales Channel) and updates your catalog according to these settings.

## Configure Third Party Listings settings

1. Expand the **Third Party Listings** section.

1. For **Import Third Party Listings** (required), select an option in the drop down:

    - **Import Listing**: Choose when you want products and information from your Amazon listings to import into your Magento catalog of products. This is the recommended and the default setting.

    - **Do Not Import Listing**: Choose when you want to manually [create and assign new products]({% link catalog/products.md %}) to your Magento catalog for your Amazon listings.

    {:.bs-callout .bs-callout-info}
    The following options fields are only active when you select `Import Listing`.

1. For **Attribute That Contains Amazon Seller SKU**, select the Magento attribute that matches to the Amazon Seller SKU value.

1. For **Attribute That Contains Amazon ASIN**, select the Magento attribute that you created and match it to the Amazon ASIN.

    {:.bs-callout .bs-callout-info}
    If you did not create these Magento attributes for your Amazon listings, see [Creating Attributes for Amazon Matching]({% link sales-channels/asc/ob-creating-magento-attributes.md %}) for information.

![]({% link sales-channels/asc/assets/amazon-third-party-listings.png %}){: .zoom}
_Third Party Listings_

|Field|Description|
|---|---|
|Import Third Party Listings|Required field. Options:<br/>**Import Listing**: (Default) Choose when you want products and information from your Amazon listings to import into your Magento catalog of products. <br/>**Do Not Import Listing**: Choose when you want to manually [create and assign new products]({% link catalog/products.md %}) to your Magento catalog for your Amazon listings.|
|Attribute That Contains Amazon Seller SKU|Only active when `Import Listing` is selected.<br />Select the Magento attribute to match to the Amazon attribute for the Amazon Seller SKU. This attribute should have been created during onboarding. See [Creating Amazon Product Attributes for Amazon Matching]({% link sales-channels/asc/ob-creating-magento-attributes.md %}). You may need to review your Magento [attributes]({% link sales-channels/asc/managing-attributes.md %}) and create or edit an attribute to match to this Amazon data.|
|Attribute That Contains Amazon ASIN|Only active when `Import Listing` is selected.<br />Select the Magento attribute that matches to the Amazon attribute for the Amazon ASIN. This attribute should have been created during onboarding. See [Creating Amazon Product Attributes for Amazon Matching]({% link sales-channels/asc/ob-creating-magento-attributes.md %}). You may need to review your Magento [attributes]({% link sales-channels/asc/managing-attributes.md %}) and create or edit an attribute to match to this Amazon data.|