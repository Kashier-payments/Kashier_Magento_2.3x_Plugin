# Kashier_Magento_2.3x_Plugin

Accept online payments on Magent 2.3x (Egyptian Merchants)

![](https://raw.githubusercontent.com/Kashier-payments/Kashier_Magento_2.3x_Plugin/main/steps/kashier-logo.png)
![](https://raw.githubusercontent.com/Kashier-payments/Kashier_Magento_2.3x_Plugin/main/steps/mag_2.png)

## Features

- Fully PCI DSS compliant as a Level 1 Service for merchant operating in Egypt.
- I-frame integration.
- 3D secure cards authentication support.
- Support multiple payment method.
     
      1. Card Payments
      2. Wallet Payments  
      3. Bank Installments Payment 

## Installation  

1. Download a ZIP of the [repository](https://raw.githubusercontent.com/Kashier-payments/Kashier_Magento_2.3x_Plugin/main/Kashier_magento2.3.x.zip).
2. Create a new folder `app/code`.
3. Unzip the downloaded folder in `app/code`, the correct path should be "your/website-magento2-files/app/code/Kashier.
4. Run the command below from Magento Webstore folder:
         
         - php bin/magento module:enable Kashier_Payments
         - php bin/magento setup:upgrade
         - php bin/magento setup:static-content:deploy

5. After installation, proceed for configuration.

## Configuration

1. Log into your Magento Webstore Admin.
2. Navigate to the Admin Panel then to Store->Configuration->Sales->Payment Method.

![](https://raw.githubusercontent.com/Kashier-payments/Kashier_Magento_2.3x_Plugin/main/steps/configuration.png)

3. choose payment methods which you would like to use to accept payment via kashier.
      
      - Kashier (Visa / Mastercard / Mezza)
      - Kashier Wallets
      - Kashier Bank Installments
      - 
4. Save the configuration below in Kashier Gateway Extension.

   - Insert the MID and Test Api Key in the Configuration page of each payment method.
   - Make sure the enable checkbox is checked.
   - Make sure the test mode is on.
   - Customize the title that will show up tp your users.
   - Save configuration.

![](https://raw.githubusercontent.com/Kashier-payments/Kashier_Magento_2.3x_Plugin/main/steps/configuration_test.png)

5. In System, select Cache Management, then click on Flush Magento Cache.
6. Your Paytm Payment Gateway is enabled. Now you can accept payment through Paytm.

`Note: If you have Linux server, please make sure the folder permissions are set to 755 & file permissions to 644.`

## Obtain Test Credentials

- Login or Sign up on kashier.io https://merchant.kashier.io/
- Navigate to Integrate now section > payment api keys.
- Generate a new api key with your prefered name that describes your integration channel, there is 1 default api key you could use that is created when signing up.
- Copy Merchant ID visible under your user name "MID-xx-xx".

![](https://raw.githubusercontent.com/Kashier-payments/Kashier_Magento_2.3x_Plugin/main/steps/apikeylive.png)

## Go live

1. After activating your account.
2. Make sure you are on live mode.
3. Navigate to Integrate now section > payment api keys.
4. Generate a new api key with your prefered name that describes your integration channel, there is 1 default api key you could use that is created when signing up.

![](https://raw.githubusercontent.com/Kashier-payments/Kashier_Magento_2.3x_Plugin/main/steps/apikeytest.png)

5. Save the configuration below in Kashier Gateway Extension.
     
     - Insert Live Api Key in the Configuration page of each module.
     - Remove the test mode check.
     - Customize the title and description that will show up tp your users.
     - Save configuration.
     
6. In System, select Cache Management, then click on Flush Magento Cache.
7. Your Paytm Payment Gateway is enabled. Now you can accept payment through Paytm.

![](https://raw.githubusercontent.com/Kashier-payments/Kashier_Magento_2.3x_Plugin/main/steps/configuration_live.png)


### Support

- Leave us an inquiry ticket on https://kashier.io for questions.
