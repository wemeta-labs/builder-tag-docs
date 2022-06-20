
# Public API

**`GET /api/v1/public_api/unique_visitor_count`**

*Description:*

> Returns the number of unique visitors of a specific scene with multiple time granularities.

*Request Parameters:*

    scene_tag: string (required)

*Sample*:

>https://staging-api.wemeta.world/api/v1/public_api/unique_visitor_count?scene_tag=900cf53c-d927-42e0-ab66-a3992e08d057

> [Response](./responses/unique_visitor_count.json)

<br>
<br>


**`GET /api/v1/public_api/active_visitor_count`**

*Description:*

> Returns the number of active visitors of a specific parcel coordinate. If start_time is specified, the response will be the number of active visitors between the start_time and now.


*Request Parameters:*

    parcel_coord: string (required)
    start_time: int (optional) - default is one day ago

*Sample*:

>https://staging-api.wemeta.world/api/v1/public_api/active_visitor_count?parcel_coord=-132,90

> [Response](./responses/active_visitor_count.json)

<br>
<br>


**`GET /api/v1/public_api/visit_time`**

*Description:*

> Returns multiple variations of visit time of a specific scene with avg, total, median and histograms for total time, total active time, and total idle time with multiple time granularities.


*Request Parameters:*

    scene_tag: string (required)

*Sample*:

>https://staging-api.wemeta.world/api/v1/public_api/visit_time?scene_tag=900cf53c-d927-42e0-ab66-a3992e08d057

>[Response](./responses/visit_time.json)

<br>
<br>


**`GET /api/v1/public_api/number_of_sessions_per_visitor`**

*Description:*

> Returns the number of sessions per visitor for a specific scene with average, median, and histograms for the number of sessions per visitor with multiple time granularities.


*Request Parameters:*

    scene_tag: string (required)

*Sample*:

>https://staging-api.wemeta.world/api/v1/public_api/number_of_sessions_per_visitor?scene_tag=900cf53c-d927-42e0-ab66-a3992e08d057

> [Response](./responses/number_of_sessions_per_visitor.json)


<br>
<br>



**`GET /api/v1/public_api/foottraffic_by_parcel`**

*Description:*

> Returns the foot traffic by parcel for a specific scene with multiple time granularities.


*Request Parameters:*

    scene_tag: string (required)

*Sample:*

>https://staging-api.wemeta.world/api/v1/public_api/foottraffic_by_parcel?scene_tag=900cf53c-d927-42e0-ab66-a3992e08d057

> [Response](./responses/foottraffic_by_parcel.json)


<br>
<br>

**`GET /api/v1/public_api/wearables`**

*Description:*

> Returns the wearables used in a specific scene with the number of players and percentage of players using the wearable with multiple time granularities.


*Request Parameters:*

    scene_tag: string (required)

*Sample*:

>https://staging-api.wemeta.world/api/v1/public_api/wearables?scene_tag=900cf53c-d927-42e0-ab66-a3992e08d057

> [Response](./responses/wearables.json)

<br>
<br>

**`POST /api/v1/public_api/parcels_foottraffic_catalyst`**

*Description:*

> Returns the current foottraffic of specified parcels from decentraland's catalyst server.

*Request Body:*

    parcels: list[string] (required)

*Sample*:

>https://staging-api.wemeta.world/api/v1/public_api/parcels_foottraffic_catalyst

Body:
```
{
    "parcels": [
        "0,0", "0,1"
    ]
}

```

> [Response](./responses/parcels_foottraffic_catalyst.json)
