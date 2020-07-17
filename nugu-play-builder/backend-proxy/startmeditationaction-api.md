---
description: 명상 지도 시작 서비스
---

# StartMeditationAction

{% api-method method="post" host="http://stac.gondr.net" path="/nugu/StartMeditationAction" %}
{% api-method-summary %}
StartMeditationAction
{% endapi-method-summary %}

{% api-method-description %}
NUGU SDK
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="meditation\_playing\_hour" type="integer" required=false %}
재생시간 : 시
{% endapi-method-parameter %}

{% api-method-parameter name="meditation\_playing\_minute" type="integer" required=false %}
재생 시간 : 분
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```
{ output: "{{meditation_playing_hour}}시 {{meditation_playing_minute}}분 동안, 명상 실행" }
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```
{output: "연결 실패 했습니다."}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



