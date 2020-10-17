# GetDiscordRoles

{% api-method method="get" host="exports.Badger\_Discord\_API:GetDiscordRoles" path="\(user\)" %}
{% api-method-summary %}
GetDiscordRoles
{% endapi-method-summary %}

{% api-method-description %}
This export allows you to get a player's Discord roles within the server \(discord role IDs returned\).
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
Returns array of role IDs if found:
{% endapi-method-response-example-description %}

```text
{ 597446100206616596, 597450498060058624, 597929446124552192 }
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Returns false if not found:
{% endapi-method-response-example-description %}

```text
false
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

