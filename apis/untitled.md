---
description: APIs start with api/device
---

# Device APIs

{% api-method method="get" host="api/device" path="/devices" %}
{% api-method-summary %}
Get Devices
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get free cakes.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```
{
    "devices": [
        {
            "_id": "5f1067f533612a867c8c6763",
            "value": 0,
            "name": "node-1",
            "description": "A device for",
            "ipAddress": "192.168.56.1",
            "port": "5000",
            "historical": [
                {
                    "lastModified": 1594910709226,
                    "_id": "5f1067f533612a867c8c6764",
                    "value": 0
                }
            ],
            "hub": "5f1067c933612a867c8c675e",
            "lastModified": 1594910709227,
            "__v": 0
        },
    ]
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```
{    "message": "Ain't no cake like that."}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="device/api" path="/create" %}
{% api-method-summary %}
CREATE Device
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-form-data-parameters %}
{% api-method-parameter name="hubId" type="string" required=true %}
hub id. Can be obtained from hub.\_id
{% endapi-method-parameter %}

{% api-method-parameter name="name" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="ipAddress" type="string" required=true %}
sf
{% endapi-method-parameter %}

{% api-method-parameter name="port" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="description" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-form-data-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



{% api-method method="get" host="api/device" path="/get/:id" %}
{% api-method-summary %}
GET Device
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="id" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="patch" host="api/device" path="/update" %}
{% api-method-summary %}
UPDATE Device
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-form-data-parameters %}
{% api-method-parameter name="id" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="description" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="name" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="ipAddress" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="port" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-form-data-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "device": {
        "_id": "5f112161be3f819548d05e4f",
        "value": 0,
        "name": "device 1",
        "description": "a simple device",
        "ipAddress": "192.168.56.1",
        "port": "5001",
        "historical": [
            {
                "lastModified": 1594958177369,
                "_id": "5f112161be3f819548d05e50",
                "value": 0,
                "id": "5f112161be3f819548d05e50"
            }
        ],
        "hub": "5f1067d833612a867c8c675f",
        "lastModified": 1594958506914,
        "__v": 0,
        "id": "5f112161be3f819548d05e4f"
    }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



{% api-method method="delete" host="device/api" path="/delete/:id" %}
{% api-method-summary %}
DELETE Device
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="id" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Deleted device
{% endapi-method-response-example-description %}

```
{
    "device": {
        "_id": "5f1067f533612a867c8c6763",
        "value": 0,
        "name": "node-1",
        "description": "A device for",
        "ipAddress": "192.168.56.1",
        "port": "5000",
        "historical": [
            {
                "lastModified": 1594910709226,
                "_id": "5f1067f533612a867c8c6764",
                "value": 0,
                "id": "5f1067f533612a867c8c6764"
            }
        ],
        "hub": "5f1067c933612a867c8c675e",
        "lastModified": 1594910709227,
        "__v": 0,
        "id": "5f1067f533612a867c8c6763"
    }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



{% api-method method="patch" host="device/api" path="/updatevalue" %}
{% api-method-summary %}
Update Device Value
{% endapi-method-summary %}

{% api-method-description %}
Update only the value of given device
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-form-data-parameters %}
{% api-method-parameter name="id" type="string" required=true %}
device uuid
{% endapi-method-parameter %}

{% api-method-parameter name="value" type="string" required=true %}
new value
{% endapi-method-parameter %}
{% endapi-method-form-data-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "device": {
        "_id": "5f1067f533612a867c8c6763",
        "value": 0,
        "name": "node-1",
        "description": "A device for",
        "ipAddress": "192.168.56.1",
        "port": "5000",
        "historical": [
            {
                "lastModified": 1594910709226,
                "_id": "5f1067f533612a867c8c6764",
                "value": 0,
                "id": "5f1067f533612a867c8c6764"
            }
        ],
        "hub": "5f1067c933612a867c8c675e",
        "lastModified": 1594910709227,
        "__v": 0,
        "id": "5f1067f533612a867c8c6763"
    }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

