# BeLenka\SAP\SalesOrderWOCharge\ItemPartnerApi

All URIs are relative to https://:/sap/opu/odata/sap/API_SALES_ORDER_WITHOUT_CHARGE_SRV, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToPartnerGet()**](ItemPartnerApi.md#aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToPartnerGet) | **GET** /A_SalesOrderWithoutChargeItem(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;)/to_Partner | Reads the item partners of a specific sales order without charge item. |
| [**aSlsOrdWthoutChrgItmPartnerGet()**](ItemPartnerApi.md#aSlsOrdWthoutChrgItmPartnerGet) | **GET** /A_SlsOrdWthoutChrgItmPartner | Reads the item partners for all sales order without charges. |
| [**aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionDelete()**](ItemPartnerApi.md#aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionDelete) | **DELETE** /A_SlsOrdWthoutChrgItmPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;) | Deletes the item partners of a specific item with a specific partner function in a specific sales order without charge. |
| [**aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionGet()**](ItemPartnerApi.md#aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionGet) | **GET** /A_SlsOrdWthoutChrgItmPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;) | Reads the item partners of a specific item with a specific partner function in a specific sales order without charge. |
| [**aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionPatch()**](ItemPartnerApi.md#aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionPatch) | **PATCH** /A_SlsOrdWthoutChrgItmPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;) | Updates the item partners of a specific item with a specific partner function in a specific sales order without charge. |
| [**aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionToItemGet()**](ItemPartnerApi.md#aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionToItemGet) | **GET** /A_SlsOrdWthoutChrgItmPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;)/to_Item | Reads the sales order without charge item for a specific partner function of a sales order without charge item. |
| [**aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionToSalesOrderWithoutChargeGet()**](ItemPartnerApi.md#aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionToSalesOrderWithoutChargeGet) | **GET** /A_SlsOrdWthoutChrgItmPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific partner function of a sales order without charge item. |


## `aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToPartnerGet()`

```php
aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToPartnerGet($sales_order_without_charge, $sales_order_without_charge_item, $top, $skip, $filter, $inlinecount, $orderby, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper4
```

Reads the item partners of a specific sales order without charge item.

Reads the partner data for a specific item of a specific sales order without charge. Consumers must pass the following key fields: sales order without charge ID and item number.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\ItemPartnerApi(
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
    $result = $apiInstance->aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToPartnerGet($sales_order_without_charge, $sales_order_without_charge_item, $top, $skip, $filter, $inlinecount, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ItemPartnerApi->aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToPartnerGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper4**](../Model/Wrapper4.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSlsOrdWthoutChrgItmPartnerGet()`

```php
aSlsOrdWthoutChrgItmPartnerGet($top, $skip, $filter, $inlinecount, $orderby, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper4
```

Reads the item partners for all sales order without charges.

Reads the partner data from the items of all sales order without charges in the system.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\ItemPartnerApi(
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
    $result = $apiInstance->aSlsOrdWthoutChrgItmPartnerGet($top, $skip, $filter, $inlinecount, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ItemPartnerApi->aSlsOrdWthoutChrgItmPartnerGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper4**](../Model/Wrapper4.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionDelete()`

```php
aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionDelete($sales_order_without_charge, $sales_order_without_charge_item, $partner_function)
```

Deletes the item partners of a specific item with a specific partner function in a specific sales order without charge.

Deletes the item partners with a specific partner function of a specific sales order without charge item. Consumers must pass the following key fields: sales order without charge ID, item number, and partner function.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\ItemPartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sales_order_without_charge = 'sales_order_without_charge_example'; // string | Sales Order Without Charge
$sales_order_without_charge_item = 'sales_order_without_charge_item_example'; // string | Sales Order Without Charge Item
$partner_function = 'partner_function_example'; // string | Partner Function

try {
    $apiInstance->aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionDelete($sales_order_without_charge, $sales_order_without_charge_item, $partner_function);
} catch (Exception $e) {
    echo 'Exception when calling ItemPartnerApi->aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionDelete: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sales_order_without_charge** | **string**| Sales Order Without Charge | |
| **sales_order_without_charge_item** | **string**| Sales Order Without Charge Item | |
| **partner_function** | **string**| Partner Function | |

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

## `aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionGet()`

```php
aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionGet($sales_order_without_charge, $sales_order_without_charge_item, $partner_function, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\ASlsOrdWthoutChrgItmPartnerType
```

Reads the item partners of a specific item with a specific partner function in a specific sales order without charge.

Reads the item partners with a specific partner function of a specific sales order without charge item. Consumers must pass the following key fields: sales order without charge ID, item number, and partner function.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\ItemPartnerApi(
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
    $result = $apiInstance->aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionGet($sales_order_without_charge, $sales_order_without_charge_item, $partner_function, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ItemPartnerApi->aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\SalesOrderWOCharge\Model\ASlsOrdWthoutChrgItmPartnerType**](../Model/ASlsOrdWthoutChrgItmPartnerType.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionPatch()`

```php
aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionPatch($sales_order_without_charge, $sales_order_without_charge_item, $partner_function, $modified_a_sls_ord_wthout_chrg_itm_partner_type)
```

Updates the item partners of a specific item with a specific partner function in a specific sales order without charge.

Updates the item partners with a specific partner function of a specific sales order without charge item. Consumers must pass the following key fields: sales order without charge ID, item number, and partner function.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\ItemPartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sales_order_without_charge = 'sales_order_without_charge_example'; // string | Sales Order Without Charge
$sales_order_without_charge_item = 'sales_order_without_charge_item_example'; // string | Sales Order Without Charge Item
$partner_function = 'partner_function_example'; // string | Partner Function
$modified_a_sls_ord_wthout_chrg_itm_partner_type = new \BeLenka\SAP\SalesOrderWOCharge\Model\ModifiedASlsOrdWthoutChrgItmPartnerType(); // \BeLenka\SAP\SalesOrderWOCharge\Model\ModifiedASlsOrdWthoutChrgItmPartnerType | New property values

try {
    $apiInstance->aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionPatch($sales_order_without_charge, $sales_order_without_charge_item, $partner_function, $modified_a_sls_ord_wthout_chrg_itm_partner_type);
} catch (Exception $e) {
    echo 'Exception when calling ItemPartnerApi->aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionPatch: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sales_order_without_charge** | **string**| Sales Order Without Charge | |
| **sales_order_without_charge_item** | **string**| Sales Order Without Charge Item | |
| **partner_function** | **string**| Partner Function | |
| **modified_a_sls_ord_wthout_chrg_itm_partner_type** | [**\BeLenka\SAP\SalesOrderWOCharge\Model\ModifiedASlsOrdWthoutChrgItmPartnerType**](../Model/ModifiedASlsOrdWthoutChrgItmPartnerType.md)| New property values | |

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

## `aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionToItemGet()`

```php
aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionToItemGet($sales_order_without_charge, $sales_order_without_charge_item, $partner_function, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeItemType
```

Reads the sales order without charge item for a specific partner function of a sales order without charge item.

Reads the sales order without charge item data for a specific item partner function. Consumers must pass the following key fields: sales order without charge ID, item number, and partner function.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\ItemPartnerApi(
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
    $result = $apiInstance->aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionToItemGet($sales_order_without_charge, $sales_order_without_charge_item, $partner_function, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ItemPartnerApi->aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionToItemGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeItemType**](../Model/ASalesOrderWithoutChargeItemType.md)

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\ItemPartnerApi(
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
    echo 'Exception when calling ItemPartnerApi->aSlsOrdWthoutChrgItmPartnerSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemPartnerFunctionPartnerFunctionToSalesOrderWithoutChargeGet: ', $e->getMessage(), PHP_EOL;
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
