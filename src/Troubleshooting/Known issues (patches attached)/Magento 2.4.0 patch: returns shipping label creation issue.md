---
title: Magento 2.4.0 patch: returns shipping label creation issue
link: https://support.magento.com/hc/en-us/articles/360046441312-Magento-2-4-0-patch-returns-shipping-label-creation-issue
labels: Magento Commerce Cloud,Magento Commerce,patch,known issues,2.4.0,shipping label,return
---

This article provides a patch for the Magento 2.4.0 known issue when there is a problem with printing a shipping label for customers’ returns.

## Affected products and versions

* Magento Commerce Cloud 2.4.0
* Magento Commerce 2.4.0

## Issue

Steps to reproduce:

1. Place and complete an order with one of the following core shipping methods FedEx, DHL, UPS, or USPS.
1. Create and authorize returns for this order.
1. Open an authorized Return Information page and click the Create Shipping Label button._  
    _
1. Select shipping method, add a product to a package and click Save. 

Expected result:

A shipping label is created successfully and you see a message: _You created a shipping label._  
  
Actual result:

The Return Information page is broken and you see an error message on the Return Information page: _General Information Changes have been made to this section that have not been saved. This tab contains invalid data_. 

## Solution

Apply [patch](https://support.magento.com/hc/en-us/article_attachments/360063124151/MC-35984-2.4.0-CE-composer.patch) provided in this article.

## Patch

The patch is attached to this article. To download it, scroll down to the end of the article and click the file name, or click the following link:

[MC-35984-2.4.0-CE-composer.patch](https://support.magento.com/hc/en-us/article_attachments/360063124151/MC-35984-2.4.0-CE-composer.patch)

The patch is also available for download in both, `` .git `` and `` .composer ``, formats on [Magento Commerce Downloads](https://magento.com/tech-resources/download) page, under Patches in the left column navigation. Search for MC-35984 patch. 

## How to apply the patch

See [How to apply a composer patch provided by Magento](https://support.magento.com/hc/en-us/articles/360028367731) for instructions.

## Related reading

* [Magento 2.4.0 known issue: raw message data display on storefront](https://support.magento.com/hc/en-us/articles/360045804332)
* [Magento 2.4.0 known issue: Export Tax Rates does not work](https://support.magento.com/hc/en-us/articles/360045850032)
* [Magento 2.4.0 known issue: “Add selections to my cart” button does not work](https://support.magento.com/hc/en-us/articles/360045838312)
* [Magento 2.4.0 known issue: Braintree payment methods do not show up in Multiple Addresses checkout](https://support.magento.com/hc/en-us/articles/360046354992)
* [Magento 2.4.0 B2B Admin can't add configurable product to quote](https://support.magento.com/hc/en-us/articles/360046801971-Magento-2-4-0-known-issue-B2B-Admin-cannot-add-a-configurable-product-to-a-quote)
* [Magento 2.4.0 known issue: orders display error](https://support.magento.com/hc/en-us/articles/360046802271-Magento-2-4-0-known-issue-orders-display-error)
* [Shipping labels creation known issue in Magento 2.4.0](https://support.magento.com/hc/en-us/articles/360046750171-Shipping-labels-creation-known-issue-in-Magento-2-4-0)