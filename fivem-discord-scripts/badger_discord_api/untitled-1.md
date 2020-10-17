# IsDiscordEmailVerified

{% api-method method="get" host="exports.Badger\_Discord\_API:IsDiscordEmailVerified" path="\(user\)" %}
{% api-method-summary %}
IsDiscordEmailVerified
{% endapi-method-summary %}

{% api-method-description %}
This export allows you to check if a player has their Discord email verified.
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
Returns true if email is verified:
{% endapi-method-response-example-description %}

```text
true
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Returns false if email is not verified \[returns nil if data returned is nil\]:
{% endapi-method-response-example-description %}

```text
false
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

