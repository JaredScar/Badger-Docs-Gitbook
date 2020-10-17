# CheckEqual

{% api-method method="get" host="exports.Badger\_Discord\_API:CheckEqual" path="\(role1, role2\);" %}
{% api-method-summary %}
CheckEqual
{% endapi-method-summary %}

{% api-method-description %}
This export allows you to get a Discord role ID from what it is named on the Guild.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="roleName" type="string" required=true %}
The name of the Discord role you want the ID for.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Number of role ID will be returned:
{% endapi-method-response-example-description %}

```text
761459588058185738
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a role with the name provided:
{% endapi-method-response-example-description %}

```text
nil
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

