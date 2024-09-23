# BeLenka\SAP\SalesOrderWOCharge\SalesOrderWithoutChargeHeaderApi

All URIs are relative to https://:/sap/opu/odata/sap/API_SALES_ORDER_WITHOUT_CHARGE_SRV, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**aSalesOrderWithoutChargeGet()**](SalesOrderWithoutChargeHeaderApi.md#aSalesOrderWithoutChargeGet) | **GET** /A_SalesOrderWithoutCharge | Reads all sales order without charge headers. |
| [**aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToSalesOrderWithoutChargeGet()**](SalesOrderWithoutChargeHeaderApi.md#aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToSalesOrderWithoutChargeGet) | **GET** /A_SalesOrderWithoutChargeItem(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific item. |
| [**aSalesOrderWithoutChargePost()**](SalesOrderWithoutChargeHeaderApi.md#aSalesOrderWithoutChargePost) | **POST** /A_SalesOrderWithoutCharge | Creates a sales order without charge. |
| [**aSalesOrderWithoutChargeSalesOrderWithoutChargeDelete()**](SalesOrderWithoutChargeHeaderApi.md#aSalesOrderWithoutChargeSalesOrderWithoutChargeDelete) | **DELETE** /A_SalesOrderWithoutCharge(&#39;{SalesOrderWithoutCharge}&#39;) | Deletes a specific sales order without charge. |
| [**aSalesOrderWithoutChargeSalesOrderWithoutChargeGet()**](SalesOrderWithoutChargeHeaderApi.md#aSalesOrderWithoutChargeSalesOrderWithoutChargeGet) | **GET** /A_SalesOrderWithoutCharge(&#39;{SalesOrderWithoutCharge}&#39;) | Reads the header of a specific sales order without charge. |
| [**aSalesOrderWithoutChargeSalesOrderWithoutChargePatch()**](SalesOrderWithoutChargeHeaderApi.md#aSalesOrderWithoutChargeSalesOrderWithoutChargePatch) | **PATCH** /A_SalesOrderWithoutCharge(&#39;{SalesOrderWithoutCharge}&#39;) | Updates a specific sales order without charge. |
| [**aSalesOrderWithoutChargeSalesOrderWithoutChargeToItemGet()**](SalesOrderWithoutChargeHeaderApi.md#aSalesOrderWithoutChargeSalesOrderWithoutChargeToItemGet) | **GET** /A_SalesOrderWithoutCharge(&#39;{SalesOrderWithoutCharge}&#39;)/to_Item | Reads all items of a specific sales order without charge. |
| [**aSalesOrderWithoutChargeSalesOrderWithoutChargeToItemPost()**](SalesOrderWithoutChargeHeaderApi.md#aSalesOrderWithoutChargeSalesOrderWithoutChargeToItemPost) | **POST** /A_SalesOrderWithoutCharge(&#39;{SalesOrderWithoutCharge}&#39;)/to_Item | Creates a sales order without charge item for a specific sales order without charge. |
| [**aSalesOrderWithoutChargeSalesOrderWithoutChargeToPartnerGet()**](SalesOrderWithoutChargeHeaderApi.md#aSalesOrderWithoutChargeSalesOrderWithoutChargeToPartnerGet) | **GET** /A_SalesOrderWithoutCharge(&#39;{SalesOrderWithoutCharge}&#39;)/to_Partner | Reads the header partners of a specific sales order without charge. |
| [**aSalesOrderWithoutChargeSalesOrderWithoutChargeToTextGet()**](SalesOrderWithoutChargeHeaderApi.md#aSalesOrderWithoutChargeSalesOrderWithoutChargeToTextGet) | **GET** /A_SalesOrderWithoutCharge(&#39;{SalesOrderWithoutCharge}&#39;)/to_Text | Reads the header texts of a specific sales order without charge. |
| [**aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionToSalesOrderWithoutChargeGet()**](SalesOrderWithoutChargeHeaderApi.md#aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionToSalesOrderWithoutChargeGet) | **GET** /A_SlsOrdWthoutChrgItmPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific partner function of a sales order without charge item. |
| [**aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeGet()**](SalesOrderWithoutChargeHeaderApi.md#aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeGet) | **GET** /A_SlsOrdWthoutChrgItmText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific text of a sales order without charge item. |
| [**aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionToSalesOrderWithoutChargeGet()**](SalesOrderWithoutChargeHeaderApi.md#aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionToSalesOrderWithoutChargeGet) | **GET** /A_SlsOrdWthoutChrgPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific header partner. |
| [**aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineToSalesOrderWithoutChargeGet()**](SalesOrderWithoutChargeHeaderApi.md#aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineToSalesOrderWithoutChargeGet) | **GET** /A_SlsOrdWthoutChrgSchedLine(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,ScheduleLine&#x3D;&#39;{ScheduleLine}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific schedule line. |
| [**aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeGet()**](SalesOrderWithoutChargeHeaderApi.md#aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeGet) | **GET** /A_SlsOrdWthoutChrgText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific header text. |


## `aSalesOrderWithoutChargeGet()`

```php
aSalesOrderWithoutChargeGet($top, $skip, $filter, $inlinecount, $orderby, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper
```

Reads all sales order without charge headers.

Reads the header data of all sales order without charges in the system.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: BasicAuth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');

// Configure OAuth2 access token for authorization: OAuth2Auth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\SalesOrderWithoutChargeHeaderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$top = 50; // int | Show only the first n items, see [Paging - Top](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=66)
$skip = 56; // int | Skip the first n items, see [Paging - Skip](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=65)
$filter = 'filter_example'; // string | Filter items by property values, see [Filtering](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=64)
$inlinecount = 'inlinecount_example'; // string | Include count of items, see [Inlinecount](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=67)
$orderby = array('orderby_example'); // string[] | Order items by property values, see [Sorting](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=65)
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=68)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=63)

try {
    $result = $apiInstance->aSalesOrderWithoutChargeGet($top, $skip, $filter, $inlinecount, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SalesOrderWithoutChargeHeaderApi->aSalesOrderWithoutChargeGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **top** | **int**| Show only the first n items, see [Paging - Top](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;66) | [optional] |
| **skip** | **int**| Skip the first n items, see [Paging - Skip](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;65) | [optional] |
| **filter** | **string**| Filter items by property values, see [Filtering](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;64) | [optional] |
| **inlinecount** | **string**| Include count of items, see [Inlinecount](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;67) | [optional] |
| **orderby** | [**string[]**](../Model/string.md)| Order items by property values, see [Sorting](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;65) | [optional] |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;68) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;63) | [optional] |

### Return type

[**\BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper**](../Model/Wrapper.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToSalesOrderWithoutChargeGet()`

```php
aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToSalesOrderWithoutChargeGet($sales_order_without_charge, $sales_order_without_charge_item, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeType
```

Reads the sales order without charge header for a specific item.

Reads the sales order without charge header data for a specific item. Consumers must pass the following key fields: sales order without charge ID and item number.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: BasicAuth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');

// Configure OAuth2 access token for authorization: OAuth2Auth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\SalesOrderWithoutChargeHeaderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sales_order_without_charge = 'sales_order_without_charge_example'; // string | Sales Order Without Charge
$sales_order_without_charge_item = 'sales_order_without_charge_item_example'; // string | Sales Order Without Charge Item
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=68)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=63)

try {
    $result = $apiInstance->aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToSalesOrderWithoutChargeGet($sales_order_without_charge, $sales_order_without_charge_item, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SalesOrderWithoutChargeHeaderApi->aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToSalesOrderWithoutChargeGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sales_order_without_charge** | **string**| Sales Order Without Charge | |
| **sales_order_without_charge_item** | **string**| Sales Order Without Charge Item | |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;68) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;63) | [optional] |

### Return type

[**\BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeType**](../Model/ASalesOrderWithoutChargeType.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSalesOrderWithoutChargePost()`

```php
aSalesOrderWithoutChargePost($apisalesorderwithoutchargesrva_sales_order_without_charge_type_create): \BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeType
```

Creates a sales order without charge.

Creates a sales order without charge header using deep insert requests. This means consumers can create a sales order without charge with all possible sub-entities (for example, header partners or items).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: BasicAuth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');

// Configure OAuth2 access token for authorization: OAuth2Auth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\SalesOrderWithoutChargeHeaderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$apisalesorderwithoutchargesrva_sales_order_without_charge_type_create = new \BeLenka\SAP\SalesOrderWOCharge\Model\APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeTypeCreate(); // \BeLenka\SAP\SalesOrderWOCharge\Model\APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeTypeCreate | New entity

try {
    $result = $apiInstance->aSalesOrderWithoutChargePost($apisalesorderwithoutchargesrva_sales_order_without_charge_type_create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SalesOrderWithoutChargeHeaderApi->aSalesOrderWithoutChargePost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **apisalesorderwithoutchargesrva_sales_order_without_charge_type_create** | [**\BeLenka\SAP\SalesOrderWOCharge\Model\APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeTypeCreate**](../Model/APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeTypeCreate.md)| New entity | |

### Return type

[**\BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeType**](../Model/ASalesOrderWithoutChargeType.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSalesOrderWithoutChargeSalesOrderWithoutChargeDelete()`

```php
aSalesOrderWithoutChargeSalesOrderWithoutChargeDelete($sales_order_without_charge)
```

Deletes a specific sales order without charge.

Deletes the header data of a specific sales order without charge. Consumers must pass the sales order without charge ID (key field).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: BasicAuth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');

// Configure OAuth2 access token for authorization: OAuth2Auth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\SalesOrderWithoutChargeHeaderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sales_order_without_charge = 'sales_order_without_charge_example'; // string | Sales Order Without Charge

try {
    $apiInstance->aSalesOrderWithoutChargeSalesOrderWithoutChargeDelete($sales_order_without_charge);
} catch (Exception $e) {
    echo 'Exception when calling SalesOrderWithoutChargeHeaderApi->aSalesOrderWithoutChargeSalesOrderWithoutChargeDelete: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sales_order_without_charge** | **string**| Sales Order Without Charge | |

### Return type

void (empty response body)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSalesOrderWithoutChargeSalesOrderWithoutChargeGet()`

```php
aSalesOrderWithoutChargeSalesOrderWithoutChargeGet($sales_order_without_charge, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeType
```

Reads the header of a specific sales order without charge.

Reads the header data of a specific sales order without charge. Consumers must pass the sales order without charge ID (key field).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: BasicAuth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');

// Configure OAuth2 access token for authorization: OAuth2Auth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\SalesOrderWithoutChargeHeaderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sales_order_without_charge = 'sales_order_without_charge_example'; // string | Sales Order Without Charge
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=68)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=63)

try {
    $result = $apiInstance->aSalesOrderWithoutChargeSalesOrderWithoutChargeGet($sales_order_without_charge, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SalesOrderWithoutChargeHeaderApi->aSalesOrderWithoutChargeSalesOrderWithoutChargeGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sales_order_without_charge** | **string**| Sales Order Without Charge | |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;68) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;63) | [optional] |

### Return type

[**\BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeType**](../Model/ASalesOrderWithoutChargeType.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSalesOrderWithoutChargeSalesOrderWithoutChargePatch()`

```php
aSalesOrderWithoutChargeSalesOrderWithoutChargePatch($sales_order_without_charge, $modified_a_sales_order_without_charge_type)
```

Updates a specific sales order without charge.

Updates the header data of a specific sales order without charge. Consumers must pass the sales order without charge ID (key field).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: BasicAuth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');

// Configure OAuth2 access token for authorization: OAuth2Auth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\SalesOrderWithoutChargeHeaderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sales_order_without_charge = 'sales_order_without_charge_example'; // string | Sales Order Without Charge
$modified_a_sales_order_without_charge_type = new \BeLenka\SAP\SalesOrderWOCharge\Model\ModifiedASalesOrderWithoutChargeType(); // \BeLenka\SAP\SalesOrderWOCharge\Model\ModifiedASalesOrderWithoutChargeType | New property values

try {
    $apiInstance->aSalesOrderWithoutChargeSalesOrderWithoutChargePatch($sales_order_without_charge, $modified_a_sales_order_without_charge_type);
} catch (Exception $e) {
    echo 'Exception when calling SalesOrderWithoutChargeHeaderApi->aSalesOrderWithoutChargeSalesOrderWithoutChargePatch: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sales_order_without_charge** | **string**| Sales Order Without Charge | |
| **modified_a_sales_order_without_charge_type** | [**\BeLenka\SAP\SalesOrderWOCharge\Model\ModifiedASalesOrderWithoutChargeType**](../Model/ModifiedASalesOrderWithoutChargeType.md)| New property values | |

### Return type

void (empty response body)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSalesOrderWithoutChargeSalesOrderWithoutChargeToItemGet()`

```php
aSalesOrderWithoutChargeSalesOrderWithoutChargeToItemGet($sales_order_without_charge, $top, $skip, $filter, $inlinecount, $orderby, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper1
```

Reads all items of a specific sales order without charge.

Reads all item data of a specific sales order without charge. Consumers must pass the sales order without charge ID (key field).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: BasicAuth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');

// Configure OAuth2 access token for authorization: OAuth2Auth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\SalesOrderWithoutChargeHeaderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sales_order_without_charge = 'sales_order_without_charge_example'; // string | Sales Order Without Charge
$top = 50; // int | Show only the first n items, see [Paging - Top](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=66)
$skip = 56; // int | Skip the first n items, see [Paging - Skip](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=65)
$filter = 'filter_example'; // string | Filter items by property values, see [Filtering](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=64)
$inlinecount = 'inlinecount_example'; // string | Include count of items, see [Inlinecount](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=67)
$orderby = array('orderby_example'); // string[] | Order items by property values, see [Sorting](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=65)
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=68)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=63)

try {
    $result = $apiInstance->aSalesOrderWithoutChargeSalesOrderWithoutChargeToItemGet($sales_order_without_charge, $top, $skip, $filter, $inlinecount, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SalesOrderWithoutChargeHeaderApi->aSalesOrderWithoutChargeSalesOrderWithoutChargeToItemGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sales_order_without_charge** | **string**| Sales Order Without Charge | |
| **top** | **int**| Show only the first n items, see [Paging - Top](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;66) | [optional] |
| **skip** | **int**| Skip the first n items, see [Paging - Skip](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;65) | [optional] |
| **filter** | **string**| Filter items by property values, see [Filtering](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;64) | [optional] |
| **inlinecount** | **string**| Include count of items, see [Inlinecount](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;67) | [optional] |
| **orderby** | [**string[]**](../Model/string.md)| Order items by property values, see [Sorting](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;65) | [optional] |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;68) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;63) | [optional] |

### Return type

[**\BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper1**](../Model/Wrapper1.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSalesOrderWithoutChargeSalesOrderWithoutChargeToItemPost()`

```php
aSalesOrderWithoutChargeSalesOrderWithoutChargeToItemPost($sales_order_without_charge, $apisalesorderwithoutchargesrva_sales_order_without_charge_item_type_create): \BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeItemType
```

Creates a sales order without charge item for a specific sales order without charge.

Creates a sales order without charge item for a specific sales order without charge using deep insert requests. This means consumers can create an item with all possible sub-entities (for example, item partners or item texts).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: BasicAuth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');

// Configure OAuth2 access token for authorization: OAuth2Auth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\SalesOrderWithoutChargeHeaderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sales_order_without_charge = 'sales_order_without_charge_example'; // string | Sales Order Without Charge
$apisalesorderwithoutchargesrva_sales_order_without_charge_item_type_create = new \BeLenka\SAP\SalesOrderWOCharge\Model\APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeItemTypeCreate(); // \BeLenka\SAP\SalesOrderWOCharge\Model\APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeItemTypeCreate | New entity

try {
    $result = $apiInstance->aSalesOrderWithoutChargeSalesOrderWithoutChargeToItemPost($sales_order_without_charge, $apisalesorderwithoutchargesrva_sales_order_without_charge_item_type_create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SalesOrderWithoutChargeHeaderApi->aSalesOrderWithoutChargeSalesOrderWithoutChargeToItemPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sales_order_without_charge** | **string**| Sales Order Without Charge | |
| **apisalesorderwithoutchargesrva_sales_order_without_charge_item_type_create** | [**\BeLenka\SAP\SalesOrderWOCharge\Model\APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeItemTypeCreate**](../Model/APISALESORDERWITHOUTCHARGESRVASalesOrderWithoutChargeItemTypeCreate.md)| New entity | |

### Return type

[**\BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeItemType**](../Model/ASalesOrderWithoutChargeItemType.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSalesOrderWithoutChargeSalesOrderWithoutChargeToPartnerGet()`

```php
aSalesOrderWithoutChargeSalesOrderWithoutChargeToPartnerGet($sales_order_without_charge, $top, $skip, $filter, $inlinecount, $orderby, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper2
```

Reads the header partners of a specific sales order without charge.

Reads the business partner data from the header of a specific sales order without charge. Consumers must pass the sales order without charge ID (key field). The data is relevant for all items for which no item-specific partners are maintained.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: BasicAuth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');

// Configure OAuth2 access token for authorization: OAuth2Auth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\SalesOrderWithoutChargeHeaderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sales_order_without_charge = 'sales_order_without_charge_example'; // string | Sales Order Without Charge
$top = 50; // int | Show only the first n items, see [Paging - Top](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=66)
$skip = 56; // int | Skip the first n items, see [Paging - Skip](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=65)
$filter = 'filter_example'; // string | Filter items by property values, see [Filtering](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=64)
$inlinecount = 'inlinecount_example'; // string | Include count of items, see [Inlinecount](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=67)
$orderby = array('orderby_example'); // string[] | Order items by property values, see [Sorting](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=65)
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=68)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=63)

try {
    $result = $apiInstance->aSalesOrderWithoutChargeSalesOrderWithoutChargeToPartnerGet($sales_order_without_charge, $top, $skip, $filter, $inlinecount, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SalesOrderWithoutChargeHeaderApi->aSalesOrderWithoutChargeSalesOrderWithoutChargeToPartnerGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sales_order_without_charge** | **string**| Sales Order Without Charge | |
| **top** | **int**| Show only the first n items, see [Paging - Top](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;66) | [optional] |
| **skip** | **int**| Skip the first n items, see [Paging - Skip](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;65) | [optional] |
| **filter** | **string**| Filter items by property values, see [Filtering](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;64) | [optional] |
| **inlinecount** | **string**| Include count of items, see [Inlinecount](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;67) | [optional] |
| **orderby** | [**string[]**](../Model/string.md)| Order items by property values, see [Sorting](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;65) | [optional] |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;68) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;63) | [optional] |

### Return type

[**\BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper2**](../Model/Wrapper2.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSalesOrderWithoutChargeSalesOrderWithoutChargeToTextGet()`

```php
aSalesOrderWithoutChargeSalesOrderWithoutChargeToTextGet($sales_order_without_charge, $top, $skip, $filter, $inlinecount, $orderby, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper3
```

Reads the header texts of a specific sales order without charge.

Reads the text data from the header of a specific sales order without charge. Consumers must pass the sales order without charge ID (key field).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: BasicAuth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');

// Configure OAuth2 access token for authorization: OAuth2Auth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\SalesOrderWithoutChargeHeaderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sales_order_without_charge = 'sales_order_without_charge_example'; // string | Sales Order Without Charge
$top = 50; // int | Show only the first n items, see [Paging - Top](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=66)
$skip = 56; // int | Skip the first n items, see [Paging - Skip](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=65)
$filter = 'filter_example'; // string | Filter items by property values, see [Filtering](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=64)
$inlinecount = 'inlinecount_example'; // string | Include count of items, see [Inlinecount](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=67)
$orderby = array('orderby_example'); // string[] | Order items by property values, see [Sorting](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=65)
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=68)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=63)

try {
    $result = $apiInstance->aSalesOrderWithoutChargeSalesOrderWithoutChargeToTextGet($sales_order_without_charge, $top, $skip, $filter, $inlinecount, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SalesOrderWithoutChargeHeaderApi->aSalesOrderWithoutChargeSalesOrderWithoutChargeToTextGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sales_order_without_charge** | **string**| Sales Order Without Charge | |
| **top** | **int**| Show only the first n items, see [Paging - Top](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;66) | [optional] |
| **skip** | **int**| Skip the first n items, see [Paging - Skip](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;65) | [optional] |
| **filter** | **string**| Filter items by property values, see [Filtering](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;64) | [optional] |
| **inlinecount** | **string**| Include count of items, see [Inlinecount](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;67) | [optional] |
| **orderby** | [**string[]**](../Model/string.md)| Order items by property values, see [Sorting](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;65) | [optional] |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;68) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;63) | [optional] |

### Return type

[**\BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper3**](../Model/Wrapper3.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionToSalesOrderWithoutChargeGet()`

```php
aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionToSalesOrderWithoutChargeGet($sales_order_without_charge, $sales_order_without_charge_item, $partner_function, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeType
```

Reads the sales order without charge header for a specific partner function of a sales order without charge item.

Reads the sales order without charge header data for a specific item partner function. Consumers must pass the following key fields: sales order without charge ID, item number, and partner function.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: BasicAuth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');

// Configure OAuth2 access token for authorization: OAuth2Auth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\SalesOrderWithoutChargeHeaderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sales_order_without_charge = 'sales_order_without_charge_example'; // string | Sales Order Without Charge
$sales_order_without_charge_item = 'sales_order_without_charge_item_example'; // string | Sales Order Without Charge Item
$partner_function = 'partner_function_example'; // string | Partner Function
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=68)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=63)

try {
    $result = $apiInstance->aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionToSalesOrderWithoutChargeGet($sales_order_without_charge, $sales_order_without_charge_item, $partner_function, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SalesOrderWithoutChargeHeaderApi->aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionToSalesOrderWithoutChargeGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sales_order_without_charge** | **string**| Sales Order Without Charge | |
| **sales_order_without_charge_item** | **string**| Sales Order Without Charge Item | |
| **partner_function** | **string**| Partner Function | |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;68) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;63) | [optional] |

### Return type

[**\BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeType**](../Model/ASalesOrderWithoutChargeType.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeGet()`

```php
aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeGet($sales_order_without_charge, $sales_order_without_charge_item, $language, $long_text_id, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeType
```

Reads the sales order without charge header for a specific text of a sales order without charge item.

Reads the sales order without charge header data for a specific text of a specific sales order without charge item in a specific language. Consumers must pass the following key fields: sales order without charge ID, item number, language, and text ID.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: BasicAuth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');

// Configure OAuth2 access token for authorization: OAuth2Auth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\SalesOrderWithoutChargeHeaderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sales_order_without_charge = 'sales_order_without_charge_example'; // string | Sales Order Without Charge
$sales_order_without_charge_item = 'sales_order_without_charge_item_example'; // string | Sales Order Without Charge Item
$language = 'language_example'; // string | Language Key
$long_text_id = 'long_text_id_example'; // string | Text ID
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=68)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=63)

try {
    $result = $apiInstance->aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeGet($sales_order_without_charge, $sales_order_without_charge_item, $language, $long_text_id, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SalesOrderWithoutChargeHeaderApi->aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sales_order_without_charge** | **string**| Sales Order Without Charge | |
| **sales_order_without_charge_item** | **string**| Sales Order Without Charge Item | |
| **language** | **string**| Language Key | |
| **long_text_id** | **string**| Text ID | |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;68) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;63) | [optional] |

### Return type

[**\BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeType**](../Model/ASalesOrderWithoutChargeType.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionToSalesOrderWithoutChargeGet()`

```php
aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionToSalesOrderWithoutChargeGet($sales_order_without_charge, $partner_function, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeType
```

Reads the sales order without charge header for a specific header partner.

Reads the sales order without charge header data for a specific header partner function. Consumers must pass the following key fields: partner function and the sales order without charge ID.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: BasicAuth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');

// Configure OAuth2 access token for authorization: OAuth2Auth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\SalesOrderWithoutChargeHeaderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sales_order_without_charge = 'sales_order_without_charge_example'; // string | Sales Order Without Charge
$partner_function = 'partner_function_example'; // string | Partner Function
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=68)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=63)

try {
    $result = $apiInstance->aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionToSalesOrderWithoutChargeGet($sales_order_without_charge, $partner_function, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SalesOrderWithoutChargeHeaderApi->aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionToSalesOrderWithoutChargeGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sales_order_without_charge** | **string**| Sales Order Without Charge | |
| **partner_function** | **string**| Partner Function | |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;68) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;63) | [optional] |

### Return type

[**\BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeType**](../Model/ASalesOrderWithoutChargeType.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineToSalesOrderWithoutChargeGet()`

```php
aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineToSalesOrderWithoutChargeGet($sales_order_without_charge, $sales_order_without_charge_item, $schedule_line, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeType
```

Reads the sales order without charge header for a specific schedule line.

Reads the sales order without charge header data for a specific schedule line. Consumers must pass the following key fields: sales order without charge ID, item number, and schedule line number.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: BasicAuth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');

// Configure OAuth2 access token for authorization: OAuth2Auth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\SalesOrderWithoutChargeHeaderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sales_order_without_charge = 'sales_order_without_charge_example'; // string | Sales Document
$sales_order_without_charge_item = 'sales_order_without_charge_item_example'; // string | Sales Document Item
$schedule_line = 'schedule_line_example'; // string | Schedule Line Number
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=68)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=63)

try {
    $result = $apiInstance->aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineToSalesOrderWithoutChargeGet($sales_order_without_charge, $sales_order_without_charge_item, $schedule_line, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SalesOrderWithoutChargeHeaderApi->aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineToSalesOrderWithoutChargeGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sales_order_without_charge** | **string**| Sales Document | |
| **sales_order_without_charge_item** | **string**| Sales Document Item | |
| **schedule_line** | **string**| Schedule Line Number | |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;68) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;63) | [optional] |

### Return type

[**\BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeType**](../Model/ASalesOrderWithoutChargeType.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeGet()`

```php
aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeGet($sales_order_without_charge, $language, $long_text_id, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeType
```

Reads the sales order without charge header for a specific header text.

Reads the sales order without charge header data for a specific header text. Consumers must pass the following key fields: sales order without charge ID, language, and text ID.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: BasicAuth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');

// Configure OAuth2 access token for authorization: OAuth2Auth
$config = BeLenka\SAP\SalesOrderWOCharge\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\SalesOrderWithoutChargeHeaderApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sales_order_without_charge = 'sales_order_without_charge_example'; // string | Sales Order Without Charge
$language = 'language_example'; // string | Language Key
$long_text_id = 'long_text_id_example'; // string | Text ID
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=68)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=63)

try {
    $result = $apiInstance->aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeGet($sales_order_without_charge, $language, $long_text_id, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SalesOrderWithoutChargeHeaderApi->aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sales_order_without_charge** | **string**| Sales Order Without Charge | |
| **language** | **string**| Language Key | |
| **long_text_id** | **string**| Text ID | |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;68) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;63) | [optional] |

### Return type

[**\BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeType**](../Model/ASalesOrderWithoutChargeType.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
