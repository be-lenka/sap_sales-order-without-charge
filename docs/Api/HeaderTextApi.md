# BeLenka\SAP\SalesOrderWOCharge\HeaderTextApi

All URIs are relative to https://:/sap/opu/odata/sap/API_SALES_ORDER_WITHOUT_CHARGE_SRV, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**aSalesOrderWithoutChargeSalesOrderWithoutChargeToTextGet()**](HeaderTextApi.md#aSalesOrderWithoutChargeSalesOrderWithoutChargeToTextGet) | **GET** /A_SalesOrderWithoutCharge(&#39;{SalesOrderWithoutCharge}&#39;)/to_Text | Reads the header texts of a specific sales order without charge. |
| [**aSlsOrdWthoutChrgTextGet()**](HeaderTextApi.md#aSlsOrdWthoutChrgTextGet) | **GET** /A_SlsOrdWthoutChrgText | Reads the header texts of all sales order without charges. |
| [**aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDDelete()**](HeaderTextApi.md#aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDDelete) | **DELETE** /A_SlsOrdWthoutChrgText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;) | Deletes a specific header text for a specific sales order without charge. |
| [**aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDGet()**](HeaderTextApi.md#aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDGet) | **GET** /A_SlsOrdWthoutChrgText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;) | Reads a specific header text for a specific sales order without charge. |
| [**aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDPatch()**](HeaderTextApi.md#aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDPatch) | **PATCH** /A_SlsOrdWthoutChrgText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;) | Updates a specific header text for a specific sales order without charge. |
| [**aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeGet()**](HeaderTextApi.md#aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeGet) | **GET** /A_SlsOrdWthoutChrgText(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,Language&#x3D;&#39;{Language}&#39;,LongTextID&#x3D;&#39;{LongTextID}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific header text. |


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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\HeaderTextApi(
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
    echo 'Exception when calling HeaderTextApi->aSalesOrderWithoutChargeSalesOrderWithoutChargeToTextGet: ', $e->getMessage(), PHP_EOL;
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

## `aSlsOrdWthoutChrgTextGet()`

```php
aSlsOrdWthoutChrgTextGet($top, $skip, $filter, $inlinecount, $orderby, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper3
```

Reads the header texts of all sales order without charges.

Reads the text data from the headers of all sales order without charges in the system.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\HeaderTextApi(
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
    $result = $apiInstance->aSlsOrdWthoutChrgTextGet($top, $skip, $filter, $inlinecount, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HeaderTextApi->aSlsOrdWthoutChrgTextGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper3**](../Model/Wrapper3.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDDelete()`

```php
aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDDelete($sales_order_without_charge, $language, $long_text_id)
```

Deletes a specific header text for a specific sales order without charge.

Deletes the text data from the header of a specific sales order without charge. Consumers must pass the following key fields: sales order without charge ID, language, and text ID.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\HeaderTextApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sales_order_without_charge = 'sales_order_without_charge_example'; // string | Sales Order Without Charge
$language = 'language_example'; // string | Language Key
$long_text_id = 'long_text_id_example'; // string | Text ID

try {
    $apiInstance->aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDDelete($sales_order_without_charge, $language, $long_text_id);
} catch (Exception $e) {
    echo 'Exception when calling HeaderTextApi->aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDDelete: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sales_order_without_charge** | **string**| Sales Order Without Charge | |
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

## `aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDGet()`

```php
aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDGet($sales_order_without_charge, $language, $long_text_id, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\ASlsOrdWthoutChrgTextType
```

Reads a specific header text for a specific sales order without charge.

Reads the text data from the header of a specific sales order without charge. Consumers must pass the following key fields: sales order without charge ID, language, and text ID.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\HeaderTextApi(
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
    $result = $apiInstance->aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDGet($sales_order_without_charge, $language, $long_text_id, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HeaderTextApi->aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\SalesOrderWOCharge\Model\ASlsOrdWthoutChrgTextType**](../Model/ASlsOrdWthoutChrgTextType.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDPatch()`

```php
aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDPatch($sales_order_without_charge, $language, $long_text_id, $modified_a_sls_ord_wthout_chrg_text_type)
```

Updates a specific header text for a specific sales order without charge.

Updates the text data from the header of a specific sales order without charge. Consumers must pass the following key fields: sales order without charge ID, language, and text ID.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\HeaderTextApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sales_order_without_charge = 'sales_order_without_charge_example'; // string | Sales Order Without Charge
$language = 'language_example'; // string | Language Key
$long_text_id = 'long_text_id_example'; // string | Text ID
$modified_a_sls_ord_wthout_chrg_text_type = new \BeLenka\SAP\SalesOrderWOCharge\Model\ModifiedASlsOrdWthoutChrgTextType(); // \BeLenka\SAP\SalesOrderWOCharge\Model\ModifiedASlsOrdWthoutChrgTextType | New property values

try {
    $apiInstance->aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDPatch($sales_order_without_charge, $language, $long_text_id, $modified_a_sls_ord_wthout_chrg_text_type);
} catch (Exception $e) {
    echo 'Exception when calling HeaderTextApi->aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDPatch: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sales_order_without_charge** | **string**| Sales Order Without Charge | |
| **language** | **string**| Language Key | |
| **long_text_id** | **string**| Text ID | |
| **modified_a_sls_ord_wthout_chrg_text_type** | [**\BeLenka\SAP\SalesOrderWOCharge\Model\ModifiedASlsOrdWthoutChrgTextType**](../Model/ModifiedASlsOrdWthoutChrgTextType.md)| New property values | |

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\HeaderTextApi(
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
    echo 'Exception when calling HeaderTextApi->aSlsOrdWthoutChrgTextSalesOrderWithoutChargeSalesOrderWithoutChargeLanguageLanguageLongTextIDLongTextIDToSalesOrderWithoutChargeGet: ', $e->getMessage(), PHP_EOL;
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
