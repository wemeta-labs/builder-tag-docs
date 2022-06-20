# Public API

**`GET /api/v1/public_api/analytics_dashboard/floor_price`**

*Description:*

> Returns floor price time series data points depending on the time granularity.

*Request Parameters:*

    granularity: string (required) - Time granularity. Possible values: `day`, `week`, `month`, `all`.
    worlds: list (required) - World name. Possible values: `decentraland`, `cryptovoxels`, `somnium_space`, `the_sandbox`, `superworld`, `nft_worlds`.

*Sample*:

>https://staging-api.wemeta.world/api/v1/public_api/analytics_dashboard/floor_price?granularity=day&worlds=decentraland,nft_worlds,somnium_space,the_sandbox

> [Response](./responses/analytics_dashboard/unique_visitor_count.json)

<br>
<br>