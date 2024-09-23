# BeLenka\SAP\SalesOrderWOCharge\ItemScheduleLineApi

All URIs are relative to https://:/sap/opu/odata/sap/API_SALES_ORDER_WITHOUT_CHARGE_SRV, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToScheduleLineGet()**](ItemScheduleLineApi.md#aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToScheduleLineGet) | **GET** /A_SalesOrderWithoutChargeItem(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;)/to_ScheduleLine | Reads the schedule lines of a specific sales order without charge item. |
| [**aSlsOrdWthoutChrgSchedLineGet()**](ItemScheduleLineApi.md#aSlsOrdWthoutChrgSchedLineGet) | **GET** /A_SlsOrdWthoutChrgSchedLine | Reads the schedule lines of all sales order without charges. |
| [**aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineGet()**](ItemScheduleLineApi.md#aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineGet) | **GET** /A_SlsOrdWthoutChrgSchedLine(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,ScheduleLine&#x3D;&#39;{ScheduleLine}&#39;) | Reads a specific schedule line. |
| [**aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineToItemGet()**](ItemScheduleLineApi.md#aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineToItemGet) | **GET** /A_SlsOrdWthoutChrgSchedLine(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,ScheduleLine&#x3D;&#39;{ScheduleLine}&#39;)/to_Item | Reads the sales order without charge item for a specific schedule line. |
| [**aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineToSalesOrderWithoutChargeGet()**](ItemScheduleLineApi.md#aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineToSalesOrderWithoutChargeGet) | **GET** /A_SlsOrdWthoutChrgSchedLine(SalesOrderWithoutCharge&#x3D;&#39;{SalesOrderWithoutCharge}&#39;,SalesOrderWithoutChargeItem&#x3D;&#39;{SalesOrderWithoutChargeItem}&#39;,ScheduleLine&#x3D;&#39;{ScheduleLine}&#39;)/to_SalesOrderWithoutCharge | Reads the sales order without charge header for a specific schedule line. |


## `aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToScheduleLineGet()`

```php
aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToScheduleLineGet($sales_order_without_charge, $sales_order_without_charge_item, $top, $skip, $filter, $inlinecount, $orderby, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper5
```

Reads the schedule lines of a specific sales order without charge item.

Reads the schedule line data for a specific item. Consumers must pass the following key fields: sales order without charge ID and item number.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\ItemScheduleLineApi(
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
    $result = $apiInstance->aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToScheduleLineGet($sales_order_without_charge, $sales_order_without_charge_item, $top, $skip, $filter, $inlinecount, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ItemScheduleLineApi->aSalesOrderWithoutChargeItemSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemToScheduleLineGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper5**](../Model/Wrapper5.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSlsOrdWthoutChrgSchedLineGet()`

```php
aSlsOrdWthoutChrgSchedLineGet($top, $skip, $filter, $inlinecount, $orderby, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper5
```

Reads the schedule lines of all sales order without charges.

Reads the schedule line data from the items of all sales order without charges in the system.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\ItemScheduleLineApi(
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
    $result = $apiInstance->aSlsOrdWthoutChrgSchedLineGet($top, $skip, $filter, $inlinecount, $orderby, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ItemScheduleLineApi->aSlsOrdWthoutChrgSchedLineGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\SalesOrderWOCharge\Model\Wrapper5**](../Model/Wrapper5.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineGet()`

```php
aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineGet($sales_order_without_charge, $sales_order_without_charge_item, $schedule_line, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\ASlsOrdWthoutChrgSchedLineType
```

Reads a specific schedule line.

Reads the schedule line data from a specific item of a specific sales order without charge. Consumers must pass the following key fields: sales order without charge ID, sales order without charge item, and schedule line number.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\ItemScheduleLineApi(
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
    $result = $apiInstance->aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineGet($sales_order_without_charge, $sales_order_without_charge_item, $schedule_line, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ItemScheduleLineApi->aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\SalesOrderWOCharge\Model\ASlsOrdWthoutChrgSchedLineType**](../Model/ASlsOrdWthoutChrgSchedLineType.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth), [OAuth2Auth](../../README.md#OAuth2Auth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineToItemGet()`

```php
aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineToItemGet($sales_order_without_charge, $sales_order_without_charge_item, $schedule_line, $select, $expand): \BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeItemType
```

Reads the sales order without charge item for a specific schedule line.

Reads the sales order without charge item data for a specific schedule line. Consumers must pass the following key fields: sales order without charge ID, item number, and schedule line number.

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\ItemScheduleLineApi(
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
    $result = $apiInstance->aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineToItemGet($sales_order_without_charge, $sales_order_without_charge_item, $schedule_line, $select, $expand);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ItemScheduleLineApi->aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineToItemGet: ', $e->getMessage(), PHP_EOL;
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

[**\BeLenka\SAP\SalesOrderWOCharge\Model\ASalesOrderWithoutChargeItemType**](../Model/ASalesOrderWithoutChargeItemType.md)

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


$apiInstance = new BeLenka\SAP\SalesOrderWOCharge\Api\ItemScheduleLineApi(
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
    echo 'Exception when calling ItemScheduleLineApi->aSlsOrdWthoutChrgSchedLineSalesOrderWithoutChargeSalesOrderWithoutChargeSalesOrderWithoutChargeItemSalesOrderWithoutChargeItemScheduleLineScheduleLineToSalesOrderWithoutChargeGet: ', $e->getMessage(), PHP_EOL;
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
