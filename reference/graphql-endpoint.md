# GraphQL Endpoint

{% hint style="info" %}
Full type reference generated from the schema can be found [here](../graphql-api/queries.md).
{% endhint %}

{% api-method method="post" host="https://apiv2.whitehead.ai" path="/v1/graphql" %}
{% api-method-summary %}
Query
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to query our GraphQL schema.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Authentication token to identify the user.
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-query-parameters %}
{% api-method-parameter name="query" type="string" %}
Valid GraphQL query as a string.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
If the query is successfully executed, its output is returned as follows:
{% endapi-method-response-example-description %}

```text
{
  "data": {
    "<SERVICE_NAME>": {
      "result": ...
    }
  }
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=400 %}
{% api-method-response-example-description %}
If there are any client errors, an appropriate error code and message will be returned.
{% endapi-method-response-example-description %}

```
{
  "errors": [...]
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



