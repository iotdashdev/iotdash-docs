# Command APIs

{% api-method method="get" host="api/command" path="/hub/ping/:id" %}
{% api-method-summary %}
Ping Hub
{% endapi-method-summary %}

{% api-method-description %}
Ping hub to check connectivity
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="id" type="string" required=true %}
hub.\_id
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Hub server is current running and connected.  Return hub data if connected.
{% endapi-method-response-example-description %}

```
{
    hub: {...hubData}
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="api/command" path="/device/ping/:id" %}
{% api-method-summary %}
Ping Device
{% endapi-method-summary %}

{% api-method-description %}
Device server is running and connected. Return device data
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="id" type="string" required=true %}
device.\_id
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    device: {...device data}
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="api/command" path="/hub/ping/:id" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="id" type="string" required=true %}
hub.\_id
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Hub server is current running and connected.  Return hub data if connected.
{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="api/command" path="/create" %}
{% api-method-summary %}
CREATE Command
{% endapi-method-summary %}

{% api-method-description %}
Send a command to device. Response OK if command is send successfully.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="deviceId" type="string" required=true %}
device.\_id
{% endapi-method-parameter %}

{% api-method-parameter name="type" type="string" required=true %}
type of command
{% endapi-method-parameter %}

{% api-method-parameter name="content" type="string" required=true %}
content of command
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
command is created and send to device
{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

