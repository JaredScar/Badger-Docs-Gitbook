# GetGuildRoleList

{% api-method method="get" host="exports.Badger\_Discord\_API:GetGuildRoleList" path="\(\)" %}
{% api-method-summary %}
GetGuildRoleList
{% endapi-method-summary %}

{% api-method-description %}
This export allows you to get all of the server's roles with their role names and role IDs correspondent to each other.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Returns associative array if found:
{% endapi-method-response-example-description %}

```text
{ 
    ['Founder'] = 597446100206616596, 
    ['Staff'] = 597450498060058624, 
    ['Java Developer'] = 597928420017438725 
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Returns nil if not found:
{% endapi-method-response-example-description %}

```text
nil
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

