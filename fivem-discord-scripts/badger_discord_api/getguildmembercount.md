# GetGuildMemberCount

{% api-method method="get" host="exports.Badger\_Discord\_API:GetGuildMemberCount" path="\(\)" %}
{% api-method-summary %}
GetGuildMemberCount
{% endapi-method-summary %}

{% api-method-description %}
This export allows you to get the count of members \(including offline members\) on the server the script is connected to.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Returns member count if found:
{% endapi-method-response-example-description %}

```text
435
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

