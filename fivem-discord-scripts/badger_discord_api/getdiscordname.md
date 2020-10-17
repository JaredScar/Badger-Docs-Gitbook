# GetDiscordName

{% api-method method="get" host="exports.Badger\_Discord\_API:GetDiscordName" path="\(user\)" %}
{% api-method-summary %}
GetDiscordName
{% endapi-method-summary %}

{% api-method-description %}
This export allows you to get a player's Discord name.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="user" type="object" required=true %}
The source of the player you want to check.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Returns Discord name if found:
{% endapi-method-response-example-description %}

```text
'Badger'
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

