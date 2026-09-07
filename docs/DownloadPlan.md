# BuiltByBitApi.DownloadPlan

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**level** | **String** |  | 
**actions** | [**[DownloadPlanAction]**](DownloadPlanAction.md) |  | [optional] 
**notices** | [**[DownloadPlanNotice]**](DownloadPlanNotice.md) |  | [optional] 
**unsupported** | **[String]** | A list of features which were unsupported (not passed into the &#39;supported&#39; query paramter) which were needed, resulting in the plan level being downgraded to &#39;manual&#39;. | [optional] 
**requiresEmptyServer** | **String** | Whether the server files must be empty before exeucting the plan steps. | [optional] 



## Enum: LevelEnum


* `full` (value: `"full"`)

* `partial` (value: `"partial"`)

* `manual` (value: `"manual"`)




