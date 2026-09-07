# BuiltByBitApi.DownloadPlanAction

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **String** |  | 
**src** | **String** | The source file/directory. | [optional] 
**dst** | **String** | A destination file/directory relative to the server root. | [optional] 
**actions** | [**[DownloadPlanAction]**](DownloadPlanAction.md) | A set of subactions to execute in the context of this action. | [optional] 



## Enum: TypeEnum


* `copy` (value: `"copy"`)

* `copy_dir` (value: `"copy_dir"`)

* `open_zip` (value: `"open_zip"`)

* `server_restart` (value: `"server_restart"`)




