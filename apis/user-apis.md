---
description: Authentication and Authorization
---

# Authentication APIs



{% api-method method="post" host="api/user/" path="login" %}
{% api-method-summary %}
Login
{% endapi-method-summary %}

{% api-method-description %}
Login to acquire a token
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="email" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="password" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Return user data with signed-in token. Token is only valid for 1 hour.
{% endapi-method-response-example-description %}

```
{
    "userId": "5ef5b4d2b56aad8240db229c",
    "email": "admin1@user.com",
    "userName": "admin1",
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI1ZWY1YjRkMmI1NmFhZDgyNDBkYjIyOWMiLCJ1c2VyTmFtZSI6ImFkbWluMSIsImVtYWlsIjoiYWRtaW4xQHVzZXIuY29tIiwiaWF0IjoxNTk0OTY3MDgxLCJleHAiOjE1OTQ5NzA2ODF9.DoHgM4XbGD94HHV-wFdL1vu__aAjs05oEAVMjB8gpS8"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="api/user" path="/signup" %}
{% api-method-summary %}
Sign Up
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="name" type="string" required=true %}
username
{% endapi-method-parameter %}

{% api-method-parameter name="email" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="password" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "userId": "5ef5b4d2b56aad8240db229c",
    "email": "admin1@user.com",
    "userName": "admin1",
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI1ZWY1YjRkMmI1NmFhZDgyNDBkYjIyOWMiLCJ1c2VyTmFtZSI6ImFkbWluMSIsImVtYWlsIjoiYWRtaW4xQHVzZXIuY29tIiwiaWF0IjoxNTk0OTY3MDgxLCJleHAiOjE1OTQ5NzA2ODF9.DoHgM4XbGD94HHV-wFdL1vu__aAjs05oEAVMjB8gpS8"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

