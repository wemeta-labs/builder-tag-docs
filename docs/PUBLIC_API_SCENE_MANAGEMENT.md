
# Public API

**`POST /api/v1/public_api/scene_management/create_scene_tag`**

*Description:*

> Creates a scene and returns a scene tag to be implemented.

*Request Headers:*

    * `Content-Type: application/json`
    * `X-API-KEY: <token>`

*Request Body:*

    scene_friendly_name: string (required)
    email: string (required)

*Sample*:

>https://staging-api.wemeta.world/api/v1/public_api/scene_management/create_scene_tag

Body:
```
{
    "scene_friendly_name": "WeMeta Office Scene",
    "email": "wemeta@wemetalabs.com"
}
```

> [Response](./responses/create_scene_tag.json)

<br>
<br>

**`GET /api/v1/public_api/scene_management/create_scene_tag`**

*Description:*

> Returns all scene tags associated with an account.

*Request Headers:*

    * `Content-Type: application/json`
    * `X-API-KEY: <token>`

*Request Body:*

    email: string (required)

*Sample*:

>https://staging-api.wemeta.world/api/v1/public_api/scene_management/view_scenes

Body:
```
{
    "email": "wemeta@wemetalabs.com"
}
```

> [Response](./responses/view_scenes.json)

<br>
<br>
