---
description: 명상 지도 만족도 서비스
---

# RecordMeditationAction

{% api-method method="post" host="http://stac.gondr.net" path="/nugu/RecordMeditationAction" %}
{% api-method-summary %}
RecordMeditationAction
{% endapi-method-summary %}

{% api-method-description %}
NUGU SDK
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="score" type="integer" required=false %}
명상 점수
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```
{output: "오늘의 명상점수 : {{score}}" } or {output: "오늘의 명상점수 : {{score}} 오늘 명상점수는 {{score}}으로 가장 최근의 명상점수인 {{prevScore}}점보다 좋아졌네요. 좋은 하루 되세요."}
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



