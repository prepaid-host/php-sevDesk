# ModelCreditNote

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The creditNote id. &lt;span style&#x3D;&#x27;color:red&#x27;&gt;Required&lt;/span&gt; if you want to create/update an credit note position for an existing credit note\&quot; | [optional] 
**object_name** | **string** | The creditNote object name | 
**map_all** | **bool** |  | 
**create** | [**\DateTime**](\DateTime.md) | Date of creditNote creation | [optional] 
**update** | [**\DateTime**](\DateTime.md) | Date of last creditNote update | [optional] 
**credit_note_number** | **string** | The creditNote number | 
**contact** | [**\Swagger\Client\Model\ModelCreditNoteContact**](ModelCreditNoteContact.md) |  | 
**credit_note_date** | [**\DateTime**](\DateTime.md) | Needs to be provided as timestamp or dd.mm.yyyy | 
**status** | **string** | Please have a look in       &lt;a href&#x3D;&#x27;https://api.sevdesk.de/#section/Types-and-status-of-credit-notes&#x27;&gt;status of credit note&lt;/a&gt;      to see what the different status codes mean | 
**header** | **string** | Normally consist of prefix plus the creditNote number | 
**head_text** | **string** | Certain html tags can be used here to format your text | [optional] 
**foot_text** | **string** | Certain html tags can be used here to format your text | [optional] 
**address_country** | [**\Swagger\Client\Model\ModelCreditNoteAddressCountry**](ModelCreditNoteAddressCountry.md) |  | 
**create_user** | [**\Swagger\Client\Model\ModelCreditNoteCreateUser**](ModelCreditNoteCreateUser.md) |  | [optional] 
**sev_client** | [**\Swagger\Client\Model\ModelCreditNoteSevClient**](ModelCreditNoteSevClient.md) |  | [optional] 
**delivery_terms** | **string** | Delivery terms of the creditNote | [optional] 
**payment_terms** | **string** | Payment terms of the creditNote | [optional] 
**version** | **int** | Version of the creditNote.&lt;br&gt;      Can be used if you have multiple drafts for the same creditNote.&lt;br&gt;      Should start with 0 | [optional] 
**small_settlement** | **bool** | Defines if the client uses the small settlement scheme.      If yes, the creditNote must not contain any vat | [optional] 
**contact_person** | [**\Swagger\Client\Model\ModelCreditNoteContactPerson**](ModelCreditNoteContactPerson.md) |  | 
**tax_rate** | **float** | Is overwritten by creditNote position tax rates | 
**tax_set** | [**\Swagger\Client\Model\ModelCreditNoteTaxSet**](ModelCreditNoteTaxSet.md) |  | [optional] 
**tax_text** | **string** | A common tax text would be &#x27;Umsatzsteuer 19%&#x27; | 
**tax_type** | **string** | Tax type of the creditNote. There are four tax types: 1. default - Umsatzsteuer ausweisen 2. eu - Steuerfreie innergemeinschaftliche Lieferung (Europäische Union) 3. noteu - Steuerschuldnerschaft des Leistungsempfängers (außerhalb EU, z. B. Schweiz) 4. custom - Using custom tax set 5. ss - Not subject to VAT according to §19 1 UStG Tax rates are heavily connected to the tax type used. | 
**credit_note_type** | **string** | Type of the creditNote. | [optional] 
**send_date** | [**\DateTime**](\DateTime.md) | The date the creditNote was sent to the customer | [optional] 
**address** | **string** | Complete address of the recipient including name, street, city, zip and country.&lt;br&gt;       Line breaks can be used and will be displayed on the invoice pdf. | [optional] 
**booking_category** | **string** | defines the booking category, for more information see the section \&quot;&lt;a href&#x3D;&#x27;https://api.sevdesk.de/#section/Credit-note-booking-categories&#x27;&gt;Credit note booking categories&lt;/a&gt;\&quot; | [optional] 
**currency** | **string** | Currency used in the creditNote. Needs to be currency code according to ISO-4217 | 
**sum_net** | **float** | Net sum of the creditNote | [optional] 
**sum_tax** | **float** | Tax sum of the creditNote | [optional] 
**sum_gross** | **float** | Gross sum of the creditNote | [optional] 
**sum_discounts** | **float** | Sum of all discounts in the creditNote | [optional] 
**sum_net_foreign_currency** | **float** | Net sum of the creditNote in the foreign currency | [optional] 
**sum_tax_foreign_currency** | **float** | Tax sum of the creditNote in the foreign currency | [optional] 
**sum_gross_foreign_currency** | **float** | Gross sum of the creditNote in the foreign currency | [optional] 
**sum_discounts_foreign_currency** | **float** | Discounts sum of the creditNote in the foreign currency | [optional] 
**customer_internal_note** | **string** | Internal note of the customer. Contains data entered into field &#x27;Referenz/Bestellnummer&#x27; | [optional] 
**show_net** | **bool** | If true, the net amount of each position will be shown on the creditNote. Otherwise gross amount | [optional] 
**send_type** | **string** | Type which was used to send the creditNote. IMPORTANT: Please refer to the creditNote section of the       *     API-Overview to understand how this attribute can be used before using it! | [optional] 

[[Back to Model list]](../../README.md#documentation-for-models) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to README]](../../README.md)

