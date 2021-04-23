# API example

{% api-method method="get" host="https://enterprise.disasteraware.com" path="/hazards/t/json/get\_hazard\_type" %}
{% api-method-summary %}
Get hazard type
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get hazard type
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
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

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```
{    "message": "hazard type not found."}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://enterprise.disasteraware.com" path="/hazards/t/json/search\_hazard" %}
{% api-method-summary %}
Search hazard
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="pagination" type="object" required=false %}

{% endapi-method-parameter %}

{% api-method-parameter name="order" type="object" required=false %}

{% endapi-method-parameter %}

{% api-method-parameter name="restrictions" type="array" required=false %}

{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation.
{% endapi-method-response-example-description %}

```
[
  {
    "app_ID": 0,
    "app_IDs": "string",
    "autoexpire": "string",
    "category_ID": "string",
    "charter_Uri": "string",
    "comment_Text": "string",
    "create_Date": "2021-04-23T00:59:56.664Z",
    "creator": "string",
    "end_Date": "2021-04-23T00:59:56.664Z",
    "glide_Uri": "string",
    "hazard_ID": 0,
    "hazard_Name": "string",
    "last_Update": "2021-04-23T00:59:56.664Z",
    "latitude": 0,
    "longitude": 0,
    "master_Incident_ID": "string",
    "message_ID": "string",
    "org_ID": 0,
    "severity_ID": "string",
    "snc_url": "string",
    "start_Date": "2021-04-23T00:59:56.664Z",
    "status": "string",
    "type_ID": "string",
    "update_Date": "2021-04-23T00:59:56.664Z",
    "update_User": "string",
    "product_total": "string",
    "uuid": "string",
    "in_Dashboard": "string",
    "areabrief_url": "string",
    "description": "string",
    "roles": [
      "string"
    ]
  }
]
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=400 %}
{% api-method-response-example-description %}
Unrecognized parameter.
{% endapi-method-response-example-description %}

```
{
  "status": "OK",
  "message": "string"
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Authentication failed.
{% endapi-method-response-example-description %}

```
{
  "status": "OK",
  "message": "string"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

Example

```text
{
 "pagination":{
    "page": 2,
    "pagesize": 20
 },
 "order":{
    "orderlist":{"latitude": "DESC", "longitude": "ASC"}
 },
 "restrictions": [
 [
    {
     "searchType": "LIKE",
     "hazardName": "Matthew"
    },
    {
     "searchType": "GREATER_THAN",
     "hazardId": 50
    }
 ],
 [
    {
     "searchType": "LIKE",
     "hazardName": "Earthquake"
    }
 ]
]
}
```

