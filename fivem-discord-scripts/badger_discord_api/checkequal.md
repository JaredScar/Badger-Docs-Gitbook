# CheckEqual

{% api-method method="get" host="exports.Badger\_Discord\_API:CheckEqual" path="\(role1, role2\)" %}
{% api-method-summary %}
CheckEqual
{% endapi-method-summary %}

{% api-method-description %}
This export allows you to check if a Discord role ID is equal to a Discord role Name, this can also check if a Discord role ID is equal to Badger\_Discord\_API config's RoleList role reference.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="role2" type="number" required=true %}
The 2nd role ID you are comparing.
{% endapi-method-parameter %}

{% api-method-parameter name="role2" type="string" required=true %}
The 2nd role name or role reference you are comparing.
{% endapi-method-parameter %}

{% api-method-parameter name="role1" type="number" required=true %}
The role ID.
{% endapi-method-parameter %}

{% api-method-parameter name="role1" type="string" required=true %}
The role name or role reference.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Returns true if the roles are considered equal:
{% endapi-method-response-example-description %}

```
true
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Returns false if the roles are not considered equal:
{% endapi-method-response-example-description %}

```text
false
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

