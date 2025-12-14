
# ListOrganizationsResponseDto


## Properties

Name | Type
------------ | -------------
`organizations` | [Array&lt;Organization&gt;](Organization.md)

## Example

```typescript
import type { ListOrganizationsResponseDto } from '@cashful-co/typescript'

// TODO: Update the object below with actual values
const example = {
  "organizations": [{"id":"org_123","name":"Acme Corp","metadata":{}}],
} satisfies ListOrganizationsResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ListOrganizationsResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


