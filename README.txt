Description
===========
Commerce Parsian Payment is a module that defines a new "Payment Method" for an Commerce powered
website to process its online payments through the [Parsian Bank](http://parsian-bank.com/) gateway.


Requirements
============
1. A valid PIN number provided by Parsian Bank.
2. A registered IP address on Parsian Bank databases.

You need to have a valid PIN number provided by Parsian Bank and also a registered IP Address on their gateway to be able to process you website payments via Parsian bank online payment gateway. If these requirements are not satisfied, expect to get a "22 Error Code".


Dependencies
============
- [commerce](http://drupal.org/project/commerce) and its commerce_payment.
- [SOAP Client](http://drupal.org/project/soapclient)
  - Note: nuSOAP library's `$soap_defencoding` value is not important for commerce_parsian, It works with both 'UTF-8' and 'ISO-8859-1'.

Installation
============
1. Install [commerce](http://drupal.org/project/ubercart) if not yet installed:
  - Enable "Payment" module under "commerce - core (optional)" and all its dependencies.

2. Install & enable [SOAP Client](http://drupal.org/project/soapclient).
  - Go to admin/settings/soapclient.
  - Under "Active SOAP Library" check the "nuSOAP" option.
  - Leave other options as default.

3. Install and enable [Commerce Parsian Payment](http://drupal.org/project/uc_parsian)
  - Go to admin/store/settings/payment/edit/methods.
  - Check "Parsian Bank" under "Payment methods" block.
  - Click on "Parsian Bank settings" and fill the "Parsian Authentication PIN" field with the PIN number provided by Parsian Bank.
  - Leave other fields as default and save the configuration.


Author and Maintainer
=====================
Farhang Darzi (http://drupal.org/user/668010)

