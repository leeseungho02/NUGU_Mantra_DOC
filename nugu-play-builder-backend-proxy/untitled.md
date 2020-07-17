# StartWhitenoiseAction

{% api-method method="get" host="http://stac.gondr.net" path="/nugu/StartWhitenoiseAction" %}
{% api-method-summary %}
Get Cakes
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get free cakes.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="whitenoise\_type" type="string" required=false %}
실행할 백색소음 종류
{% endapi-method-parameter %}

{% api-method-parameter name="whitenoise\_playing\_hour" type="integer" required=false %}
실행 시간 : 시
{% endapi-method-parameter %}

{% api-method-parameter name="whitenoise\_playing\_minute" type="integer" required=false %}
실행 시간 : 분
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```
{ output:"{{whitenoise_playing_time}} 동안, {{whitenoise_type}} 백색소음을 재생할게요." }
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```
{    "message": "Ain't no cake like that."}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



