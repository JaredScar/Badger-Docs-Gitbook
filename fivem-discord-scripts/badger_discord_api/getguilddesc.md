# GetGuildDescription

{% api-method method="get" host="exports.Badger\_Discord\_API:GetGuildDescription" path="\(\)" %}
{% api-method-summary %}
GetGuildDescription
{% endapi-method-summary %}

{% api-method-description %}
This export allows you to get the server's description the script is connected to.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Returns server description if found:
{% endapi-method-response-example-description %}

```text
'Jared's Developer Community is a friendly community...'
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

