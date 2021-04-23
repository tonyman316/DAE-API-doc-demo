# Requesting Hazard Types

To request the list of hazard types configured in the system please use the route defined here:

[https://enterprise.disasteraware.com/hp\_srv/\#!/hazards/getHazard\_TypesTokenServer\_JSON](https://enterprise.disasteraware.com/hp_srv/)

{% api-method method="get" host="https://enterprise.disasteraware.com/hazards/1/json/get\_hazard\_types" path="" %}
{% api-method-summary %}
Get hazard types
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="hazard id" type="number" required=false %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
[
  {
    "type_id": "string",
    "type_name": "string",
    "type_icon": "string"
  }
]
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

This request will return an array that contains all of the hazard types.  Each element in the array will have three properties:

1. **type\_id** - This is like the primary key for the hazard type.  This is the value that will be found on the hazard object.
2. **type\_name** - A human readable value for the hazard e.g. Volcano
3. **type\_icon** - This is the url for the hazard type icon’s image e.g. avalanche.png. The hazard icons are hosted at:[ https://static.pdc.org/icons/hazard/large/](https://static.pdc.org/icons/hazard/large/).  To construct the fully qualified location for the hazard type’s icon combine the host location with type\_icon value.



