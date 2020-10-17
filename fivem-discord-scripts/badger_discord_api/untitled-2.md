# GetDiscordEmail

{% api-method method="get" host="exports.Badger\_Discord\_API:GetDiscordEmail" path="\(user\)" %}
{% api-method-summary %}
GetDiscordEmail
{% endapi-method-summary %}

{% api-method-description %}
This export allows you to get a player's Discord email if allowed
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="user" type="object" required=true %}
The source of the player you want to check
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Returns email of user if found:
{% endapi-method-response-example-description %}

```text
'thewolfbadger@gmail.com'
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

