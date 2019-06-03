# CheckDetail

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | CheckDetail ID | [optional] 
**AuxiliaryOnUs** | **string** | AuxiliaryOnUs identifies a code used on commercial checks at the discretion of the payor bank. | [optional] 
**ExternalProcessingCode** | **string** | ExternalProcessingCode identifies a code used for special purposes as authorized by the Accredited Standards Committee X9. Also known as Position 44. | [optional] 
**PayorBankRoutingNumber** | **string** | PayorBankRoutingNumber identifies a number that identifies the institution by or through which the item is payable. Must be a valid routing and transit number issued by the ABA’s Routing Number Registrar. Shall represent the first 8 digits of a 9-digit routing number or 8 numeric digits of a 4 dash 4 routing number. A valid routing number consists of 2 fields: the eight- digit Payor Bank Routing Number  and the one-digit Payor Bank Routing Number Check Digit.  | [optional] 
**PayorBankCheckDigit** | **string** | PayorBankCheckDigit identifies a digit representing the routing number check digit.  The combination of Payor Bank Routing Number and payor Bank Routing Number Check Digit must be a mod-checked routing number with a valid check digit.  | [optional] 
**OnUs** | **string** | OnUs identifies data specified by the payor bank. On-Us data usually consists of the payor’s account number, a serial number or transaction code, or both. | [optional] 
**ItemAmount** | **int32** | Amount identifies the amount of the check.  All amounts fields have two implied decimal points. e.g., 100000 is $1,000.00 | [optional] 
**ECEInstitutionItemSequenceNumber** | **string** | ECEInstitutionItemSequenceNumber identifies a number assigned by the institution that creates the CheckDetail. Field must contain a numeric value. It cannot be all blanks. | [optional] 
**DocumentationTypeIndicator** | **string** | DocumentationTypeIndicator identifies a code that indicates the type of documentation that supports the check record.  This field is superseded by the Cash Letter Documentation Type Indicator in the Cash Letter Header Record for all Defined Values except ‘Z’ Not Same Type. In the case of Defined Value of ‘Z’, the Documentation Type Indicator in this record takes precedent.  Shall be present when Cash Letter Documentation Type Indicator in the Cash Letter Header Record is Defined Value of ‘Z’.  * &#x60;A&#x60; - No image provided, paper provided separately * &#x60;B&#x60; - No image provided, paper provided separately, image upon request * &#x60;C&#x60; - Image provided separately, no paper provided * &#x60;D&#x60; - Image provided separately, no paper provided, image upon request * &#x60;E&#x60; - Image and paper provided separately * &#x60;F&#x60; - Image and paper provided separately, image upon request * &#x60;G&#x60; - Image included, no paper provided * &#x60;H&#x60; - Image included, no paper provided, image upon request * &#x60;I&#x60; - Image included, paper provided separately * &#x60;J&#x60; - Image included, paper provided separately, image upon request * &#x60;K&#x60; - No image provided, no paper provided * &#x60;L&#x60; - No image provided, no paper provided, image upon request * &#x60;M&#x60; - No image provided, Electronic Check provided separately  | [optional] 
**ReturnAcceptanceIndicator** | **string** | ReturnAcceptanceIndicator is a code that indicates whether the institution that creates the CheckDetail will or will not support electronic return processing.  * &#x60;0&#x60; - Will not accept any electronic information * &#x60;1&#x60; - Will accept preliminary return notifications, returns, and final return notifications * &#x60;2&#x60; - Will accept preliminary return notifications and returns * &#x60;3&#x60; - Will accept preliminary return notifications and final return notifications * &#x60;4&#x60; - Will accept returns and final return notifications * &#x60;5&#x60; - Will accept preliminary return notifications only * &#x60;6&#x60; - Will accept returns only * &#x60;7&#x60; - Will accept final return notifications only * &#x60;8&#x60; - Will accept preliminary return notifications, returns, final return notifications, and image returns * &#x60;9&#x60; - Will accept preliminary return notifications, returns and image returns * &#x60;A&#x60; - Will accept preliminary return notifications, final return notifications and image returns * &#x60;B&#x60; - Will accept returns, final return notifications and image returns * &#x60;C&#x60; - Will accept preliminary return notifications and image returns * &#x60;D&#x60; - Will accept returns and image returns * &#x60;E&#x60; - Will accept final return notifications and image returns * &#x60;F&#x60; - Will accept image returns only  | [optional] 
**MICRValidIndicator** | **string** | MICRValidIndicator is a code that indicates whether any character in the Magnetic Ink Character Recognition (MICR) property is unreadable, or the OnUs property is missing from the CheckDetail. * &#x60;1&#x60; - Good read * &#x60;2&#x60; - Good read, missing field * &#x60;3&#x60; - Read error encountered * &#x60;4&#x60; - Missing field and read error encountered  | [optional] 
**BOFDIndicator** | **string** | BOFDIndicator is a code that indicates whether the ECE institution indicated on the Bundle Header Record (Type 20) is the Bank of First Deposit (BOFD). This field shall be consistent with values contained in the Check Detail Addendum A Record (Type 26) and Check Detail Addendum C Record (Type 28). * &#x60;Y&#x60; - ECE institution is BOFD * &#x60;N&#x60; - ECE institution is not BOFD * &#x60;U&#x60; - ECE institution relationship to BOFD is undetermined  | [optional] 
**AddendumCount** | **int32** | AddendumCount is a number of Check Detail Record Addenda to follow. This represents the number of CheckDetailAddendumA, CheckDetailAddendumB and CheckDetailAddendumC types.  It matches the total number of addendum records associated with this item. The standard supports up to 99 addendum records. | [optional] 
**CorrectionIndicator** | **string** | CorrectionIndicator identifies whether and how the MICR line was repaired, for fields other than Payor Bank Routing Number and Amount. * &#x60;0&#x60; - No Repair * &#x60;1&#x60; - Repaired (form of repair unknown) * &#x60;2&#x60; - Repaired without Operator intervention * &#x60;3&#x60; - Repaired with Operator intervention * &#x60;4&#x60; - Undetermined if repair has been done or not  | [optional] 
**ArchiveTypeIndicator** | **string** | ArchiveTypeIndicator is a code that indicates the type of archive that supports this CheckDetail. Access method, availability and time-frames shall be defined by clearing arrangements.  * &#x60;A&#x60; - Microfilm * &#x60;B&#x60; - Image * &#x60;C&#x60; - Paper * &#x60;D&#x60; - Microfilm and image * &#x60;E&#x60; - Microfilm and paper * &#x60;F&#x60; - Image and paper * &#x60;G&#x60; - Microfilm, image and paper * &#x60;H&#x60; - Electronic Check Instrument * &#x60;I&#x60; - None  | [optional] 
**CheckDetailAddendumA** | [**CheckDetailAddendumA**](CheckDetailAddendumA.md) |  | [optional] 
**CheckDetailAddendumB** | [**CheckDetailAddendumB**](CheckDetailAddendumB.md) |  | [optional] 
**CheckDetailAddendumC** | [**CheckDetailAddendumC**](CheckDetailAddendumC.md) |  | [optional] 
**ImageViewDetail** | [**ImageViewDetail**](ImageViewDetail.md) |  | [optional] 
**ImageViewData** | [**ImageViewData**](ImageViewData.md) |  | [optional] 
**ImageViewAnalysis** | [**ImageViewAnalysis**](ImageViewAnalysis.md) |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

