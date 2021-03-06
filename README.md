# Certegy Ezi-Pay Payment Gateway Module for Magento 2

The following instructions detail how to install the Certegy Ezi-Pay Payment gateway on the Magento 2 platform.

This assumes that you have signed the required Merchant Agreement and have been provided a Merchant Id and API Key.

## Install using Composer 

 
1. Add the Certegy Ezi-Pay Repository 

        composer config repositories.certegyezipay git https://github.com/Certegy/certegy-ezipay-magento-2.x.git

2. Require the Certegy Ezi-Pay Payment Gateway Module

        composer require certegy/module-ezipay-payment-gateway:dev-master

3. Enable the module 
       
       ./bin/magento module:enable Certegy_EzipayPaymentGateway --clear-static-content

4. Update the Database 

       ./bin/magento setup:upgrade

5.  Configure the plugin

Login to the  administration interface and go to:
  
 * Stores -> Configuration -> Sales -> Payment Methods 

 * Scroll Down to "Other Payment Methods" and select "Certegy Ezipay Payment Gateway" 

 * Enter your Merchant Number and API Key and select "Save Config" in the top right of the screen. 


## Getting help. 

If you would like assistance with the installation of the plugin or you need an API key, please contact the Certegy Ezi-Pay Platform Integration Team pit@certegy.com.au


