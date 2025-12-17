# CheckoutsApi

All URIs are relative to *http://localhost:3000*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createCheckoutSession**](CheckoutsApi.md#createcheckoutsession) | **POST** /api/canary/checkout/sessions | Create Hosted Checkout |
| [**listAllCheckoutSessionsInternal**](CheckoutsApi.md#listallcheckoutsessionsinternal) | **GET** /api/canary/checkout/sessions | List All Checkout Sessions |
| [**retrieveCheckoutSessionInternal**](CheckoutsApi.md#retrievecheckoutsessioninternal) | **GET** /api/canary/checkout/sessions/{id} | Retrieve Checkout Session |



## createCheckoutSession

> CheckoutSessionResponseDto createCheckoutSession(createCheckoutSessionDto)

Create Hosted Checkout

Creates a hosted payment page. Used for: (1) A standard e-commerce purchase, or (2) a \&quot;Pay-In\&quot; to fund a CustomerBalance.

### Example

```ts
import {
  Configuration,
  CheckoutsApi,
} from '@cashful-co/typescript';
import type { CreateCheckoutSessionRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CheckoutsApi(config);

  const body = {
    // CreateCheckoutSessionDto | Checkout session details
    createCheckoutSessionDto: ...,
  } satisfies CreateCheckoutSessionRequest;

  try {
    const data = await api.createCheckoutSession(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **createCheckoutSessionDto** | [CreateCheckoutSessionDto](CreateCheckoutSessionDto.md) | Checkout session details | |

### Return type

[**CheckoutSessionResponseDto**](CheckoutSessionResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Checkout session created successfully |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listAllCheckoutSessionsInternal

> Array&lt;CheckoutSessionResponseDto&gt; listAllCheckoutSessionsInternal(merchantId, limit, offset)

List All Checkout Sessions

Lists all checkout sessions across all merchants (internal use only)

### Example

```ts
import {
  Configuration,
  CheckoutsApi,
} from '@cashful-co/typescript';
import type { ListAllCheckoutSessionsInternalRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CheckoutsApi(config);

  const body = {
    // string | The ID of the merchant. This parameter is required.
    merchantId: merchantId_example,
    // number | Maximum number of records to return (optional)
    limit: 8.14,
    // number | Number of records to skip (optional)
    offset: 8.14,
  } satisfies ListAllCheckoutSessionsInternalRequest;

  try {
    const data = await api.listAllCheckoutSessionsInternal(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **merchantId** | `string` | The ID of the merchant. This parameter is required. | [Defaults to `undefined`] |
| **limit** | `number` | Maximum number of records to return | [Optional] [Defaults to `undefined`] |
| **offset** | `number` | Number of records to skip | [Optional] [Defaults to `undefined`] |

### Return type

[**Array&lt;CheckoutSessionResponseDto&gt;**](CheckoutSessionResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successfully retrieved checkout sessions |  -  |
| **400** | Bad Request - Invalid input |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## retrieveCheckoutSessionInternal

> CheckoutSessionResponseDto retrieveCheckoutSessionInternal(id)

Retrieve Checkout Session

Retrieves details of a specific checkout session

### Example

```ts
import {
  Configuration,
  CheckoutsApi,
} from '@cashful-co/typescript';
import type { RetrieveCheckoutSessionInternalRequest } from '@cashful-co/typescript';

async function example() {
  console.log("🚀 Testing @cashful-co/typescript SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CheckoutsApi(config);

  const body = {
    // string | The unique identifier of the checkout session
    id: id_example,
  } satisfies RetrieveCheckoutSessionInternalRequest;

  try {
    const data = await api.retrieveCheckoutSessionInternal(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | `string` | The unique identifier of the checkout session | [Defaults to `undefined`] |

### Return type

[**CheckoutSessionResponseDto**](CheckoutSessionResponseDto.md)

### Authorization

[bearer](../README.md#bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successfully retrieved checkout session |  -  |
| **401** | Unauthorized |  -  |
| **404** | Resource not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

