# BeLenka\SAP\SalesOrderWOCharge\ItemTextApi

All URIs are relative to https://:/sap/opu/odata/sap/API_SALES_ORDER_WITHOUT_CHARGE_SRV, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToTextGet()**](ItemTextApi.md#aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToTextGet) | **GET** /A_SalesOrderWithoutChargeItem(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;)/to_Text | Reads the text of a specific sales order without charge item. |
| [**aSlsOrdWthoutChrgItmTextGet()**](ItemTextApi.md#aSlsOrdWthoutChrgItmTextGet) | **GET** /A_SlsOrdWthoutChrgItmText | Reads item texts of all sales order without charges. |
| [**aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDDelete()**](ItemTextApi.md#aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDDelete) | **DELETE** /A_SlsOrdWthoutChrgItmText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;) | Deletes a specific item text. |
| [**aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDGet()**](ItemTextApi.md#aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDGet) | **GET** /A_SlsOrdWthoutChrgItmText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;) | Reads a specific item text. |
| [**aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDPatch()**](ItemTextApi.md#aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDPatch) | **PATCH** /A_SlsOrdWthoutChrgItmText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;) | Updates a specific item text. |
| [**aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeGet()**](ItemTextApi.md#aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeGet) | **GET** /A_SlsOrdWthoutChrgItmText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific text of a sales order without charge item. |
| [**aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeItemGet()**](ItemTextApi.md#aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeItemGet) | **GET** /A_SlsOrdWthoutChrgItmText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;)/to_SalesOrderWithoutChargeItem | Reads the sales order without charge item for a specific item text. |


## `aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToTextGet()`

```php
aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToTextGet($sales_order_without_charge, $sales_order_without_charge_item, $top, $skip, $filter, $inlinecount, $orderby, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper6
```

Reads the text of a specific sales order without charge item.

Reads the text data for a specific item. Consumers must pass the following key fields: sales order without charge ID and item number.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\ItemTextApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sales_order_without_charge = 'sales_order_without_charge_example'; // string | Sales Order Without Charge
$sales_order_without_charge_item = 'sales_order_without_charge_item_example'; // string | Sales Order Without Charge Item
$top = 50; // int | Show only the first n items, see [Paging - Top](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=66)
$skip = 56; // int | Skip the first n items, see [Paging - Skip](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=65)
$filter = 'filter_example'; // string | Filter items by property values, see [Filtering](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=64)
$inlinecount = 'inlinecount_example'; // string | Include count of items, see [Inlinecount](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=67)
$orderby = array('orderby_example'); // string[] | Order items by property values, see [Sorting](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=65)
$select = array('select_example'); // string[] | Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=68)
$expand = array('expand_example'); // string[] | Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page=63)

try {
    $result = $apiInstance->aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToTextGet($sales_order_without_charge, $sales_order_without_charge_item, $top, $skip, $filter, $inlinecount, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ItemTextApi->aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToTextGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sales_order_without_charge** | **string**| Sales Order Without Charge | |
| **sales_order_without_charge_item** | **string**| Sales Order Without Charge Item | |
| **top** | **int**| Show only the first n items, see [Paging - Top](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;66) | [optional] |
| **skip** | **int**| Skip the first n items, see [Paging - Skip](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;65) | [optional] |
| **filter** | **string**| Filter items by property values, see [Filtering](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;64) | [optional] |
| **inlinecount** | **string**| Include count of items, see [Inlinecount](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;67) | [optional] |
| **orderby** | [**string[]**](../Model/string.md)| Order items by property values, see [Sorting](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;65) | [optional] |
| **select** | [**string[]**](../Model/string.md)| Select properties to be returned, see [Select](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;68) | [optional] |
| **expand** | [**string[]**](../Model/string.md)| Expand related entities, see [Expand](https://help.sap.com/doc/5890d27be418427993fafa6722cdc03b/Cloud/en-US/OdataV2.pdf#page&#x3D;63) | [optional] |

### Return type

[**\BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper6**](../Model/Wrapper6.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSlsOrdWthoutChrgItmTextGet()`

```php
aSlsOrdWthoutChrgItmTextGet($top, $skip, $filter, $inlinecount, $orderby, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper6
```

Reads item texts of all sales order without charges.

Reads the text data from the items of all sales order without charges in the system.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\ItemTextApi(
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
    $result = $apiInstance->aSlsOrdWthoutChrgItmTextGet($top, $skip, $filter, $inlinecount, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ItemTextApi->aSlsOrdWthoutChrgItmTextGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper6**](../Model/Wrapper6.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDDelete()`

```php
aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDDelete($sales_order_without_charge, $sales_order_without_charge_item, $language, $long_text_id)
```

Deletes a specific item text.

Deletes a specific item text in a specific language. Consumers must pass the following key fields: sales order without charge ID, item number, language, and text ID.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\ItemTextApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sales_order_without_charge = 'sales_order_without_charge_example'; // string | Sales Order Without Charge
$sales_order_without_charge_item = 'sales_order_without_charge_item_example'; // string | Sales Order Without Charge Item
$language = 'language_example'; // string | Language Key
$long_text_id = 'long_text_id_example'; // string | Text ID

try {
    $apiInstance->aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDDelete($sales_order_without_charge, $sales_order_without_charge_item, $language, $long_text_id);
} catch (Exception $e) {
    echo 'Exception when calling ItemTextApi->aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDDelete: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sales_order_without_charge** | **string**| Sales Order Without Charge | |
| **sales_order_without_charge_item** | **string**| Sales Order Without Charge Item | |
| **language** | **string**| Language Key | |
| **long_text_id** | **string**| Text ID | |

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

## `aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDGet()`

```php
aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDGet($sales_order_without_charge, $sales_order_without_charge_item, $language, $long_text_id, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\ASlsOrdWthoutChrgItmTextType
```

Reads a specific item text.

Reads a specific item text in a specific language. Consumers must pass the following key fields: sales order without charge ID, item number, language, and text ID.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\ItemTextApi(
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
    $result = $apiInstance->aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDGet($sales_order_without_charge, $sales_order_without_charge_item, $language, $long_text_id, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ItemTextApi->aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\SalesOrderWOCharge\Model\ASlsOrdWthoutChrgItmTextType**](../Model/ASlsOrdWthoutChrgItmTextType.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDPatch()`

```php
aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDPatch($sales_order_without_charge, $sales_order_without_charge_item, $language, $long_text_id, $modified_a_sls_ord_wthout_chrg_itm_text_type)
```

Updates a specific item text.

Updates a specific item text in a specific language. Consumers must pass the following key fields: sales order without charge ID, item number, language, and text ID.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\ItemTextApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sales_order_without_charge = 'sales_order_without_charge_example'; // string | Sales Order Without Charge
$sales_order_without_charge_item = 'sales_order_without_charge_item_example'; // string | Sales Order Without Charge Item
$language = 'language_example'; // string | Language Key
$long_text_id = 'long_text_id_example'; // string | Text ID
$modified_a_sls_ord_wthout_chrg_itm_text_type = new \BeLenka\SAP\SalesOrderWOCharge\Model\ModifiedASlsOrdWthoutChrgItmTextType(); // \BeLenka\SAP\SalesOrderWOCharge\Model\ModifiedASlsOrdWthoutChrgItmTextType | New property values

try {
    $apiInstance->aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDPatch($sales_order_without_charge, $sales_order_without_charge_item, $language, $long_text_id, $modified_a_sls_ord_wthout_chrg_itm_text_type);
} catch (Exception $e) {
    echo 'Exception when calling ItemTextApi->aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDPatch: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sales_order_without_charge** | **string**| Sales Order Without Charge | |
| **sales_order_without_charge_item** | **string**| Sales Order Without Charge Item | |
| **language** | **string**| Language Key | |
| **long_text_id** | **string**| Text ID | |
| **modified_a_sls_ord_wthout_chrg_itm_text_type** | [**\BeLenka\SAP\SalesOrderWOCharge\Model\ModifiedASlsOrdWthoutChrgItmTextType**](../Model/ModifiedASlsOrdWthoutChrgItmTextType.md)| New property values | |

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\ItemTextApi(
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
    echo 'Exception when calling ItemTextApi->aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeGet: ', $e->getMessage(), PHP_EOL;
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

## `aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeItemGet()`

```php
aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeItemGet($sales_order_without_charge, $sales_order_without_charge_item, $language, $long_text_id, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeItemType
```

Reads the sales order without charge item for a specific item text.

Reads the sales order without charge item data for a specific text in a specific language. Consumers must pass the following key fields: sales order without charge ID, item number, language, and text ID.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\ItemTextApi(
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
    $result = $apiInstance->aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeItemGet($sales_order_without_charge, $sales_order_without_charge_item, $language, $long_text_id, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ItemTextApi->aSlsOrdWthoutChrgItmTextSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeItemGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeItemType**](../Model/ASalesOrderWithoutChargeItemType.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
