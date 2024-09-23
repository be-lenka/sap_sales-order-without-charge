# BeLenka\SAP\SalesOrderWOCharge\HeaderPartnerApi

All URIs are relative to https://:/sap/opu/odata/sap/API_SALES_ORDER_WITHOUT_CHARGE_SRV, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**aSalesOrderWithoutChargeSalesOrderWithoutChargeToPartnerGet()**](HeaderPartnerApi.md#aSalesOrderWithoutChargeSalesOrderWithoutChargeToPartnerGet) | **GET** /A_SalesOrderWithoutCharge(&#39;{SalesOrderWithoutCharge}&#39;)/to_Partner | Reads the header partners of a specific sales order without charge. |
| [**aSlsOrdWthoutChrgPartnerGet()**](HeaderPartnerApi.md#aSlsOrdWthoutChrgPartnerGet) | **GET** /A_SlsOrdWthoutChrgPartner | Reads the header partners of all sales order without charges. |
| [**aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionDelete()**](HeaderPartnerApi.md#aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionDelete) | **DELETE** /A_SlsOrdWthoutChrgPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;) | Deletes the header partners of a specific sales order without charge and with a specific partner function. |
| [**aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionGet()**](HeaderPartnerApi.md#aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionGet) | **GET** /A_SlsOrdWthoutChrgPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;) | Reads the header partners of a specific sales order without charge and with a specific partner function. |
| [**aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionPatch()**](HeaderPartnerApi.md#aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionPatch) | **PATCH** /A_SlsOrdWthoutChrgPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;) | Updates the header partners of a specific sales order without charge and with a specific partner function. |
| [**aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionToSalesOrderWithoutChargeGet()**](HeaderPartnerApi.md#aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionToSalesOrderWithoutChargeGet) | **GET** /A_SlsOrdWthoutChrgPartner(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,PartnerFunction&#x3D;&#39;{PartnerFunction}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific header partner. |


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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\HeaderPartnerApi(
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
    echo 'Exception when calling HeaderPartnerApi->aSalesOrderWithoutChargeSalesOrderWithoutChargeToPartnerGet: ', $e->getMessage(), PHP_EOL;
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

## `aSlsOrdWthoutChrgPartnerGet()`

```php
aSlsOrdWthoutChrgPartnerGet($top, $skip, $filter, $inlinecount, $orderby, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper2
```

Reads the header partners of all sales order without charges.

Reads the partner data from the headers of all sales order without charges in the system. The data is relevant for all items for which no item-specific partners are maintained.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\HeaderPartnerApi(
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
    $result = $apiInstance->aSlsOrdWthoutChrgPartnerGet($top, $skip, $filter, $inlinecount, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HeaderPartnerApi->aSlsOrdWthoutChrgPartnerGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper2**](../Model/Wrapper2.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionDelete()`

```php
aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionDelete($sales_order_without_charge, $partner_function)
```

Deletes the header partners of a specific sales order without charge and with a specific partner function.

Deletes the data of partners with a specific partner function from the header of a specific sales order without charge. Consumers must pass the following key fields: sales order without charge ID and partner function.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\HeaderPartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sales_order_without_charge = 'sales_order_without_charge_example'; // string | Sales Order Without Charge
$partner_function = 'partner_function_example'; // string | Partner Function

try {
    $apiInstance->aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionDelete($sales_order_without_charge, $partner_function);
} catch (Exception $e) {
    echo 'Exception when calling HeaderPartnerApi->aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionDelete: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sales_order_without_charge** | **string**| Sales Order Without Charge | |
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

## `aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionGet()`

```php
aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionGet($sales_order_without_charge, $partner_function, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\ASlsOrdWthoutChrgPartnerType
```

Reads the header partners of a specific sales order without charge and with a specific partner function.

Reads the data of partners with a specific partner function from the header of a specific sales order without charge. Consumers must pass the following key fields: sales order without charge ID and partner function.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\HeaderPartnerApi(
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
    $result = $apiInstance->aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionGet($sales_order_without_charge, $partner_function, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HeaderPartnerApi->aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\SalesOrderWOCharge\Model\ASlsOrdWthoutChrgPartnerType**](../Model/ASlsOrdWthoutChrgPartnerType.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionPatch()`

```php
aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionPatch($sales_order_without_charge, $partner_function, $modified_a_sls_ord_wthout_chrg_partner_type)
```

Updates the header partners of a specific sales order without charge and with a specific partner function.

Updates the data of partners with a specific partner function from the header of a specific sales order without charge. Consumers must pass the following key fields: sales order without charge ID and partner function.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\HeaderPartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sales_order_without_charge = 'sales_order_without_charge_example'; // string | Sales Order Without Charge
$partner_function = 'partner_function_example'; // string | Partner Function
$modified_a_sls_ord_wthout_chrg_partner_type = new \BeLenka\SAP\SalesOrderWOCharge\Model\ModifiedASlsOrdWthoutChrgPartnerType(); // \BeLenka\SAP\SalesOrderWOCharge\Model\ModifiedASlsOrdWthoutChrgPartnerType | New property values

try {
    $apiInstance->aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionPatch($sales_order_without_charge, $partner_function, $modified_a_sls_ord_wthout_chrg_partner_type);
} catch (Exception $e) {
    echo 'Exception when calling HeaderPartnerApi->aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionPatch: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sales_order_without_charge** | **string**| Sales Order Without Charge | |
| **partner_function** | **string**| Partner Function | |
| **modified_a_sls_ord_wthout_chrg_partner_type** | [**\BeLenka\SAP\SalesOrderWOCharge\Model\ModifiedASlsOrdWthoutChrgPartnerType**](../Model/ModifiedASlsOrdWthoutChrgPartnerType.md)| New property values | |

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\HeaderPartnerApi(
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
    echo 'Exception when calling HeaderPartnerApi->aSlsOrdWthoutChrgPartnerSalesOrderWithoutChargeSalesOrderWithoutChargePartnerFunctionPartnerFunctionToSalesOrderWithoutChargeGet: ', $e->getMessage(), PHP_EOL;
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
