# OpenAPIClient-php

In every API call, you can make use of the following operations:
 - You can read entire sales orders without charge or only parts of the data, using the provided filters.
 - You can create sales orders without charge. Note that you must use “deep insert” requests (a header plus the following entities: header partner, item and item partner). You cannot create entities without including any related entities.
 - For existing sales orders without charge, you can create new items. Note that you must use “deep insert” requests (with the entity: item partner). You cannot create entities without including any related entities.
 - For existing sales orders without charge, you can update the header, header partner, item and item partner.
 - For existing sales orders without charge, you can delete the header, header partner, item and item partner.


## Installation & Usage

### Requirements

PHP 7.4 and later.
Should also work with PHP 8.0.

### Composer

To install the bindings via [Composer](https://getcomposer.org/), add the following to `composer.json`:

```json
{
  "repositories": [
    {
      "type": "vcs",
      "url": "https://github.com/GIT_USER_ID/GIT_REPO_ID.git"
    }
  ],
  "require": {
    "GIT_USER_ID/GIT_REPO_ID": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
<?php
require_once('/path/to/OpenAPIClient-php/vendor/autoload.php');
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



// Configure HTTP basic authorization: BasicAuth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');

// Configure OAuth2 access token for authorization: OAuth2Auth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\BatchRequestsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->batchPost();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BatchRequestsApi->batchPost: ', $e->getMessage(), PHP_EOL;
}

```

## API Endpoints

All URIs are relative to *https://:/sap/opu/odata/sap/API_SALES_ORDER_WITHOUT_CHARGE_SRV*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*BatchRequestsApi* | [**batchPost**](docs/Api/BatchRequestsApi.md#batchpost) | **POST** /$batch | Send a group of requests
*HeaderPartnerApi* | [**aSalesOrderWithoutChargeSalesOrderWithoutChargeToPartnerGet**](docs/Api/HeaderPartnerApi.md#asalesorderwithoutchargesalesorderwithoutchargetopartnerget) | **GET** /A_SalesOrderWithoutCharge(&#39;{SalesOrderWithoutCharge}&#39;)/to_Partner | Reads the header partners of a specific sales order without charge.
*HeaderPartnerApi* | [**aSlsOrdWthoutChrgPartnerGet**](docs/Api/HeaderPartnerApi.md#aslsordwthoutchrgpartnerget) | **GET** /A_SlsOrdWthoutChrgPartner | Reads the header partners of all sales order without charges.
*HeaderPartnerApi* | [**aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionDelete**](docs/Api/HeaderPartnerApi.md#aslsordwthoutchrgpartnersalesorderwithoutchargesalesorderwithoutchargepartnerfunctionpartnerfunctiondelete) | **DELETE** /A_SlsOrdWthoutChrgPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;) | Deletes the header partners of a specific sales order without charge and with a specific partner function.
*HeaderPartnerApi* | [**aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionGet**](docs/Api/HeaderPartnerApi.md#aslsordwthoutchrgpartnersalesorderwithoutchargesalesorderwithoutchargepartnerfunctionpartnerfunctionget) | **GET** /A_SlsOrdWthoutChrgPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;) | Reads the header partners of a specific sales order without charge and with a specific partner function.
*HeaderPartnerApi* | [**aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionPatch**](docs/Api/HeaderPartnerApi.md#aslsordwthoutchrgpartnersalesorderwithoutchargesalesorderwithoutchargepartnerfunctionpartnerfunctionpatch) | **PATCH** /A_SlsOrdWthoutChrgPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;) | Updates the header partners of a specific sales order without charge and with a specific partner function.
*HeaderPartnerApi* | [**aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionToSalesOrderWithoutChargeGet**](docs/Api/HeaderPartnerApi.md#aslsordwthoutchrgpartnersalesorderwithoutchargesalesorderwithoutchargepartnerfunctionpartnerfunctiontosalesorderwithoutchargeget) | **GET** /A_SlsOrdWthoutChrgPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific header partner.
*HeaderTextApi* | [**aSalesOrderWithoutChargeSalesOrderWithoutChargeToTextGet**](docs/Api/HeaderTextApi.md#asalesorderwithoutchargesalesorderwithoutchargetotextget) | **GET** /A_SalesOrderWithoutCharge(&#39;{SalesOrderWithoutCharge}&#39;)/to_Text | Reads the header texts of a specific sales order without charge.
*HeaderTextApi* | [**aSlsOrdWthoutChrgTextGet**](docs/Api/HeaderTextApi.md#aslsordwthoutchrgtextget) | **GET** /A_SlsOrdWthoutChrgText | Reads the header texts of all sales order without charges.
*HeaderTextApi* | [**aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDDelete**](docs/Api/HeaderTextApi.md#aslsordwthoutchrgtextsalesorderwithoutchargesalesorderwithoutchargelanguagelanguagelongtextidlongtextiddelete) | **DELETE** /A_SlsOrdWthoutChrgText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;) | Deletes a specific header text for a specific sales order without charge.
*HeaderTextApi* | [**aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDGet**](docs/Api/HeaderTextApi.md#aslsordwthoutchrgtextsalesorderwithoutchargesalesorderwithoutchargelanguagelanguagelongtextidlongtextidget) | **GET** /A_SlsOrdWthoutChrgText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;) | Reads a specific header text for a specific sales order without charge.
*HeaderTextApi* | [**aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDPatch**](docs/Api/HeaderTextApi.md#aslsordwthoutchrgtextsalesorderwithoutchargesalesorderwithoutchargelanguagelanguagelongtextidlongtextidpatch) | **PATCH** /A_SlsOrdWthoutChrgText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;) | Updates a specific header text for a specific sales order without charge.
*HeaderTextApi* | [**aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeGet**](docs/Api/HeaderTextApi.md#aslsordwthoutchrgtextsalesorderwithoutchargesalesorderwithoutchargelanguagelanguagelongtextidlongtextidtosalesorderwithoutchargeget) | **GET** /A_SlsOrdWthoutChrgText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific header text.
*ItemPartnerApi* | [**aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToPartnerGet**](docs/Api/ItemPartnerApi.md#asalesorderwithoutchargeitemsalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitemtopartnerget) | **GET** /A_SalesOrderWithoutChargeItem(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;)/to_Partner | Reads the item partners of a specific sales order without charge item.
*ItemPartnerApi* | [**aSlsOrdWthoutChrgItmPartnerGet**](docs/Api/ItemPartnerApi.md#aslsordwthoutchrgitmpartnerget) | **GET** /A_SlsOrdWthoutChrgItmPartner | Reads the item partners for all sales order without charges.
*ItemPartnerApi* | [**aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionDelete**](docs/Api/ItemPartnerApi.md#aslsordwthoutchrgitmpartnersalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitempartnerfunctionpartnerfunctiondelete) | **DELETE** /A_SlsOrdWthoutChrgItmPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;) | Deletes the item partners of a specific item with a specific partner function in a specific sales order without charge.
*ItemPartnerApi* | [**aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionGet**](docs/Api/ItemPartnerApi.md#aslsordwthoutchrgitmpartnersalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitempartnerfunctionpartnerfunctionget) | **GET** /A_SlsOrdWthoutChrgItmPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;) | Reads the item partners of a specific item with a specific partner function in a specific sales order without charge.
*ItemPartnerApi* | [**aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionPatch**](docs/Api/ItemPartnerApi.md#aslsordwthoutchrgitmpartnersalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitempartnerfunctionpartnerfunctionpatch) | **PATCH** /A_SlsOrdWthoutChrgItmPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;) | Updates the item partners of a specific item with a specific partner function in a specific sales order without charge.
*ItemPartnerApi* | [**aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionToItemGet**](docs/Api/ItemPartnerApi.md#aslsordwthoutchrgitmpartnersalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitempartnerfunctionpartnerfunctiontoitemget) | **GET** /A_SlsOrdWthoutChrgItmPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;)/to_Item | Reads the sales order without charge item for a specific partner function of a sales order without charge item.
*ItemPartnerApi* | [**aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionToSalesOrderWithoutChargeGet**](docs/Api/ItemPartnerApi.md#aslsordwthoutchrgitmpartnersalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitempartnerfunctionpartnerfunctiontosalesorderwithoutchargeget) | **GET** /A_SlsOrdWthoutChrgItmPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific partner function of a sales order without charge item.
*ItemScheduleLineApi* | [**aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToScheduleLineGet**](docs/Api/ItemScheduleLineApi.md#asalesorderwithoutchargeitemsalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitemtoschedulelineget) | **GET** /A_SalesOrderWithoutChargeItem(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;)/to_ScheduleLine | Reads the schedule lines of a specific sales order without charge item.
*ItemScheduleLineApi* | [**aSlsOrdWthoutChrgSchedLineGet**](docs/Api/ItemScheduleLineApi.md#aslsordwthoutchrgschedlineget) | **GET** /A_SlsOrdWthoutChrgSchedLine | Reads the schedule lines of all sales order without charges.
*ItemScheduleLineApi* | [**aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineGet**](docs/Api/ItemScheduleLineApi.md#aslsordwthoutchrgschedlinesalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitemschedulelineschedulelineget) | **GET** /A_SlsOrdWthoutChrgSchedLine(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,ScheduleLine&#x3D;&#39;{ScheduleLine}&#39;) | Reads a specific schedule line.
*ItemScheduleLineApi* | [**aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineToItemGet**](docs/Api/ItemScheduleLineApi.md#aslsordwthoutchrgschedlinesalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitemschedulelineschedulelinetoitemget) | **GET** /A_SlsOrdWthoutChrgSchedLine(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,ScheduleLine&#x3D;&#39;{ScheduleLine}&#39;)/to_Item | Reads the sales order without charge item for a specific schedule line.
*ItemScheduleLineApi* | [**aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineToSalesOrderWithoutChargeGet**](docs/Api/ItemScheduleLineApi.md#aslsordwthoutchrgschedlinesalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitemschedulelineschedulelinetosalesorderwithoutchargeget) | **GET** /A_SlsOrdWthoutChrgSchedLine(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,ScheduleLine&#x3D;&#39;{ScheduleLine}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific schedule line.
*ItemTextApi* | [**aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToTextGet**](docs/Api/ItemTextApi.md#asalesorderwithoutchargeitemsalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitemtotextget) | **GET** /A_SalesOrderWithoutChargeItem(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;)/to_Text | Reads the text of a specific sales order without charge item.
*ItemTextApi* | [**aSlsOrdWthoutChrgItmTextGet**](docs/Api/ItemTextApi.md#aslsordwthoutchrgitmtextget) | **GET** /A_SlsOrdWthoutChrgItmText | Reads item texts of all sales order without charges.
*ItemTextApi* | [**aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDDelete**](docs/Api/ItemTextApi.md#aslsordwthoutchrgitmtextsalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitemlanguagelanguagelongtextidlongtextiddelete) | **DELETE** /A_SlsOrdWthoutChrgItmText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;) | Deletes a specific item text.
*ItemTextApi* | [**aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDGet**](docs/Api/ItemTextApi.md#aslsordwthoutchrgitmtextsalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitemlanguagelanguagelongtextidlongtextidget) | **GET** /A_SlsOrdWthoutChrgItmText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;) | Reads a specific item text.
*ItemTextApi* | [**aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDPatch**](docs/Api/ItemTextApi.md#aslsordwthoutchrgitmtextsalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitemlanguagelanguagelongtextidlongtextidpatch) | **PATCH** /A_SlsOrdWthoutChrgItmText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;) | Updates a specific item text.
*ItemTextApi* | [**aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeGet**](docs/Api/ItemTextApi.md#aslsordwthoutchrgitmtextsalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitemlanguagelanguagelongtextidlongtextidtosalesorderwithoutchargeget) | **GET** /A_SlsOrdWthoutChrgItmText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific text of a sales order without charge item.
*ItemTextApi* | [**aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeItemGet**](docs/Api/ItemTextApi.md#aslsordwthoutchrgitmtextsalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitemlanguagelanguagelongtextidlongtextidtosalesorderwithoutchargeitemget) | **GET** /A_SlsOrdWthoutChrgItmText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;)/to_SalesOrderWithoutChargeItem | Reads the sales order without charge item for a specific item text.
*SalesOrderWithoutChargeHeaderApi* | [**aSalesOrderWithoutChargeGet**](docs/Api/SalesOrderWithoutChargeHeaderApi.md#asalesorderwithoutchargeget) | **GET** /A_SalesOrderWithoutCharge | Reads all sales order without charge headers.
*SalesOrderWithoutChargeHeaderApi* | [**aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToSalesOrderWithoutChargeGet**](docs/Api/SalesOrderWithoutChargeHeaderApi.md#asalesorderwithoutchargeitemsalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitemtosalesorderwithoutchargeget) | **GET** /A_SalesOrderWithoutChargeItem(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific item.
*SalesOrderWithoutChargeHeaderApi* | [**aSalesOrderWithoutChargePost**](docs/Api/SalesOrderWithoutChargeHeaderApi.md#asalesorderwithoutchargepost) | **POST** /A_SalesOrderWithoutCharge | Creates a sales order without charge.
*SalesOrderWithoutChargeHeaderApi* | [**aSalesOrderWithoutChargeSalesOrderWithoutChargeDelete**](docs/Api/SalesOrderWithoutChargeHeaderApi.md#asalesorderwithoutchargesalesorderwithoutchargedelete) | **DELETE** /A_SalesOrderWithoutCharge(&#39;{SalesOrderWithoutCharge}&#39;) | Deletes a specific sales order without charge.
*SalesOrderWithoutChargeHeaderApi* | [**aSalesOrderWithoutChargeSalesOrderWithoutChargeGet**](docs/Api/SalesOrderWithoutChargeHeaderApi.md#asalesorderwithoutchargesalesorderwithoutchargeget) | **GET** /A_SalesOrderWithoutCharge(&#39;{SalesOrderWithoutCharge}&#39;) | Reads the header of a specific sales order without charge.
*SalesOrderWithoutChargeHeaderApi* | [**aSalesOrderWithoutChargeSalesOrderWithoutChargePatch**](docs/Api/SalesOrderWithoutChargeHeaderApi.md#asalesorderwithoutchargesalesorderwithoutchargepatch) | **PATCH** /A_SalesOrderWithoutCharge(&#39;{SalesOrderWithoutCharge}&#39;) | Updates a specific sales order without charge.
*SalesOrderWithoutChargeHeaderApi* | [**aSalesOrderWithoutChargeSalesOrderWithoutChargeToItemGet**](docs/Api/SalesOrderWithoutChargeHeaderApi.md#asalesorderwithoutchargesalesorderwithoutchargetoitemget) | **GET** /A_SalesOrderWithoutCharge(&#39;{SalesOrderWithoutCharge}&#39;)/to_Item | Reads all items of a specific sales order without charge.
*SalesOrderWithoutChargeHeaderApi* | [**aSalesOrderWithoutChargeSalesOrderWithoutChargeToItemPost**](docs/Api/SalesOrderWithoutChargeHeaderApi.md#asalesorderwithoutchargesalesorderwithoutchargetoitempost) | **POST** /A_SalesOrderWithoutCharge(&#39;{SalesOrderWithoutCharge}&#39;)/to_Item | Creates a sales order without charge item for a specific sales order without charge.
*SalesOrderWithoutChargeHeaderApi* | [**aSalesOrderWithoutChargeSalesOrderWithoutChargeToPartnerGet**](docs/Api/SalesOrderWithoutChargeHeaderApi.md#asalesorderwithoutchargesalesorderwithoutchargetopartnerget) | **GET** /A_SalesOrderWithoutCharge(&#39;{SalesOrderWithoutCharge}&#39;)/to_Partner | Reads the header partners of a specific sales order without charge.
*SalesOrderWithoutChargeHeaderApi* | [**aSalesOrderWithoutChargeSalesOrderWithoutChargeToTextGet**](docs/Api/SalesOrderWithoutChargeHeaderApi.md#asalesorderwithoutchargesalesorderwithoutchargetotextget) | **GET** /A_SalesOrderWithoutCharge(&#39;{SalesOrderWithoutCharge}&#39;)/to_Text | Reads the header texts of a specific sales order without charge.
*SalesOrderWithoutChargeHeaderApi* | [**aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionToSalesOrderWithoutChargeGet**](docs/Api/SalesOrderWithoutChargeHeaderApi.md#aslsordwthoutchrgitmpartnersalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitempartnerfunctionpartnerfunctiontosalesorderwithoutchargeget) | **GET** /A_SlsOrdWthoutChrgItmPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific partner function of a sales order without charge item.
*SalesOrderWithoutChargeHeaderApi* | [**aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeGet**](docs/Api/SalesOrderWithoutChargeHeaderApi.md#aslsordwthoutchrgitmtextsalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitemlanguagelanguagelongtextidlongtextidtosalesorderwithoutchargeget) | **GET** /A_SlsOrdWthoutChrgItmText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific text of a sales order without charge item.
*SalesOrderWithoutChargeHeaderApi* | [**aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionToSalesOrderWithoutChargeGet**](docs/Api/SalesOrderWithoutChargeHeaderApi.md#aslsordwthoutchrgpartnersalesorderwithoutchargesalesorderwithoutchargepartnerfunctionpartnerfunctiontosalesorderwithoutchargeget) | **GET** /A_SlsOrdWthoutChrgPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific header partner.
*SalesOrderWithoutChargeHeaderApi* | [**aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineToSalesOrderWithoutChargeGet**](docs/Api/SalesOrderWithoutChargeHeaderApi.md#aslsordwthoutchrgschedlinesalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitemschedulelineschedulelinetosalesorderwithoutchargeget) | **GET** /A_SlsOrdWthoutChrgSchedLine(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,ScheduleLine&#x3D;&#39;{ScheduleLine}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific schedule line.
*SalesOrderWithoutChargeHeaderApi* | [**aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeGet**](docs/Api/SalesOrderWithoutChargeHeaderApi.md#aslsordwthoutchrgtextsalesorderwithoutchargesalesorderwithoutchargelanguagelanguagelongtextidlongtextidtosalesorderwithoutchargeget) | **GET** /A_SlsOrdWthoutChrgText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific header text.
*SalesOrderWithoutChargeItemApi* | [**aSalesOrderWithoutChargeItemGet**](docs/Api/SalesOrderWithoutChargeItemApi.md#asalesorderwithoutchargeitemget) | **GET** /A_SalesOrderWithoutChargeItem | Reads all sales order without charge items.
*SalesOrderWithoutChargeItemApi* | [**aSalesOrderWithoutChargeItemPost**](docs/Api/SalesOrderWithoutChargeItemApi.md#asalesorderwithoutchargeitempost) | **POST** /A_SalesOrderWithoutChargeItem | Creates a sales order without charge item.
*SalesOrderWithoutChargeItemApi* | [**aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemDelete**](docs/Api/SalesOrderWithoutChargeItemApi.md#asalesorderwithoutchargeitemsalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitemdelete) | **DELETE** /A_SalesOrderWithoutChargeItem(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;) | Deletes a specific sales order without charge item.
*SalesOrderWithoutChargeItemApi* | [**aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemGet**](docs/Api/SalesOrderWithoutChargeItemApi.md#asalesorderwithoutchargeitemsalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitemget) | **GET** /A_SalesOrderWithoutChargeItem(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;) | Reads a specific sales order without charge item.
*SalesOrderWithoutChargeItemApi* | [**aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPatch**](docs/Api/SalesOrderWithoutChargeItemApi.md#asalesorderwithoutchargeitemsalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitempatch) | **PATCH** /A_SalesOrderWithoutChargeItem(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;) | Updates a specific sales order without charge item.
*SalesOrderWithoutChargeItemApi* | [**aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToPartnerGet**](docs/Api/SalesOrderWithoutChargeItemApi.md#asalesorderwithoutchargeitemsalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitemtopartnerget) | **GET** /A_SalesOrderWithoutChargeItem(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;)/to_Partner | Reads the item partners of a specific sales order without charge item.
*SalesOrderWithoutChargeItemApi* | [**aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToSalesOrderWithoutChargeGet**](docs/Api/SalesOrderWithoutChargeItemApi.md#asalesorderwithoutchargeitemsalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitemtosalesorderwithoutchargeget) | **GET** /A_SalesOrderWithoutChargeItem(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific item.
*SalesOrderWithoutChargeItemApi* | [**aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToScheduleLineGet**](docs/Api/SalesOrderWithoutChargeItemApi.md#asalesorderwithoutchargeitemsalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitemtoschedulelineget) | **GET** /A_SalesOrderWithoutChargeItem(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;)/to_ScheduleLine | Reads the schedule lines of a specific sales order without charge item.
*SalesOrderWithoutChargeItemApi* | [**aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToTextGet**](docs/Api/SalesOrderWithoutChargeItemApi.md#asalesorderwithoutchargeitemsalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitemtotextget) | **GET** /A_SalesOrderWithoutChargeItem(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;)/to_Text | Reads the text of a specific sales order without charge item.
*SalesOrderWithoutChargeItemApi* | [**aSalesOrderWithoutChargeSalesOrderWithoutChargeToItemGet**](docs/Api/SalesOrderWithoutChargeItemApi.md#asalesorderwithoutchargesalesorderwithoutchargetoitemget) | **GET** /A_SalesOrderWithoutCharge(&#39;{SalesOrderWithoutCharge}&#39;)/to_Item | Reads all items of a specific sales order without charge.
*SalesOrderWithoutChargeItemApi* | [**aSalesOrderWithoutChargeSalesOrderWithoutChargeToItemPost**](docs/Api/SalesOrderWithoutChargeItemApi.md#asalesorderwithoutchargesalesorderwithoutchargetoitempost) | **POST** /A_SalesOrderWithoutCharge(&#39;{SalesOrderWithoutCharge}&#39;)/to_Item | Creates a sales order without charge item for a specific sales order without charge.
*SalesOrderWithoutChargeItemApi* | [**aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionToItemGet**](docs/Api/SalesOrderWithoutChargeItemApi.md#aslsordwthoutchrgitmpartnersalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitempartnerfunctionpartnerfunctiontoitemget) | **GET** /A_SlsOrdWthoutChrgItmPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;)/to_Item | Reads the sales order without charge item for a specific partner function of a sales order without charge item.
*SalesOrderWithoutChargeItemApi* | [**aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeItemGet**](docs/Api/SalesOrderWithoutChargeItemApi.md#aslsordwthoutchrgitmtextsalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitemlanguagelanguagelongtextidlongtextidtosalesorderwithoutchargeitemget) | **GET** /A_SlsOrdWthoutChrgItmText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;)/to_SalesOrderWithoutChargeItem | Reads the sales order without charge item for a specific item text.
*SalesOrderWithoutChargeItemApi* | [**aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineToItemGet**](docs/Api/SalesOrderWithoutChargeItemApi.md#aslsordwthoutchrgschedlinesalesorderwithoutchargesalesorderwithoutchargesalesorderwithoutchargeitemsalesorderwithoutchargeitemschedulelineschedulelinetoitemget) | **GET** /A_SlsOrdWthoutChrgSchedLine(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,ScheduleLine&#x3D;&#39;{ScheduleLine}&#39;)/to_Item | Reads the sales order without charge item for a specific schedule line.

## Models

- [APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeItemType](docs/Model/APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeItemType.md)
- [APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeItemTypeCreate](docs/Model/APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeItemTypeCreate.md)
- [APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeItemTypeCreateToPartner](docs/Model/APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeItemTypeCreateToPartner.md)
- [APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeItemTypeCreateToScheduleLine](docs/Model/APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeItemTypeCreateToScheduleLine.md)
- [APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeItemTypeCreateToText](docs/Model/APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeItemTypeCreateToText.md)
- [APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeItemTypeToPartner](docs/Model/APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeItemTypeToPartner.md)
- [APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeItemTypeToScheduleLine](docs/Model/APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeItemTypeToScheduleLine.md)
- [APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeItemTypeToText](docs/Model/APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeItemTypeToText.md)
- [APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeItemTypeUpdate](docs/Model/APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeItemTypeUpdate.md)
- [APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeType](docs/Model/APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeType.md)
- [APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeTypeCreate](docs/Model/APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeTypeCreate.md)
- [APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeTypeCreateToItem](docs/Model/APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeTypeCreateToItem.md)
- [APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeTypeCreateToPartner](docs/Model/APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeTypeCreateToPartner.md)
- [APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeTypeCreateToText](docs/Model/APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeTypeCreateToText.md)
- [APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeTypeToItem](docs/Model/APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeTypeToItem.md)
- [APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeTypeToPartner](docs/Model/APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeTypeToPartner.md)
- [APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeTypeToText](docs/Model/APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeTypeToText.md)
- [APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeTypeUpdate](docs/Model/APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeTypeUpdate.md)
- [APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgItmPartnerType](docs/Model/APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgItmPartnerType.md)
- [APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgItmPartnerTypeCreate](docs/Model/APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgItmPartnerTypeCreate.md)
- [APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgItmPartnerTypeUpdate](docs/Model/APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgItmPartnerTypeUpdate.md)
- [APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgItmTextType](docs/Model/APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgItmTextType.md)
- [APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgItmTextTypeCreate](docs/Model/APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgItmTextTypeCreate.md)
- [APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgItmTextTypeUpdate](docs/Model/APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgItmTextTypeUpdate.md)
- [APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgPartnerType](docs/Model/APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgPartnerType.md)
- [APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgPartnerTypeCreate](docs/Model/APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgPartnerTypeCreate.md)
- [APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgPartnerTypeUpdate](docs/Model/APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgPartnerTypeUpdate.md)
- [APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgSchedLineType](docs/Model/APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgSchedLineType.md)
- [APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgSchedLineTypeCreate](docs/Model/APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgSchedLineTypeCreate.md)
- [APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgSchedLineTypeUpdate](docs/Model/APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgSchedLineTypeUpdate.md)
- [APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgTextType](docs/Model/APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgTextType.md)
- [APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgTextTypeCreate](docs/Model/APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgTextTypeCreate.md)
- [APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgTextTypeUpdate](docs/Model/APISALESORDERWITHOUTCHARGESRVASlsOrdWthoutChrgTextTypeUpdate.md)
- [ASalesOrderWithoutChargeItemType](docs/Model/ASalesOrderWithoutChargeItemType.md)
- [ASalesOrderWithoutChargeType](docs/Model/ASalesOrderWithoutChargeType.md)
- [ASlsOrdWthoutChrgItmPartnerType](docs/Model/ASlsOrdWthoutChrgItmPartnerType.md)
- [ASlsOrdWthoutChrgItmTextType](docs/Model/ASlsOrdWthoutChrgItmTextType.md)
- [ASlsOrdWthoutChrgPartnerType](docs/Model/ASlsOrdWthoutChrgPartnerType.md)
- [ASlsOrdWthoutChrgSchedLineType](docs/Model/ASlsOrdWthoutChrgSchedLineType.md)
- [ASlsOrdWthoutChrgTextType](docs/Model/ASlsOrdWthoutChrgTextType.md)
- [CollectionOfASalesOrderWithoutChargeItemType](docs/Model/CollectionOfASalesOrderWithoutChargeItemType.md)
- [CollectionOfASalesOrderWithoutChargeType](docs/Model/CollectionOfASalesOrderWithoutChargeType.md)
- [CollectionOfASlsOrdWthoutChrgItmPartnerType](docs/Model/CollectionOfASlsOrdWthoutChrgItmPartnerType.md)
- [CollectionOfASlsOrdWthoutChrgItmTextType](docs/Model/CollectionOfASlsOrdWthoutChrgItmTextType.md)
- [CollectionOfASlsOrdWthoutChrgPartnerType](docs/Model/CollectionOfASlsOrdWthoutChrgPartnerType.md)
- [CollectionOfASlsOrdWthoutChrgSchedLineType](docs/Model/CollectionOfASlsOrdWthoutChrgSchedLineType.md)
- [CollectionOfASlsOrdWthoutChrgTextType](docs/Model/CollectionOfASlsOrdWthoutChrgTextType.md)
- [Error](docs/Model/Error.md)
- [ErrorError](docs/Model/ErrorError.md)
- [ErrorErrorMessage](docs/Model/ErrorErrorMessage.md)
- [ModifiedASalesOrderWithoutChargeItemType](docs/Model/ModifiedASalesOrderWithoutChargeItemType.md)
- [ModifiedASalesOrderWithoutChargeType](docs/Model/ModifiedASalesOrderWithoutChargeType.md)
- [ModifiedASlsOrdWthoutChrgItmPartnerType](docs/Model/ModifiedASlsOrdWthoutChrgItmPartnerType.md)
- [ModifiedASlsOrdWthoutChrgItmTextType](docs/Model/ModifiedASlsOrdWthoutChrgItmTextType.md)
- [ModifiedASlsOrdWthoutChrgPartnerType](docs/Model/ModifiedASlsOrdWthoutChrgPartnerType.md)
- [ModifiedASlsOrdWthoutChrgTextType](docs/Model/ModifiedASlsOrdWthoutChrgTextType.md)
- [Wrapper](docs/Model/Wrapper.md)
- [Wrapper1](docs/Model/Wrapper1.md)
- [Wrapper2](docs/Model/Wrapper2.md)
- [Wrapper3](docs/Model/Wrapper3.md)
- [Wrapper4](docs/Model/Wrapper4.md)
- [Wrapper5](docs/Model/Wrapper5.md)
- [Wrapper6](docs/Model/Wrapper6.md)

## Authorization

Authentication schemes defined for the API:
### OAuth2Auth

- **Type**: `OAuth`
- **Flow**: `accessCode`
- **Authorization URL**: `https://{host}:{port}`
- **Scopes**: 
    - **API_SALES_ORDER_WITHOUT_CHARGE_SRV_0001**: 

### BasicAuth

- **Type**: HTTP basic authentication

## Tests

To run the tests, use:

```bash
composer install
vendor/bin/phpunit
```

## Author



## About this package

This PHP package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

- API version: `1.0.0`
- Build package: `org.openapitools.codegen.languages.PhpClientCodegen`
