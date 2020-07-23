# Hub APIs

{% api-method method="get" host="api/hub" path="/get/:id" %}
{% api-method-summary %}
GET Hub
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get free cakes.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="id" type="string" required=true %}
hub id
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```
{
    "hub": {
        "devices": [],
        "_id": "5f1067d833612a867c8c675f",
        "name": "hub-2",
        "description": "long-sentenceslong-sentences",
        "ipAddress": "192.27.221.30",
        "port": "3000",
        "lastModified": 1594910680898,
        "id": "5f1067d833612a867c8c675f"
    }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="api/hub" path="/create" %}
{% api-method-summary %}
CREATE Hub
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="name" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="description" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="ipAddress" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="port" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "hub": {
        "devices": [],
        "_id": "5f1067d833612a867c8c675f",
        "name": "hub-2",
        "description": "long-sentenceslong-sentences",
        "ipAddress": "192.27.221.30",
        "port": "3000",
        "lastModified": 1594910680898,
        "id": "5f1067d833612a867c8c675f"
    }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="patch" host="api/hub" path="/update" %}
{% api-method-summary %}
UPDATE Hub
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="id" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="name" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="description" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="ipAddress" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="port" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Updated hub 
{% endapi-method-response-example-description %}

```
{
    "hub": {
        "devices": [],
        "_id": "5f1067d833612a867c8c675f",
        "name": "hub-2",
        "description": "long-sentenceslong-sentences",
        "ipAddress": "192.27.221.30",
        "port": "3000",
        "lastModified": 1594910680898,
        "id": "5f1067d833612a867c8c675f"
    }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="delete" host="api/hub" path="/delete:id" %}
{% api-method-summary %}
DELETE Hub
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
deleted hub
{% endapi-method-response-example-description %}

```
{
    "hub": {
        "devices": [],
        "_id": "5f1067d833612a867c8c675f",
        "name": "hub-2",
        "description": "long-sentenceslong-sentences",
        "ipAddress": "192.27.221.30",
        "port": "3000",
        "lastModified": 1594910680898,
        "id": "5f1067d833612a867c8c675f"
    }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

