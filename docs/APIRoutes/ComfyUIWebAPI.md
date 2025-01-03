# SwarmUI API Documentation - ComfyUIWebAPI

> This is a subset of the API docs, see [/docs/API.md](/docs/API.md) for general info.

(CLASS DESCRIPTION NOT SET)

#### Table of Contents:

- HTTP Route [ComfyDeleteWorkflow](#http-route-apicomfydeleteworkflow)
- HTTP Route [ComfyEnsureRefreshable](#http-route-apicomfyensurerefreshable)
- HTTP Route [ComfyGetGeneratedWorkflow](#http-route-apicomfygetgeneratedworkflow)
- HTTP Route [ComfyInstallFeatures](#http-route-apicomfyinstallfeatures)
- HTTP Route [ComfyListWorkflows](#http-route-apicomfylistworkflows)
- HTTP Route [ComfyReadWorkflow](#http-route-apicomfyreadworkflow)
- HTTP Route [ComfySaveWorkflow](#http-route-apicomfysaveworkflow)
- WebSocket Route [DoLoraExtractionWS](#websocket-route-apidoloraextractionws)
- WebSocket Route [DoTensorRTCreateWS](#websocket-route-apidotensorrtcreatews)

## HTTP Route /API/ComfyDeleteWorkflow

#### Description

(ROUTE DESCRIPTION NOT SET)

#### Permission Flag

`comfy_edit_workflows` - `ComfyUI Edit Workflows` in group `ComfyUI`

#### Parameters

| Name | Type | Description | Default |
| --- | --- | --- | --- |
| name | String | (PARAMETER DESCRIPTION NOT SET) | **(REQUIRED)** |

#### Return Format

```js
(RETURN INFO NOT SET)
```

## HTTP Route /API/ComfyEnsureRefreshable

#### Description

(ROUTE DESCRIPTION NOT SET)

#### Permission Flag

`comfy_direct_calls` - `ComfyUI Direct Calls` in group `ComfyUI`

#### Parameters

**None.**

#### Return Format

```js
(RETURN INFO NOT SET)
```

## HTTP Route /API/ComfyGetGeneratedWorkflow

#### Description

(ROUTE DESCRIPTION NOT SET)

#### Permission Flag

`comfy_direct_calls` - `ComfyUI Direct Calls` in group `ComfyUI`

#### Parameters

| Name | Type | Description | Default |
| --- | --- | --- | --- |
| rawInput | JObject | (PARAMETER DESCRIPTION NOT SET) | **(REQUIRED)** |

#### Return Format

```js
(RETURN INFO NOT SET)
```

## HTTP Route /API/ComfyInstallFeatures

#### Description

(ROUTE DESCRIPTION NOT SET)

#### Permission Flag

`install_features` - `Install New Features` in group `Control`

#### Parameters

| Name | Type | Description | Default |
| --- | --- | --- | --- |
| features | String | (PARAMETER DESCRIPTION NOT SET) | **(REQUIRED)** |

#### Return Format

```js
(RETURN INFO NOT SET)
```

## HTTP Route /API/ComfyListWorkflows

#### Description

(ROUTE DESCRIPTION NOT SET)

#### Permission Flag

`comfy_read_workflows` - `ComfyUI Read Workflows` in group `ComfyUI`

#### Parameters

**None.**

#### Return Format

```js
(RETURN INFO NOT SET)
```

## HTTP Route /API/ComfyReadWorkflow

#### Description

(ROUTE DESCRIPTION NOT SET)

#### Permission Flag

`comfy_read_workflows` - `ComfyUI Read Workflows` in group `ComfyUI`

#### Parameters

| Name | Type | Description | Default |
| --- | --- | --- | --- |
| name | String | (PARAMETER DESCRIPTION NOT SET) | **(REQUIRED)** |

#### Return Format

```js
(RETURN INFO NOT SET)
```

## HTTP Route /API/ComfySaveWorkflow

#### Description

(ROUTE DESCRIPTION NOT SET)

#### Permission Flag

`comfy_edit_workflows` - `ComfyUI Edit Workflows` in group `ComfyUI`

#### Parameters

| Name | Type | Description | Default |
| --- | --- | --- | --- |
| name | String | (PARAMETER DESCRIPTION NOT SET) | **(REQUIRED)** |
| workflow | String | (PARAMETER DESCRIPTION NOT SET) | **(REQUIRED)** |
| prompt | String | (PARAMETER DESCRIPTION NOT SET) | **(REQUIRED)** |
| custom_params | String | (PARAMETER DESCRIPTION NOT SET) | **(REQUIRED)** |
| param_values | String | (PARAMETER DESCRIPTION NOT SET) | **(REQUIRED)** |
| image | String | (PARAMETER DESCRIPTION NOT SET) | **(REQUIRED)** |
| description | String | (PARAMETER DESCRIPTION NOT SET) | (Empty String) |
| enable_in_simple | Boolean | (PARAMETER DESCRIPTION NOT SET) | `False` |
| replace | String | (PARAMETER DESCRIPTION NOT SET) | (null) |

#### Return Format

```js
(RETURN INFO NOT SET)
```

## WebSocket Route /API/DoLoraExtractionWS

#### Description

(ROUTE DESCRIPTION NOT SET)

#### Permission Flag

`extra_loras` - `Extract LoRAs` in group `Control`

#### Parameters

| Name | Type | Description | Default |
| --- | --- | --- | --- |
| baseModel | String | (PARAMETER DESCRIPTION NOT SET) | **(REQUIRED)** |
| otherModel | String | (PARAMETER DESCRIPTION NOT SET) | **(REQUIRED)** |
| rank | Int32 | (PARAMETER DESCRIPTION NOT SET) | **(REQUIRED)** |
| outName | String | (PARAMETER DESCRIPTION NOT SET) | **(REQUIRED)** |

#### Return Format

```js
(RETURN INFO NOT SET)
```

## WebSocket Route /API/DoTensorRTCreateWS

#### Description

(ROUTE DESCRIPTION NOT SET)

#### Permission Flag

`create_tensorrt` - `Create TensorRT Models` in group `Control`

#### Parameters

| Name | Type | Description | Default |
| --- | --- | --- | --- |
| model | String | (PARAMETER DESCRIPTION NOT SET) | **(REQUIRED)** |
| aspect | String | (PARAMETER DESCRIPTION NOT SET) | **(REQUIRED)** |
| aspectRange | String | (PARAMETER DESCRIPTION NOT SET) | **(REQUIRED)** |
| optBatch | Int32 | (PARAMETER DESCRIPTION NOT SET) | **(REQUIRED)** |
| maxBatch | Int32 | (PARAMETER DESCRIPTION NOT SET) | **(REQUIRED)** |

#### Return Format

```js
(RETURN INFO NOT SET)
```

