# ModelEmailOrder

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The email id | [optional] 
**object_name** | **string** | The email object name | [optional] 
**create** | [**\DateTime**](\DateTime.md) | Date of mail creation | [optional] 
**update** | [**\DateTime**](\DateTime.md) | Date of last mail update | [optional] 
**object** | [**\Swagger\Client\Model\ModelEmailOrderObject**](ModelEmailOrderObject.md) |  | [optional] 
**from** | **string** | The sender of the email | 
**to** | **string** | The recipient of the email | 
**subject** | **string** | The subject of the email | 
**text** | **string** | The text of the email | [optional] 
**sev_client** | [**\Swagger\Client\Model\ModelEmailOrderSevClient**](ModelEmailOrderSevClient.md) |  | [optional] 
**cc** | **string** | A list of mail addresses which are in the cc | [optional] 
**bcc** | **string** | A list of mail addresses which are in the bcc | [optional] 
**arrived** | [**\DateTime**](\DateTime.md) | Date the mail arrived | [optional] 

[[Back to Model list]](../../README.md#documentation-for-models) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to README]](../../README.md)

