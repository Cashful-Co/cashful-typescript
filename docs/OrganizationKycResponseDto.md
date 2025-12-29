
# OrganizationKycResponseDto


## Properties

Name | Type
------------ | -------------
`id` | string
`createdAt` | Date
`updatedAt` | Date
`deletedAt` | Date
`organizationId` | string
`idNumber` | string
`companyRegistrationName` | string
`companyRegistrationNumber` | string
`companyTradingName` | string
`vatRegistrationNumber` | string
`industry` | string
`subIndustry` | string
`estimatedAnnualTurnover` | string
`businessDescription` | string
`companyEmail` | string
`companyContactNumber` | string
`website` | string
`socialMedia` | string
`accountContactNumber` | string
`customerSupportContactNumber` | string
`customerSupportEscalationContactNumber` | string
`emergencyContactNumber` | string
`streetAddress` | string
`apartment` | string
`suburb` | string
`city` | string
`postalCode` | string
`bank` | string
`accountType` | string
`accountName` | string
`accountNumber` | string
`branchCode` | string
`isSouthAfricanResidentAccount` | boolean
`certificateOfIncorporation` | string
`identityDocuments` | string
`bankAccountConfirmationLetter` | string
`proofOfBusinessAddress` | string
`ecnsLicense` | string
`termsAccepted` | boolean
`acceptedAt` | Date
`currentStep` | string
`isCompleted` | boolean
`completionScore` | number

## Example

```typescript
import type { OrganizationKycResponseDto } from '@cashful-co/typescript'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "createdAt": null,
  "updatedAt": null,
  "deletedAt": null,
  "organizationId": null,
  "idNumber": null,
  "companyRegistrationName": null,
  "companyRegistrationNumber": null,
  "companyTradingName": null,
  "vatRegistrationNumber": null,
  "industry": null,
  "subIndustry": null,
  "estimatedAnnualTurnover": null,
  "businessDescription": null,
  "companyEmail": null,
  "companyContactNumber": null,
  "website": null,
  "socialMedia": null,
  "accountContactNumber": null,
  "customerSupportContactNumber": null,
  "customerSupportEscalationContactNumber": null,
  "emergencyContactNumber": null,
  "streetAddress": null,
  "apartment": null,
  "suburb": null,
  "city": null,
  "postalCode": null,
  "bank": null,
  "accountType": null,
  "accountName": null,
  "accountNumber": null,
  "branchCode": null,
  "isSouthAfricanResidentAccount": null,
  "certificateOfIncorporation": null,
  "identityDocuments": null,
  "bankAccountConfirmationLetter": null,
  "proofOfBusinessAddress": null,
  "ecnsLicense": null,
  "termsAccepted": null,
  "acceptedAt": null,
  "currentStep": null,
  "isCompleted": null,
  "completionScore": null,
} satisfies OrganizationKycResponseDto

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as OrganizationKycResponseDto
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


