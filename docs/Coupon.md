# BuiltByBitApi.Coupon

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**couponId** | **Number** |  | [optional] 
**userId** | **Number** |  | [optional] 
**label** | **String** | This is the code a buyer would enter at checkout. | [optional] 
**discount** | **Number** | The discount to apply. Either a fixed value, or a decimal percent. Depends on the &#39;percent&#39; field. | [optional] 
**percent** | **Boolean** | If true, the &#39;discount&#39; field represents a decimal percentage.  If false, the &#39;discount&#39; field represents an absolute $ USD value. | [optional] 
**allContentTypes** | **[String]** |  A list of content types for which this coupon code applies to without requiring an entry. Eg. if you created the coupon with the &#39;All resources&#39; option selected, this list will include \&quot;resource\&quot;. | [optional] 
**createdAt** | **Number** | A UNIX timestamp. | [optional] 
**expiresAt** | **Number** | A UNIX timestamp. | [optional] 
**maxUses** | **Number** |  | [optional] 
**maxPerUserUses** | **Number** |  | [optional] 
**uses** | **Number** |  | [optional] 
**active** | **Boolean** | Whether or not the coupon code is active and can still be used at checkout. Accounts for the expiry date if set and the max use limit if set. | [optional] 


